# CellDeleteInsertMove
UITableViewCell的高度刷新，点击删除、移动、插入以及左滑删除的实现/n
1.利用UITableView的beginUpdates和endUpdates 实现动画改变cell的高度，
2.点击cell使其移动到顶部-(void)moveRowAtIndexPath:(NSIndexPath *)indexPath toIndexPath:(NSIndexPath *)newIndexPath（移动指定cell）以及-(void)moveSection:(NSInteger)section toSection:(NSInteger)newSection（移动整个section）
3.删除点击的cell -(void)deleteRowsAtIndexPaths:(NSArray<NSIndexPath *> *)indexPaths withRowAnimation:(UITableViewRowAnimation)animation以及- (void)deleteSections:(NSIndexSet *)sections withRowAnimation:(UITableViewRowAnimation)animation
4.指定cell插入到指定位置- (void)insertRowsAtIndexPaths:(NSArray<NSIndexPath *> *)indexPaths withRowAnimation:(UITableViewRowAnimation)animation以及- (void)insertSections:(NSIndexSet *)sections withRowAnimation:(UITableViewRowAnimation)animation
5.左滑删除或置顶cell - (NSArray<UITableViewRowAction *> *)tableView:(UITableView *)tableView editActionsForRowAtIndexPath:(NSIndexPath *)indexPath
