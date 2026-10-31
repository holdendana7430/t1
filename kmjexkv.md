代发 wailian999

================================================================================
来源：http://wn.muxihuayi.cn

C. 函数与作用域
来源：http://yt.jctech888.com.cn

================================================================================
来源：http://gx.9csxet.cn

[C01] 定义函数
来源：http://uo.wgjwhj.cn

Py:   def add(a, b): return a + b
来源：http://fg.hahajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dg.9csxet.cn

JS:   function add(a, b) { return a + b; }
来源：http://wz.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mv.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sg.gzmigu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rt.colortex.cn

Ruby: def add(a, b); a + b; end
来源：http://if.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bk.nicolike.cn

[C02] 默认参数
来源：http://gv.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://bl.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ty.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://gs.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vg.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://on.wgjwhj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jp.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://ei.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://ae.huixiangedu.cn

[C03] 可变参数
来源：http://fp.521024.cn

Py:   def total(*args): return sum(args)
来源：http://sz.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dv.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nb.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wq.huanxung.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aj.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tu.nszjky.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yu.chemitech.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jr.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://je.huixiangedu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://km.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tr.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ya.bjjhwx.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xx.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://qu.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://gl.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://qt.jianghongdianzi.cn

C#:   f(a: 1, b: 2)
来源：http://xz.9csxet.cn

[C05] 返回多个值
来源：http://jq.gzmigu.cn

Py:   return a, b
来源：http://bd.shxzukj.cn

PHP:  return [$a, $b];
来源：http://uy.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pu.nicolike.cn

TS:   return { a, b };
来源：http://ap.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qz.gzmigu.cn

Go:   return a, b
来源：http://kf.shxzukj.cn

Ruby: return a, b
来源：http://dh.lnxyls.cn

C#:   return (a, b);              // ValueTuple
来源：http://gu.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://cy.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://im.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lf.panjiajie.cn

JS:   const square = x => x * x;
来源：http://ut.huanxung.cn

TS:   const square = (x: number): number => x * x;
来源：http://qu.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nd.lnxyls.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bp.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://jm.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mn.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://ku.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://af.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ks.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vh.hnjuh.cn

TS:   arr.map(String)
来源：http://jg.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yg.wgjwhj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xe.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://yr.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wa.nicolike.cn

[C08] 闭包
来源：http://qr.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://te.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://re.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://op.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zh.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ic.chemitech.net.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qp.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://km.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ox.shtwfgs.cn

[C09] 递归
来源：http://bb.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://la.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iv.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dw.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rj.szxytkj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wp.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ja.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ug.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://de.newstarts.cn

[C10] 变量作用域
来源：http://bp.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jf.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rv.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pk.lnxyls.cn

TS:   同 JS
来源：http://ta.panjiajie.cn

Java: 方法内为块级作用域
来源：http://he.gzmigu.cn

Go:   花括号块级作用域
来源：http://ax.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lc.yuexingan06.cn

C#:   块级作用域
来源：http://gg.huixiangedu.cn

[C11] 模块导入与导出
来源：http://lp.haigaiapp.cn

Py:   from module import func
来源：http://ej.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qa.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fk.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://al.huixinmuqiang.cn

Java: import java.util.List;
来源：http://dc.hahajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uv.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://hx.yuexingan06.cn

C#:   using System.Text;
来源：http://ir.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://ae.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://di.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://le.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://kn.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://ef.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rf.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://ql.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://jx.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ug.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://za.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://km.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vc.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rk.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tf.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cl.huanxung.cn

Go:   func add(a, b int) int
来源：http://nq.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://of.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xc.yuntaijiaju.cn

[C14] 泛型函数
来源：http://ey.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gh.yuexingan06.cn

PHP:  // 无泛型
来源：http://um.gzmigu.cn

JS:   // 无泛型
来源：http://zp.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ws.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ih.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vv.nicolike.cn

Ruby: # 无泛型
来源：http://tb.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oa.szsharing.cn

[C15] 解构 / 展开参数
来源：http://dm.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fv.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://qf.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hk.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fz.hahajie.cn

Java: // 无解构
来源：http://kk.nszjky.cn

Go:   // 无解构
来源：http://av.szxytkj.cn

Ruby: a, b = pair
来源：http://hf.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://uk.newstarts.cn

[C16] 函数 / 方法重载
来源：http://jf.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dk.lnxyls.cn

PHP:  // 无重载
来源：http://ng.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yn.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://db.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qw.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://br.shxzskj.cn

Ruby: # 无重载：靠动态参数
来源：http://kh.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ym.asd995.cn

================================================================================
来源：http://ru.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://fm.szsharing.cn

================================================================================
来源：http://jz.nicolike.cn

[D01] 创建数组 / 列表
来源：http://se.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://iq.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nw.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lc.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://km.szsharing.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gl.chemitech.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://nm.colortex.cn

Ruby: arr = [1, 2, 3]
来源：http://il.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://im.panjiajie.cn

[D02] 追加元素到末尾
来源：http://ir.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ao.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bt.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://mo.colortex.cn

TS:   arr.push(4);
来源：http://io.9csxet.cn

Java: list.add(4);
来源：http://bi.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://mh.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://fa.hahajie.cn

C#:   list.Add(4);
来源：http://ur.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://ag.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://rl.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mg.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://if.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://si.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://cz.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lb.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mx.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://jn.nicolike.cn

[D04] 删除元素
来源：http://lb.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ex.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tc.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://of.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://ah.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://el.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zq.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://td.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shxzskj.cn

[D05] 访问与修改元素
来源：http://zy.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hb.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jb.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://it.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ud.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://hp.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://kk.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dc.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qd.colortex.cn

[D06] 数组长度
来源：http://su.szxytkj.cn

Py:   len(arr)
来源：http://jj.panjiajie.cn

PHP:  count($arr);
来源：http://hh.hahajie.cn

JS:   arr.length
来源：http://qu.gzmigu.cn

TS:   arr.length
来源：http://wy.muxihuayi.cn

Java: list.size();
来源：http://er.wgjwhj.cn

Go:   len(arr)
来源：http://ev.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://hk.bookmarksfly.cn

C#:   list.Count;
来源：http://bw.hahajie.cn

[D07] 切片 / 取子数组
来源：http://cg.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pw.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://we.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://rv.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://fu.newstarts.cn

Java: list.subList(1, 4);
来源：http://nc.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://gx.521024.cn

Ruby: arr[1, 3]
来源：http://cy.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://es.huixiangedu.cn

[D08] 合并两个数组
来源：http://mg.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://fx.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://ej.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wy.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://rx.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ti.colortex.cn

Go:   append(a, b...)
来源：http://cy.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://qw.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://hp.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://di.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://mz.bookmarksfly.cn

PHP:  sort($arr);
来源：http://gb.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cd.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nd.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bd.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lb.nicolike.cn

Ruby: arr.sort
来源：http://zq.haigaiapp.cn

C#:   list.Sort();
来源：http://iy.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jb.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ty.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zs.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ut.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tu.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rq.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qy.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pc.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ii.gzmigu.cn

[D11] 反转数组
来源：http://dq.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xo.huanxung.cn

PHP:  array_reverse($arr);
来源：http://iw.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dh.521024.cn

TS:   [...arr].reverse();
来源：http://dc.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://bf.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://kw.bookmarksfly.cn

Ruby: arr.reverse
来源：http://qq.asd995.cn

C#:   list.Reverse();
来源：http://ko.huixiangedu.cn

[D12] 查找元素下标
来源：http://iz.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://rz.newstarts.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ih.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vx.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://an.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ub.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://lk.colortex.cn

Ruby: arr.index(x)
来源：http://jw.asd995.cn

C#:   list.IndexOf(x);
来源：http://if.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://jp.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lu.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pj.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://qd.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://st.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kz.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gc.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ze.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cq.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://qv.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ok.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ov.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://od.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://ft.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qr.jctech888.com.cn

Go:   // 手写循环
来源：http://xy.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mr.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lz.nszjky.cn

[D15] 去重
来源：http://tn.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cp.nszjky.cn

PHP:  array_unique($arr);
来源：http://bl.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://mp.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://nc.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yc.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vx.nszjky.cn

Ruby: arr.uniq
来源：http://rr.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://cj.wgjwhj.cn

[D16] 求和与平均值
来源：http://ly.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ow.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jy.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vw.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://um.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bx.shtwfgs.cn

Go:   // 手写循环累加
来源：http://ye.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ce.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://vb.hnjuh.cn

[D17] 最大值与最小值
来源：http://ig.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://ac.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://df.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hw.colortex.cn

TS:   Math.max(...arr);
来源：http://si.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ov.shtwfgs.cn


<!-- 参考信息 -->