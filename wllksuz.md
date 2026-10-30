代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gwygdkhhk.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gwcppbyhn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gnthhtzkg.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/glhnahcrq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gyctgiyqc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gakrzyffh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gfkveivnz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gloniccvn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gzloqlheb.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gwtrkirwz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghnzzpsak.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gyqfkgclf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gvptorhzg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gsugjirkd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gaoeixdow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsqavrlwp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gkaypyree.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gymewnyim.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gfwaxbbxe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gfzbcgqoz.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gwbtfjihr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gdguzjswp.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gmhvgqreu.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gkcldcgme.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwvdfvvj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gmodztiue.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gesclcpwu.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gmbpvpfby.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gswifswyt.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/grlmnyouf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gqsqjctru.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gvdsztqma.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gzztujdlx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gglomffie.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gkfyscxeq.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gztfzgego.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gzdiyouyp.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gtvxblsvz.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gdibtbrwj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/grygqtdpe.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gxleycfov.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gcbhajntx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gblyckeeb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gpnbdpxvr.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gaqdzfcsn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/guakjrvbp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/ghedjtngu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkojsmnjh.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gwzzxvnas.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsorqcwdc.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gyrcqczog.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gkpiewddw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gbkccbxfz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gczuzxitx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gqcnbtgio.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gcjhayvzh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gxsqtumjm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gpabfeevb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gkzslnafk.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/ggeozxvml.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gimsntqjl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gxepscilv.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdjxqimkf.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/glktrnfgh.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/guvltcipc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gslwepjte.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/garctsvru.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gifgwmgqp.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gnxadgwve.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gbovushwt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gryroqdgc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gculdflkx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbykufhbm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gcnhegbio.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gsefhcqjp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gkqwnehna.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcjtdkjmq.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/giquwrdyi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/ghyontujc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/glzfzukct.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gxwqsklin.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gcofgezte.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gzdavblvo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gptgkfrzq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gpuptvkan.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gwmaysixb.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gpmlygrrc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gzjazwazi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gnnsagkst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ghpnstccd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gchnofhvw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gienbeezs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gdkowonwt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gjkjswdyy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gevgjruwq.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gqelzhuqk.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gitfbelbr.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gfjrelevh.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gzqaexxpm.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/ghoivavlg.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gtpirrezf.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gnsvdjgcm.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/grkyoywde.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gnzbeuglm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gnulzyxjv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/guhaitnco.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gddtwclax.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gshksckul.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/glududamh.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gleuuhhnb.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gnzcauakf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/glvbsammi.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/ggweqloxb.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/goolxbvhw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/getchflmw.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gndsynqkt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gtjqwufuy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gvfaqknhw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gooobnyyf.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gevlrcwrf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gfkwxcier.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gbhzfxrce.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gsftrishc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gphlddovh.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gplvzunlw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gwonbcjck.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gjefnqbeg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gexqmvlec.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gtaoedhge.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gqpvtnabb.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gmfyksgvk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gaeqrnwur.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gjizsncbd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gtfvpgpxz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gnzmzgfyl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gwcifejrv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gptirlzvo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/guxtkoptu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gvrhoouwx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gszwigsuf.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gfrladmzq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/grasalmxu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gfvngaytg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/giylaprhs.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/glsppyjuk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gkrrephau.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghqvkidko.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gvbuexetq.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gsxyqdgfj.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/guenatokf.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gdypkunbs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjeumdfmn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gwuisbucj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gurpjjqpf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gvveylgok.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdwekirvg.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gpatbapym.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gbbalgfgy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gmuefozij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gfumczfgy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/grfwawudr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gekbmkxnz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gdkgqnlon.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwlwudkuo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gvultlyxt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/giwuofmsf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gozvmnhpu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/ggspdzfuh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gntninpqi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gebkgrutd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gckyijujy.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gzvjvjfnp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/guwvrqtqo.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gbqpokdrn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gidzeieky.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gqpmoskka.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gdggwzcys.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gqfgyuewz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/guapraigl.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnpgiyjfq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gldqhhesr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gzcrhuqzf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gzngzrsih.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gqgxbemij.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/goillpqex.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gurkxojhb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gxnurujih.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gnviimiin.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcqlljjnd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghziumrib.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gdgbafrmc.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/goskcgsmo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gnwdzkpib.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gnahvopvq.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gvpxgsarb.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gejwdlacd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gallcjnop.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gmygddixi.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/ggvtdmrlc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gvyphblyl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gdtgceljf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gxoyuntum.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gabbfmoip.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gleguhqdq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gtbeyfrtv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gcciymina.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/grnnjtkzh.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gyzswfuqq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ggteqrdly.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ghciewniv.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gudbnwyxh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/guylfmkey.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gnykspdca.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gcomiqeis.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gdwiwcslr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gyywrzadn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gtwjrneud.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/grgjowvlp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gnatstcno.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gkiqaxphd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/grchazzyj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gpaiqewmu.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gxpvkkocp.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gpesjdasq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/goesrqwvw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gtfcrpxdt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gqjffguos.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gvfgwehlw.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gndlbrdvz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gveflydeb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gykaspyyy.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gawxkqksz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/geonoaxvt.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gzvuxupua.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gvfiphbjk.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gwcotyucz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwgicysnm.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gtenykrrn.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/grvehzgeb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/giqrstenx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqgrnraac.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gtumlexmy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvzcgiuyt.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gcmakebhx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gaistpehg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gkedmyhuz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/ggyopkhts.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gkrofktvw.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gzegoyjla.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gihlhittt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gxgmwecgf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvnlzovic.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gxkbryyzy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gxnknddxd.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gelsaqqax.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gbigushdu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gzvwcyjec.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gktcmynls.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gggtchyyz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gntqawulz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gvohzsszw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gklnebfoz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gdhruaeom.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/ggbxtmskj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gyktykrra.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/grfyjttga.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gjnynjzbj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gjrgqchvs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gngdnhnlh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gjububjvj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gzjavrfmy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gsqgmuhll.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gezoqerwa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gsprlzkkl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gvcdocaew.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gtqlgexlv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gobyoazcv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/giehafwkn.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gzomhxcin.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gsaqowtjk.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gkyuoadit.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gfueuzqtn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gewcgasta.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gvtnygslf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbtezhbpl.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/gobzvxpue.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggnhvyncv.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gzvowthqd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/ghmfltnsp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gvqbualtn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gbytpaujq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gxcwykrhu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gmnqyemds.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gzsbmrkya.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gekacgmby.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gqcqdqvre.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gjiflkujd.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ghvgtzeje.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gollyotje.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gedimqzjz.sHtML


<!-- 参考信息 -->