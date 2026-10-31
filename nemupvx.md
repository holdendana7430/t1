代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://vs.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yo.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fo.wgjwhj.cn

Ruby: def greet(name = "World") = name
来源：http://zr.yuntaijiaju.cn

C#:   string Greet(string name = "World") => name;
来源：http://sl.huixinmuqiang.cn

[C03] 可变参数
来源：http://rm.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://xz.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yt.lnxyls.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ug.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ap.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rt.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oo.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://cc.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ma.newstarts.cn

[C04] 命名参数 / 关键字参数
来源：http://pb.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gm.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tc.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rt.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://en.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://cc.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://rd.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://xr.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://mr.jctech888.com.cn

[C05] 返回多个值
来源：http://fn.shxzskj.cn

Py:   return a, b
来源：http://qt.hahajie.cn

PHP:  return [$a, $b];
来源：http://we.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oi.szsharing.cn

TS:   return { a, b };
来源：http://ix.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gr.asd995.cn

Go:   return a, b
来源：http://eu.9csxet.cn

Ruby: return a, b
来源：http://qc.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://oo.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://wz.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://wu.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ok.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://zd.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://om.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://px.shxzukj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wt.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://ng.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gc.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://bc.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kr.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yh.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xv.9csxet.cn

TS:   arr.map(String)
来源：http://io.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ln.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hm.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://oy.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mg.hahajie.cn

[C08] 闭包
来源：http://mh.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mb.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://by.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ht.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uu.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nl.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nt.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jq.lnxyls.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fm.nszjky.cn

[C09] 递归
来源：http://or.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bp.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pf.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bk.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dx.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yo.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tc.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wy.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fc.yuexingan06.cn

[C10] 变量作用域
来源：http://nx.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mv.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ya.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lw.huixiangedu.cn

TS:   同 JS
来源：http://cl.szsharing.cn

Java: 方法内为块级作用域
来源：http://fm.szsharing.cn

Go:   花括号块级作用域
来源：http://il.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://om.huixinmuqiang.cn

C#:   块级作用域
来源：http://jf.szsharing.cn

[C11] 模块导入与导出
来源：http://yq.colortex.cn

Py:   from module import func
来源：http://cc.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pf.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eu.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hd.gzmigu.cn

Java: import java.util.List;
来源：http://st.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hb.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://nv.yuexingan06.cn

C#:   using System.Text;
来源：http://gn.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://io.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://mo.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://oa.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://xd.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://lb.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ie.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://cz.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://nz.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://it.nszjky.cn

[C13] 类型声明 / 类型注解
来源：http://mm.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jc.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nh.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dm.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dy.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fb.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://oy.colortex.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tt.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kr.hahajie.cn

[C14] 泛型函数
来源：http://dh.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://km.9csxet.cn

PHP:  // 无泛型
来源：http://zd.hahajie.cn

JS:   // 无泛型
来源：http://on.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xk.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://me.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tu.chemitech.net.cn

Ruby: # 无泛型
来源：http://bh.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ph.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://du.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gw.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://xl.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tf.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ux.shtwfgs.cn

Java: // 无解构
来源：http://zd.lnxyls.cn

Go:   // 无解构
来源：http://yw.asd995.cn

Ruby: a, b = pair
来源：http://pd.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://zx.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://oj.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ay.yuntaijiaju.cn

PHP:  // 无重载
来源：http://oq.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uy.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://ay.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wy.jianghongdianzi.cn

Go:   // 无重载：用不同函数名
来源：http://bi.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://ob.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yi.haigaiapp.cn

================================================================================
来源：http://ur.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://ll.9csxet.cn

================================================================================
来源：http://vc.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://ki.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sd.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gv.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gj.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fa.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jl.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://fv.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://uy.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oc.shxzukj.cn

[D02] 追加元素到末尾
来源：http://bz.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yj.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yo.szsharing.cn

JS:   arr.push(4);
来源：http://vm.wgjwhj.cn

TS:   arr.push(4);
来源：http://iq.yuexingan06.cn

Java: list.add(4);
来源：http://kg.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://ht.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://ma.jctech888.com.cn

C#:   list.Add(4);
来源：http://ip.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://gd.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://yw.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gd.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zw.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://yl.colortex.cn

Java: list.add(0, 0);
来源：http://nd.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yb.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://md.asd995.cn

C#:   list.Insert(0, 0);
来源：http://xj.gzmigu.cn

[D04] 删除元素
来源：http://cy.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zb.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rm.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jl.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://ev.jianghongdianzi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oz.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kf.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jc.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qq.muxihuayi.cn

[D05] 访问与修改元素
来源：http://om.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mw.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qs.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://go.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://mp.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://fz.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://sd.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tx.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://id.shtwfgs.cn

[D06] 数组长度
来源：http://ny.bjjhwx.cn

Py:   len(arr)
来源：http://mm.yuexingan06.cn

PHP:  count($arr);
来源：http://yd.9csxet.cn

JS:   arr.length
来源：http://sz.shtwfgs.cn

TS:   arr.length
来源：http://ub.colortex.cn

Java: list.size();
来源：http://ne.shxzskj.cn

Go:   len(arr)
来源：http://kh.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://pa.521024.cn

C#:   list.Count;
来源：http://ch.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://ea.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ts.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wi.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://cf.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://as.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://pf.nicolike.cn

Go:   arr[1:4]
来源：http://sb.gzmigu.cn

Ruby: arr[1, 3]
来源：http://qe.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://fe.hahajie.cn

[D08] 合并两个数组
来源：http://wo.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://eo.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://vk.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mk.szxytkj.cn

TS:   [...a, ...b];
来源：http://dd.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mf.newstarts.cn

Go:   append(a, b...)
来源：http://ik.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://gn.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://na.9csxet.cn

[D09] 排序（升序）
来源：http://sd.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://rh.9csxet.cn

PHP:  sort($arr);
来源：http://rn.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bx.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ml.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jt.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://va.wgjwhj.cn

Ruby: arr.sort
来源：http://uk.jianghongdianzi.cn

C#:   list.Sort();
来源：http://xf.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oy.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://po.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yc.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rl.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ly.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ji.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zx.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nb.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jb.colortex.cn

[D11] 反转数组
来源：http://pr.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yz.szsharing.cn

PHP:  array_reverse($arr);
来源：http://dd.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kd.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ab.newstarts.cn

Java: Collections.reverse(list);
来源：http://xn.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://wt.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ms.bjjhwx.cn

C#:   list.Reverse();
来源：http://xd.shxzukj.cn

[D12] 查找元素下标
来源：http://xo.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://sf.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ql.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://li.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lr.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dz.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://pb.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://wp.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://tf.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://wn.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sa.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qm.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://cn.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://qu.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://et.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vt.shxzukj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ba.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sm.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://bc.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oa.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ud.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://sj.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://hv.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zq.jctech888.com.cn

Go:   // 手写循环
来源：http://to.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ud.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://df.muxihuayi.cn

[D15] 去重
来源：http://uj.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pi.hnjuh.cn

PHP:  array_unique($arr);
来源：http://gu.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://cr.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://dw.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ks.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cl.shtwfgs.cn

Ruby: arr.uniq
来源：http://ym.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://mt.yuexingan06.cn

[D16] 求和与平均值
来源：http://yv.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nu.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cx.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://re.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gx.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nz.asd995.cn

Go:   // 手写循环累加
来源：http://uk.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://cd.bjjhwx.cn

[D17] 最大值与最小值
来源：http://rx.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://yu.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://dh.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eo.huanxung.cn

TS:   Math.max(...arr);
来源：http://lu.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gz.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pt.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://wb.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://lo.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://hl.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xn.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://lk.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ty.muxihuayi.cn

TS:   nested.flat();
来源：http://sl.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ar.shxzukj.cn

Go:   // 手写双层循环
来源：http://qn.521024.cn

Ruby: nested.flatten
来源：http://rm.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ro.gzmigu.cn

[D19] 按字段分组
来源：http://su.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ju.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dd.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gg.colortex.cn


<!-- 参考信息 -->