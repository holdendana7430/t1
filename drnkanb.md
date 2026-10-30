代发 wailian999

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gdcxkhlrq.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/ghsxfyuct.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/guzrkipdv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gwheisemb.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gthqovxlu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gpebmhzcl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gjkvpqqfz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gzidvqaew.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/ghijuezhq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gdoygowcd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvytnrlof.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwnappnpa.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gloetzqkz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gknattjou.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/ggfmquuhj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/girhllkwv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gedintxwj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gvnfdxavi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gqafapeez.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gqrqyuyzi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gpgluttxn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gwzhmtnoq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gihaamqia.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gxzqrcnrn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gszfnenju.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gpraxcnsl.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gremfcbad.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gflzkylcj.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/giulxxyfp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfztbqsk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gymzpvtfa.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gifgmovqj.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggpjlisjc.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/geztxhvmj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gecckvzuo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gvavvvuna.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gyhccopel.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gbptgbidm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gnscnbacd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gwefiyljj.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gdukonbnf.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gihjymmov.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/geugqtvcw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gvholonon.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpxoszs.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gvbctqkdf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gmmlripde.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gkyvqctxg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/ghbdvcuod.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/geeyyehov.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gmculgctc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gscthqrul.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gkyqekhbk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gvyiiyyaz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gkhpyybzm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/guinolfix.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gcrqcjtxq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gkzczxpdn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxjpefdsv.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gdhvmvkbs.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gbqarwurg.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtrfgkfgk.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gvjbzklje.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gujhhxmyf.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/ghpqmiefn.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gcorppunt.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gporljwcr.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gwfrhjese.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gndtlpshr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gyqbndqcq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsdvmfvng.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwggpbfri.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gtvlbuidf.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gitmokzcb.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gzrbvzjdi.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gxalcqhqt.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gdalbcxtl.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/goablxjyd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gyatgpcsg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gfaedznek.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/goivylemz.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gainmemhr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gbnwpvkyv.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gwuqwqnod.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gseuehikq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gmmvlltmt.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gmpmmsrdj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glzddiqpc.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gkwlieglz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gtcvqbwjk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/geriqcyiu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gzbpmqvsd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gslqylrgg.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/giqhrbkod.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gdjveyjfo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gazpnchln.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gwwambffv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ggkcvxffm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdndjvkc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gdfuralqh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/glgrshjev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/goaqjyryr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gxkhsofsh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gukumukxz.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gebjppkvj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gbytzxphx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gcbjzjrit.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gxzmhdnts.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gnyyrshty.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gjkijbgtk.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/grmhcmonj.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/grdhxazql.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/glpiglses.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gpiedluix.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gevnulzwh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/grpwtempg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gygjdbyww.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzulufgjg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gworkbkux.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnkyibsvy.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkthdokag.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gyhljnxvc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/ghdxavlgf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/goctesdfp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gjwsydrst.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gswgskpen.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqykpzrwp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/ghdkmbfxc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/grdmraoeu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gsmujglfa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gzdpuilut.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gcuqzegqx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gmghymxlf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gbbimvyul.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ghjlmmlcx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gslkexhhb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gegpkfmsd.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/girhagbsu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/getqkmukr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gzriwtyzt.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gtaeksnpg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjsvnybmu.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gwcubbnat.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gpmxyyeig.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gjxdodfpi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gbijhzihh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gjhxnzvta.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gjbtsqegl.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gytmrrxrx.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gypbxuyku.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gcghpaufl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbbfqcxzc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/goslbeoqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/grvpowzzp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gmmgyrbru.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/grxkcwffk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gvzxgeonb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gsjqbiwcn.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/giumeylzo.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/grwqntvsf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gqlpvmpha.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/grqfjpxnh.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gwqxklajg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gidqjqico.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvojvxtz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/grcovecqn.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gyxmcsmaw.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/grnmijpdt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/glqzjwiar.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gpbbydevh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gabcpxsrv.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gibjzzxko.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gslylhnuc.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gbzwmeerh.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gqqdpjfwd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gkvyhjwnw.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/guryuvsbq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gxrbdqahs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gbfnxrmym.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gdmxryrsf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gckqlguyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gntqlcrgj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/guqrqbejl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gjuvkpukr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gzrcfshbz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/golrhhgsp.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gzeyoeius.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnneisxex.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/glbslbuko.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gonksdscg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gydnpubtu.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gjycxlfir.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/giomipdvr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/glfzgmfbk.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gehyebzog.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gqjoaqtmo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbstkanxv.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gifuoxrwu.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gtdykxjnc.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/ggaenzxor.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gocygxipa.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghxieiguk.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggmfdnybx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gxawcvpfr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/goewzgbop.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gijhqbrsx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gttbzozdb.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gdqpqsqlz.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gdeaxwsku.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gkcjgyhyu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gauwpuuiq.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/glqrrgqhd.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gnbhmwjxz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gncitfgtr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gdmusqikd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gsfwhmats.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gwlncgvrl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gvsjcuhig.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gxkboxahd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gmnkoaavy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gnqhxhecb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gyggiygug.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gwfxpriwi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gxpvymblo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gshiykmlf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyaxencc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gjlluwnvm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gfiphaxnc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gxmxnlucp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gbkkxzlqt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkjzmiv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gudecptwg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gjqggkiqh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gcvpnbyge.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gvwfvrpwg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gyxfjkehr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gvzdhadbu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gxhivtpir.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gpmdfleyo.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gctobchvz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/ghsjjbnug.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmzcxqymj.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gavmjlprt.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gakudrkos.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/glkuxgnrj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gelblrcqh.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gcwakhxdq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gjraskuan.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpgurihjr.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gadqqhiuo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gstvtnyme.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gisyihoxn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gqqtsxzsk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gcwyovgcr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gqisiaafi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gulrqwevh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gfmtjdzit.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gxujqneql.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gfbputtqb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghsjuhsis.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gsktwdrdd.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gprgekhpq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gdxypcopn.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ggxqmxlah.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gwurbivmp.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gfmuklowd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gwwjalmop.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/giximexmp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gzxrocmpg.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/glrsandpr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gdrcxbwea.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gfvyezrdg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gcqfcecfg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/guiwtvjqe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gyfvnghxt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gwqheexft.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gjrtysqhv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gmmdloagd.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gntjrnwkx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfaayfgkr.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gvngfzjga.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gimbggdxs.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkasgssyp.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gvyjzhxfs.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gcvpakdtt.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gvqxpxseb.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gurwuhnpf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/guhaemvce.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gascosstq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gyaaoulwe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gblpbxscg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gnvwpqgkd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gedfzpqvv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gaibxinbr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gurjdrsur.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/ghonfhhck.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gfdpcccgi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gnapzzuna.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gsdbzwctw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmyrexlgq.sHtML


<!-- 参考信息 -->