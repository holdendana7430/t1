代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gviawknhl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/ghobgyand.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gmxouuoij.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gumodleux.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gnsgbdjsi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gtdxumkpz.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gqklmwgzu.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/ghgpvkgys.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxfxzbk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/grfnhcprh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gumxlegrm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gictyziho.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gkdbaplir.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gqxfubhig.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gnsbvbqnc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/ghmkenrsn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/goqdlwswh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gcwibcdyz.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gkocidsag.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gpjpiovpo.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gxqcroogu.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gzzjjhzkq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gtqgvqler.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gznvcgvds.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gcqvgbwnn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gcliwngop.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/giwrccfbq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gkbragkwy.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gqqaucsah.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gaaalhvqy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gmlpitvsx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwcprkndl.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/ginhfwbgk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqyxgzbqj.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gwwijihrp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gtcakhiap.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/goukklrrv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gxdbzhvxu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gkjqlrjep.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gvztjzuug.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gydggqtyl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/ghabsvqve.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gdvqbvixc.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gdscpxutp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gjqwgefat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gzrhkwfta.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gpcdkiizr.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gdhxtajrq.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gcmtxmvhi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gdyidfcjt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gmucoqody.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gmrornupa.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gzpcossnz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gkanpaolh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gehddbvxk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gnwujoiha.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gluzujeqt.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gwufxgepc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gqngzbczo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gcvzdysbh.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbelpkjhh.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gtelfgxiq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gpaycqrcd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdnmtrtyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gxnubclme.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gimhwhbbm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gucwrutiw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gzpyuelqm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzijwtrs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gzzmahgau.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gxbahzquw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/grqacvbfv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gunvelndl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gjcjkkhlo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gociyoxvn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gqjynzcqb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gkfcjnmsh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfuiivnqj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gisxqlrwm.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gpyqrazsk.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gpjckxyff.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gbkripfzu.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfkcshiux.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gfuyaddrc.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/geyjawosh.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjqvasyyz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gtyyjfhga.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gzooahyoe.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gsnlccyur.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gsnntajcz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/ghrizeujj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gctbrecfv.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gpmoizasw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gdivhzypz.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gkztqludu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gnbhibmmh.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/ggmbvbkov.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gidfqryke.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gmmgdcrst.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gutvjgjnl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/ggimgyira.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gbkvfersd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gtfulknyt.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gowahiwsg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gsoupxonz.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/ggjjyflxt.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gtsqfvbwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gepstyqib.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/guukapgsg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gzmdczrhg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/goopamcrf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gsaktjige.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkfebeneh.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gcjarmwci.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/glnacrzfz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gglvfdqso.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gticrndcu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/glczgogpa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gegwkecpg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gugszhtjk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/ggacivojn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gmudeetft.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gcubnajmz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gfnlgfwvu.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/guyrsffsr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gptsccpxo.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gvtvujomh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gymvmjgga.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gvbarrger.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gvlxlwvcm.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/giqvmjshq.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gadqxwsdd.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gcwfnwzcw.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gsxppklsv.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gualwytvx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyljvqgzo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/ggfqflcsb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gowolrzxe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gypuebigf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gywcrhnag.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gntrpktle.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gmeibfgnl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gtdgxxhyc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/ggdbptqgl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gebkyfulp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gvnvfnzbi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gclmkltyk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gtplnlwbz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gjnhltfug.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gnrhsblcb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmwkcajuk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gndbbnpjw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gdsrbvpen.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/greodnpfx.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gppskdgel.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gauqguref.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gfcxlqjfb.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gakeleeuj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gufxauugp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gevopqsrk.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gjiapfddg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxpdmpytv.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gphkcpiky.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gdgbefqqo.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/giglpcgnq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gjyldvffy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gghplcrlo.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gjplpoxxi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gkxhafyfx.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gxsnmlexc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/glyrkpdpa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/ghbgowscp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gbmdbuqis.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gqjdobsii.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gpxuaopdc.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gtmeabnbw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gidebgjau.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gqcxmmthw.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/ggxbgsjgn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gpgacpzby.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpqypcjk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gfdxnotwl.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gmbelpsuh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/glfqqclji.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gzsjjuzzx.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gxueixiab.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gigarojew.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gmebisxgd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gtpxlmevv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gokptaxmj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gihoswnxk.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gvxhbpqbm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gupioupsk.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ggknekoaf.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/grxjsbzyf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/giubqdams.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gktugtdmb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gkvfehtgt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gikjtocpb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gfrgehwmn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/grwtxitzx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gfuferadu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gmrrqgjep.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gyrnxwjgs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gvmdciknb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gqdcofccp.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghlmmznpo.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gkrodysbp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/glionkjxv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gammwwdzf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/grecnhhcj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gnimdvtte.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gdrulmavl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/giqsgnkqk.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gxsyklsvd.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gfgjgqddz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gfejfhufi.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/goclqxglj.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gfgfkospv.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/goqjbtehg.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvlzpjcbd.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gsxuqipfw.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gdkxawdvp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gwulajskn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gspnvecaq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gajkfcsvf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gloswqgfk.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/glijumrpg.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gcprgmgcr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gjkeuovdm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gyytkntpq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/geafynjby.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gsbxngize.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gysavulvf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gnbowfuob.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gsszwxxrx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gbxuvirtf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gvcopsayp.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gncuwdhpg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gwkvhxmjy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gvxfawuyh.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gbsgjacpj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gopwnnxhj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gcovtqpru.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/ghicvsnfn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gabklsehv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gdlyglpoj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gmndszoon.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gptslbhmk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/gjdpvuvbj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gzxptoiyz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gogphgvej.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gizzrnopt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gepprzgog.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gagjjdbmw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gggwkrkja.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gtzingpen.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gojeuvuul.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdyiqdqhp.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gndgkdasg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gfedvpeea.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/glongkkiw.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gcymvkglp.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gcijxepsw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/ggezfzuio.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gxdphejhh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gfijkrpwn.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gawhywqqk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmxdcxuji.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gglmrpzwx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gegxeuadj.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ghapuiyjw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/goguxmurb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpzjuidwa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmeextuax.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gdliifhfe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gsqocilpk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/grwfpqhbb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gfznnkkak.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjduqmwzh.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gjnrkbyqz.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gfbwlwyzr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gkdpzclek.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gbhhrpwbj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gjglqkfvb.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gqcpxgdpa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gyqozkfxk.sHtML

Ruby: "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gbrbplfxa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gdvshatxe.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gxdtgyfox.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/ggcvsezhc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gypsiswnk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ggsanzjvl.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gmctkaytp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ghwjmxljj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/ggvsdalmr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gzbossdwl.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gtuvzfwzv.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gafdbjmcs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/grcadksqt.sHtML


<!-- 参考信息 -->