代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/guxbkczsd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gubzdhdlp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gjzlugvsm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gdzgpbatb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gelrznesq.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/guveluxhg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gwsnjzgkc.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gsdeuucsh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/glvmxcyvp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/godsueiwe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/grhzaecub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvrzcxscl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gnbmisnmg.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/ggwxkpucv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gtivnoxuf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/guvwqcadk.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gifmjgfol.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gfopqqdts.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gwwgutfod.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gprjcuoir.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/ggyjfryey.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gpvmpbahk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gwlsbsgif.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gruehysqx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/grywtljys.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/giakuxdkv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gpiremfpo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gsxqjosgi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gxoojzmqp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkofumvsh.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gshdnxcyy.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ggnzgflrq.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gzsaqpphi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gznmsxkgn.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gaswccvba.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gwozflmgj.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gnokjsrzr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gttwthqai.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gwrriqvwc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gnpefvdbv.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gdwdfkcvf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gxhsezahc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gszqdflry.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grdjdcomb.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gtgrevtkj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvbjpfjni.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gxofnwmgm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gurljgcti.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/goicubhcc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gzadryqvn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gtppvupiw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/glodxeqoq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gqdjrtimy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gllafcdxe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/glubpkimm.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gwjqeizlk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gllytfsyi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gskkfwukd.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gwkdqzrqq.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gvreqwqmi.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gtzrksetr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gomujeipm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gstzwflks.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gilqgoven.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/giybtkywi.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gascwmqil.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gywcpnzbq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gttftkzfh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gexjbrsyy.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpjbqvwnr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gdskerjlz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gnvxlqlfz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gghviydsm.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gzktqxipb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gngfmjlrp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/guctbtppu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/guljaxxpg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gykuzsuws.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gxezoxdwm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gkdxxuraa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gfmfscuwr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gwdyeaayf.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/ganqxmini.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gabrxcqat.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gtkkoqqib.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gqkdnvmlk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gdmuvcvbh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gcikhbkoy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/giyjnbwjb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gfwyyhtnm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gebweaynj.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gasqpjyqt.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gnauvuutr.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gbsnwqfbd.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gqcaboklf.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/glgzgcgym.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/granximei.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/guclwyyrd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gkmauztrl.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gbjhcbtis.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gwohaivdv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gfnzpkpxd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gofyapvpr.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ghohuqrfb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/guklhpqqm.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/ghepxkhkq.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/ghpiqduus.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/guswclqhs.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkcoplgma.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gwrxaihaz.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gwmfugbgv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gwivtppfj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gyxlfetgx.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gvztqhqzm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gejimnaey.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gicgjhviq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/ghjjpzztn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gctnkjole.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gaddryrsh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/grltvzejn.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gujcqpuej.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gzqixxmsp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gssjdginl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gpsicolbw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gkeqbnhdp.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gyyftnusi.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gjxuxqpgp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gjtflbpsv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/guzgcnlxl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/ggprdpjnm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gdcnlmoyu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gbjmfyhcf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gseqrcyjy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gpzwnnusi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gylamatlf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gmdmyidkr.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/gclogrjfi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/ghpqyvboh.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gevjgkmyn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gzwjewwmz.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gxjuearmf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfhtrqzt.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gvyxrbbmu.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/grcefdsik.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gsltrmqxd.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gxrfyjzyi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/ggobkhffv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gdbxdtvdo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ggwbywtmh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gewnyfujz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gwsxuxukq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzwqjumza.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzdnxoixf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gfameoswg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gdmuekssq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glrchgxyv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfspmsoct.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gtzmjgnlp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gydbwpapz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gthiwypdt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gwcdvfpka.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/geefjsvwe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/ghqjarjmm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gvhgownjk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gfkzjnypg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gqnyzbhkk.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gsaufkzpt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ghutsxifp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gimhmfibo.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/guzvrsppk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gltvbtthp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gojfyfdhx.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gupuquvxc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gkdppsfgt.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gbafpggji.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/giblxpdel.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gawwnydkc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gopsrgaqw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gparcjcdu.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gqssizomg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gfneahpsu.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gmzxehmax.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gdofsjoxz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gmlccwrbs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gtbqzkrxi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gffgxknoz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/guoiyhphf.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gmdmbdytp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gccqihzun.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gkyibzsba.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gxxkmbpdw.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gbxvtvmko.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gycyllyvk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/garmkklpc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gkneylwjy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gpcgyfcan.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gycnqqfpj.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/giztwoeet.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gsxreivkn.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gukntqbgo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/giqkoycig.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gwlpqezme.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gvzascgfn.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gtrjhndzb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gybsguvgs.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gxacvdule.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gltnzilak.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtxtbcouv.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/guzpmpbpj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gczylqxry.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gwhthwmdk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gazszmbzt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gkbyijiux.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gccabidnh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gaiqsqjud.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gdinspdbz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gbwzxhljo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/geraaafoy.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/ghyweubdr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/ggsarytck.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gveqiwoxy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gzdgidnfn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gqvvwbfhw.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gryliohpe.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/geoxdtooj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gbthqyyjc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gfqgmeuty.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/ggzuzvntv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/ghonvzrvo.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gwviqpcvj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gmxgrvofp.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gzxxsdbex.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzogdxnau.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glbsnkoco.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gteowbxsw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/ghhiyxdlb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ghfspxhtn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/ggufcdilw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ghtugxaqc.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gucewlngy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gpipcdyhb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gdalggopl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/geswuotza.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/guhlswjfy.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gssszsods.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gmlavzsca.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gntmvbonx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gykbsxhen.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxmaafcvw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/glyxxyihi.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gjznwwtgc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gibxmwflm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gngaysxlw.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/gnyylicru.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gnifpvysz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gailxyvkd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gxypifefy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/ggkzqmykh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gpmujdtqn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gvkhexsni.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gbfodjulw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gcltygoag.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gbdunuzer.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/ghdjgqfec.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gopygxrok.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gxpbftite.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gjbyhxful.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/giglynlgw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/glcoxaune.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gkcaiiyxx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gjfpjgjam.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/goxpftmhz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghxeadlov.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmjnfoprv.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ghzpmtbld.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/glbikgcbu.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gwwokyfit.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gghrlgqnz.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gxqvkghvi.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/ggckvrfdg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gipmbwiwy.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/ggqgcywxg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyelorizo.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqrzrxxrk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gsrlndczf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gdgebhbqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/ggmprjkjn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gsomzmuvq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gztpqovzl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gjcmrizhb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gxhufskvr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gojhnvpho.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmdcaslje.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gvykmfcmd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gowjmyhhw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gfdntxoss.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gahxmubgy.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnshfdrtw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gehhrhbll.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gkrlrhfmj.sHtML


<!-- 参考信息 -->