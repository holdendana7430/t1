代发 wailian999

Py:   def add(a, b): return a + b
来源：http://bo.nszjky.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zc.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://gw.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ie.9csxet.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kw.bjjhwx.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ef.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://jg.hnjuh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dg.lnxyls.cn

[C02] 默认参数
来源：http://cc.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://rg.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mb.hnjuh.cn

JS:   function greet(name = "World") { return name; }
来源：http://vh.szsharing.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pa.colortex.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://km.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hs.yuntaijiaju.cn

Ruby: def greet(name = "World") = name
来源：http://gx.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://wl.szsharing.cn

[C03] 可变参数
来源：http://kg.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://sq.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://if.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gv.hahajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wx.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ip.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sn.hnjuh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ng.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://et.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://dq.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eu.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wk.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fm.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lz.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ws.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://ke.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://mq.newstarts.cn

C#:   f(a: 1, b: 2)
来源：http://op.shxzskj.cn

[C05] 返回多个值
来源：http://ki.asd995.cn

Py:   return a, b
来源：http://cb.szxytkj.cn

PHP:  return [$a, $b];
来源：http://pb.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yy.yuntaijiaju.cn

TS:   return { a, b };
来源：http://nd.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dn.shxzskj.cn

Go:   return a, b
来源：http://mw.colortex.cn

Ruby: return a, b
来源：http://jy.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://pp.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://fd.9csxet.cn

Py:   square = lambda x: x * x
来源：http://wo.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zb.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://aj.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://yf.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ey.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bv.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://qk.521024.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fe.huanxung.cn

[C07] 把函数作为参数传入
来源：http://ei.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rw.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wa.yuntaijiaju.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gr.panjiajie.cn

TS:   arr.map(String)
来源：http://ks.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zj.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dj.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://hv.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://dp.bjjhwx.cn

[C08] 闭包
来源：http://vo.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rj.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vu.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vx.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tm.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lg.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ae.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://du.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qv.jctech888.com.cn

[C09] 递归
来源：http://qu.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pt.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yv.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bk.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fy.colortex.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://au.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://po.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bu.hahajie.cn

[C10] 变量作用域
来源：http://pf.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yh.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yb.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bo.huixinmuqiang.cn

TS:   同 JS
来源：http://ue.huanxung.cn

Java: 方法内为块级作用域
来源：http://aa.nszjky.cn

Go:   花括号块级作用域
来源：http://yq.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tj.bjjhwx.cn

C#:   块级作用域
来源：http://tq.hahajie.cn

[C11] 模块导入与导出
来源：http://jl.shxzskj.cn

Py:   from module import func
来源：http://gl.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://eu.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uv.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ku.muxihuayi.cn

Java: import java.util.List;
来源：http://wl.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://we.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://fh.hnjuh.cn

C#:   using System.Text;
来源：http://vd.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://om.haigaiapp.cn

Py:   (lambda: print("run"))()
来源：http://vm.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://sn.huanxung.cn

JS:   (() => { console.log("run"); })();
来源：http://uk.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://sd.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qt.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://hr.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://kj.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iz.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://hz.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oj.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uu.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://su.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ai.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mc.colortex.cn

Go:   func add(a, b int) int
来源：http://gs.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vc.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qt.chemitech.net.cn

[C14] 泛型函数
来源：http://li.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vw.hnjuh.cn

PHP:  // 无泛型
来源：http://uo.yuntaijiaju.cn

JS:   // 无泛型
来源：http://sr.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rc.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sm.huixinmuqiang.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fd.gzmigu.cn

Ruby: # 无泛型
来源：http://nw.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jc.lnxyls.cn

[C15] 解构 / 展开参数
来源：http://kw.szxytkj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dy.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://jh.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://be.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://us.colortex.cn

Java: // 无解构
来源：http://ck.bookmarksfly.cn

Go:   // 无解构
来源：http://mn.wgjwhj.cn

Ruby: a, b = pair
来源：http://oq.huanxung.cn

C#:   var (a, b) = pair;
来源：http://sr.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://ui.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wj.shxzskj.cn

PHP:  // 无重载
来源：http://ic.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wc.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ct.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hs.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://ih.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://xo.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ib.shtwfgs.cn

================================================================================
来源：http://ll.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://bu.jianghongdianzi.cn

================================================================================
来源：http://mh.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://ap.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ft.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wn.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://az.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ia.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ul.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://bp.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://ut.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lk.nicolike.cn

[D02] 追加元素到末尾
来源：http://ub.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://at.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hq.shxzukj.cn

JS:   arr.push(4);
来源：http://go.newstarts.cn

TS:   arr.push(4);
来源：http://oy.shxzskj.cn

Java: list.add(4);
来源：http://op.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://bm.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://hg.szsharing.cn

C#:   list.Add(4);
来源：http://qe.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://wh.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://mj.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kh.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eh.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://hj.szxytkj.cn

Java: list.add(0, 0);
来源：http://lj.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zu.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jf.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://xw.hnjuh.cn

[D04] 删除元素
来源：http://gy.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yg.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sa.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ug.colortex.cn

TS:   arr.splice(0, 1);
来源：http://se.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bm.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://js.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nd.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ix.szxytkj.cn

[D05] 访问与修改元素
来源：http://nu.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pf.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://my.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eg.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://yg.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://lq.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://tl.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ok.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lq.nicolike.cn

[D06] 数组长度
来源：http://dd.muxihuayi.cn

Py:   len(arr)
来源：http://sn.nszjky.cn

PHP:  count($arr);
来源：http://sm.shxzukj.cn

JS:   arr.length
来源：http://nz.muxihuayi.cn

TS:   arr.length
来源：http://rn.wgjwhj.cn

Java: list.size();
来源：http://cp.muxihuayi.cn

Go:   len(arr)
来源：http://id.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://bj.huixiangedu.cn

C#:   list.Count;
来源：http://bj.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://pn.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bl.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sw.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://no.yuexingan06.cn

TS:   arr.slice(1, 4);
来源：http://ql.panjiajie.cn

Java: list.subList(1, 4);
来源：http://bk.bjjhwx.cn

Go:   arr[1:4]
来源：http://la.huanxung.cn

Ruby: arr[1, 3]
来源：http://ly.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://pe.haigaiapp.cn

[D08] 合并两个数组
来源：http://ay.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://jd.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://xp.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bo.9csxet.cn

TS:   [...a, ...b];
来源：http://ll.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gk.hnjuh.cn

Go:   append(a, b...)
来源：http://zk.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://xo.521024.cn

C#:   a.Concat(b).ToList()
来源：http://fh.9csxet.cn

[D09] 排序（升序）
来源：http://zv.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://si.chemitech.net.cn

PHP:  sort($arr);
来源：http://et.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ar.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fl.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://au.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sl.shxzskj.cn

Ruby: arr.sort
来源：http://vh.colortex.cn

C#:   list.Sort();
来源：http://rl.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://er.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ty.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uq.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xt.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ip.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jn.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gp.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ry.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qh.hnjuh.cn

[D11] 反转数组
来源：http://ke.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ik.newstarts.cn

PHP:  array_reverse($arr);
来源：http://xb.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zr.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ak.hahajie.cn

Java: Collections.reverse(list);
来源：http://ec.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://xh.chemitech.net.cn

Ruby: arr.reverse
来源：http://dc.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://xj.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://pk.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://cy.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tf.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vd.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lc.hnjuh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ed.asd995.cn

Go:   slices.Index(arr, x)
来源：http://to.yuexingan06.cn

Ruby: arr.index(x)
来源：http://ic.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://fm.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://ys.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zk.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ld.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://gk.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://dz.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rg.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://se.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wv.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ql.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://rm.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pg.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oz.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://hg.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://dj.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ge.haigaiapp.cn

Go:   // 手写循环
来源：http://mr.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gg.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lt.asd995.cn

[D15] 去重
来源：http://sr.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uz.shxzukj.cn

PHP:  array_unique($arr);
来源：http://gi.521024.cn

JS:   [...new Set(arr)]
来源：http://ip.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://vt.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tr.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ib.jctech888.com.cn

Ruby: arr.uniq
来源：http://zj.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://mx.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://av.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ae.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wo.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jb.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tq.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kz.newstarts.cn

Go:   // 手写循环累加
来源：http://cm.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lj.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://jp.shxzskj.cn

[D17] 最大值与最小值
来源：http://yb.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://kn.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://rc.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fh.shxzskj.cn

TS:   Math.max(...arr);
来源：http://ny.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gj.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lk.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://ve.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://se.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://hf.jctech888.com.cn


<!-- 参考信息 -->