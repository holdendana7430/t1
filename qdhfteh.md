代发 wailian999

Py:   if not data: return
来源：http://uo.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://qz.haigaiapp.cn

JS:   if (!data) return;
来源：http://tj.jianghongdianzi.cn

TS:   if (!data) return;
来源：http://qi.nszjky.cn

Java: if (data == null) return;
来源：http://qx.9csxet.cn

Go:   if data == nil { return }
来源：http://xm.shxzukj.cn

Ruby: return if data.nil?
来源：http://mw.newstarts.cn

C#:   if (data == null) return;
来源：http://rx.muxihuayi.cn

================================================================================
来源：http://nn.wgjwhj.cn

C. 函数与作用域
来源：http://gd.szxytkj.cn

================================================================================
来源：http://np.jctech888.com.cn

[C01] 定义函数
来源：http://rs.shtwfgs.cn

Py:   def add(a, b): return a + b
来源：http://tr.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ua.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://vd.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fz.newstarts.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gb.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bl.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://bl.jianghongdianzi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://un.huixinmuqiang.cn

[C02] 默认参数
来源：http://jd.jctech888.com.cn

Py:   def greet(name="World"): return name
来源：http://ye.chemitech.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rm.haigaiapp.cn

JS:   function greet(name = "World") { return name; }
来源：http://ix.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kf.gzmigu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zu.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qg.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://ij.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://zl.gzmigu.cn

[C03] 可变参数
来源：http://rs.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://je.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yf.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sv.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rq.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ij.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dl.huanxung.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pl.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ih.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://nm.bookmarksfly.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cp.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ti.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yi.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jz.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://eu.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://hc.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://pi.haigaiapp.cn

C#:   f(a: 1, b: 2)
来源：http://cj.bjjhwx.cn

[C05] 返回多个值
来源：http://md.huixiangedu.cn

Py:   return a, b
来源：http://zm.huanxung.cn

PHP:  return [$a, $b];
来源：http://wg.lnxyls.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pw.hahajie.cn

TS:   return { a, b };
来源：http://en.huixinmuqiang.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lv.szxytkj.cn

Go:   return a, b
来源：http://dh.nicolike.cn

Ruby: return a, b
来源：http://db.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://fn.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://wy.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://fg.gzmigu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iv.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://rg.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://xb.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zh.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ml.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://jr.bookmarksfly.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jv.colortex.cn

[C07] 把函数作为参数传入
来源：http://mv.shxzskj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gd.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cz.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://en.haigaiapp.cn

TS:   arr.map(String)
来源：http://rr.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jx.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gw.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://hu.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uf.jctech888.com.cn

[C08] 闭包
来源：http://ls.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://th.hnjuh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xx.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yv.bjjhwx.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zq.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zc.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fj.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ox.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ou.asd995.cn

[C09] 递归
来源：http://ml.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wn.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yi.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ag.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zp.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uy.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fv.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cb.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hh.asd995.cn

[C10] 变量作用域
来源：http://gy.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mw.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ew.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gq.szxytkj.cn

TS:   同 JS
来源：http://yy.colortex.cn

Java: 方法内为块级作用域
来源：http://dc.newstarts.cn

Go:   花括号块级作用域
来源：http://dd.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jt.bjjhwx.cn

C#:   块级作用域
来源：http://us.hnjuh.cn

[C11] 模块导入与导出
来源：http://yc.gzmigu.cn

Py:   from module import func
来源：http://co.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zk.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iw.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://us.huixiangedu.cn

Java: import java.util.List;
来源：http://hh.szxytkj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vm.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://qq.szsharing.cn

C#:   using System.Text;
来源：http://ox.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://wj.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://yc.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://gu.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://qx.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://bc.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zn.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://lz.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://pl.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://me.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://kt.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fj.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jp.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://go.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cp.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zf.9csxet.cn

Go:   func add(a, b int) int
来源：http://pp.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yx.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gw.jianghongdianzi.cn

[C14] 泛型函数
来源：http://hn.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qo.shxzukj.cn

PHP:  // 无泛型
来源：http://zc.panjiajie.cn

JS:   // 无泛型
来源：http://ll.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qg.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hl.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ue.nicolike.cn

Ruby: # 无泛型
来源：http://fz.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ds.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://ys.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dk.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://dv.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vz.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tq.gzmigu.cn

Java: // 无解构
来源：http://jk.nszjky.cn

Go:   // 无解构
来源：http://vf.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://ef.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://rp.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://hp.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mb.szsharing.cn

PHP:  // 无重载
来源：http://pe.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lx.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://zd.chemitech.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uv.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://ip.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://av.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pw.szsharing.cn

================================================================================
来源：http://il.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://aq.jctech888.com.cn

================================================================================
来源：http://ww.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://yk.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rv.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ng.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sb.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://py.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ka.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://jh.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://po.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://md.newstarts.cn

[D02] 追加元素到末尾
来源：http://hf.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://na.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wk.nszjky.cn

JS:   arr.push(4);
来源：http://te.chemitech.net.cn

TS:   arr.push(4);
来源：http://du.chemitech.net.cn

Java: list.add(4);
来源：http://uv.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://du.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://oz.haigaiapp.cn

C#:   list.Add(4);
来源：http://cj.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://wy.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://eb.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hd.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fs.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ri.huanxung.cn

Java: list.add(0, 0);
来源：http://ns.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nl.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ey.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://df.newstarts.cn

[D04] 删除元素
来源：http://ma.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qk.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fj.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uv.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://kp.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mn.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fx.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://en.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://es.szxytkj.cn

[D05] 访问与修改元素
来源：http://dl.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nm.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hg.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iy.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://qz.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://mz.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://bs.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hf.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ip.shxzskj.cn

[D06] 数组长度
来源：http://ly.huixinmuqiang.cn

Py:   len(arr)
来源：http://do.huanxung.cn

PHP:  count($arr);
来源：http://to.lnxyls.cn

JS:   arr.length
来源：http://rn.521024.cn

TS:   arr.length
来源：http://dw.wgjwhj.cn

Java: list.size();
来源：http://yj.haigaiapp.cn

Go:   len(arr)
来源：http://bl.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://gb.chemitech.net.cn

C#:   list.Count;
来源：http://ql.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://xf.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rc.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://or.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://db.asd995.cn

TS:   arr.slice(1, 4);
来源：http://fk.lnxyls.cn

Java: list.subList(1, 4);
来源：http://gs.haigaiapp.cn

Go:   arr[1:4]
来源：http://mw.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://if.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://mr.nszjky.cn

[D08] 合并两个数组
来源：http://uo.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://zb.asd995.cn

PHP:  array_merge($a, $b);
来源：http://dv.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wd.9csxet.cn

TS:   [...a, ...b];
来源：http://wh.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xb.shxzskj.cn

Go:   append(a, b...)
来源：http://bq.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://oe.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://pl.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://en.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://vn.bjjhwx.cn

PHP:  sort($arr);
来源：http://lz.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ai.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zb.huanxung.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sd.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jw.shtwfgs.cn

Ruby: arr.sort
来源：http://cz.huixiangedu.cn

C#:   list.Sort();
来源：http://gu.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ld.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tc.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ih.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nz.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yx.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zg.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ss.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ei.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gd.jctech888.com.cn

[D11] 反转数组
来源：http://ud.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qq.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://iv.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://in.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://ip.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://dn.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://ql.muxihuayi.cn

Ruby: arr.reverse
来源：http://be.chemitech.net.cn

C#:   list.Reverse();
来源：http://ql.yuexingan06.cn

[D12] 查找元素下标
来源：http://fz.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://eu.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zz.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sv.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ef.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ab.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://yl.shxzskj.cn

Ruby: arr.index(x)
来源：http://pn.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://io.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://sv.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://km.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fz.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://dd.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://qq.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tp.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mu.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ck.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ay.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://kn.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fh.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ym.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://pc.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://sx.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ie.nicolike.cn

Go:   // 手写循环
来源：http://qg.hnjuh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jk.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://by.yuexingan06.cn

[D15] 去重
来源：http://vy.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://es.asd995.cn

PHP:  array_unique($arr);
来源：http://yg.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://hn.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ln.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://td.colortex.cn

Go:   // 用 map[T]struct{} 手写
来源：http://py.panjiajie.cn

Ruby: arr.uniq
来源：http://cv.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://is.jctech888.com.cn

[D16] 求和与平均值
来源：http://pg.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yx.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pa.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rc.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vy.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pa.muxihuayi.cn

Go:   // 手写循环累加
来源：http://yu.huixiangedu.cn


<!-- 参考信息 -->