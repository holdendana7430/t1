代发 wailian999

Py:   def add(a, b): return a + b
来源：http://bx.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cq.newstarts.cn

JS:   function add(a, b) { return a + b; }
来源：http://zd.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://si.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hu.521024.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ek.panjiajie.cn

Ruby: def add(a, b); a + b; end
来源：http://zq.szsharing.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ns.shtwfgs.cn

[C02] 默认参数
来源：http://dn.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://cw.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ot.jctech888.com.cn

JS:   function greet(name = "World") { return name; }
来源：http://mz.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ef.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yc.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mc.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://eu.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://ma.shxzskj.cn

[C03] 可变参数
来源：http://sy.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://sa.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hq.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gr.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eq.lnxyls.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rf.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gu.colortex.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ed.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://og.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ft.huixinmuqiang.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ts.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aj.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fc.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pu.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://tb.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://xs.hnjuh.cn

Ruby: f(a: 1, b: 2)
来源：http://eh.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://ht.jctech888.com.cn

[C05] 返回多个值
来源：http://ee.jianghongdianzi.cn

Py:   return a, b
来源：http://sd.gzmigu.cn

PHP:  return [$a, $b];
来源：http://mf.asd995.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://km.newstarts.cn

TS:   return { a, b };
来源：http://xo.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xi.shtwfgs.cn

Go:   return a, b
来源：http://ya.jctech888.com.cn

Ruby: return a, b
来源：http://rl.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://ny.shtwfgs.cn

[C06] 匿名函数 / lambda
来源：http://zo.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://jx.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jz.shxzskj.cn

JS:   const square = x => x * x;
来源：http://ld.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://vo.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uu.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fp.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://of.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zz.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://lb.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://os.szsharing.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tu.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ed.lnxyls.cn

TS:   arr.map(String)
来源：http://ve.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ig.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mf.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://ga.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pv.shxzskj.cn

[C08] 闭包
来源：http://wo.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gx.muxihuayi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ab.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yd.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cu.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kl.yuntaijiaju.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dx.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://as.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vz.huanxung.cn

[C09] 递归
来源：http://so.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mc.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ux.colortex.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oo.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gr.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ya.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kb.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zp.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ep.jctech888.com.cn

[C10] 变量作用域
来源：http://uu.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mj.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://on.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://br.shxzskj.cn

TS:   同 JS
来源：http://wl.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://ka.yuexingan06.cn

Go:   花括号块级作用域
来源：http://tc.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ny.hnjuh.cn

C#:   块级作用域
来源：http://eo.newstarts.cn

[C11] 模块导入与导出
来源：http://ms.huanxung.cn

Py:   from module import func
来源：http://yu.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kw.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qn.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tw.jctech888.com.cn

Java: import java.util.List;
来源：http://ef.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ul.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://qx.haigaiapp.cn

C#:   using System.Text;
来源：http://uu.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://jl.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://kp.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://ik.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://cb.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://mp.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tv.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://ns.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://qv.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vp.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://mn.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hw.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tg.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ke.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fz.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oq.panjiajie.cn

Go:   func add(a, b int) int
来源：http://np.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gx.newstarts.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zm.hnjuh.cn

[C14] 泛型函数
来源：http://da.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qs.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://wt.521024.cn

JS:   // 无泛型
来源：http://dp.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kg.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mu.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fi.huanxung.cn

Ruby: # 无泛型
来源：http://pv.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bx.huanxung.cn

[C15] 解构 / 展开参数
来源：http://pe.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://td.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://ll.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ke.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dt.haigaiapp.cn

Java: // 无解构
来源：http://dv.huanxung.cn

Go:   // 无解构
来源：http://gr.asd995.cn

Ruby: a, b = pair
来源：http://wn.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://pw.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://lh.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nl.muxihuayi.cn

PHP:  // 无重载
来源：http://ci.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dj.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ot.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://df.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://rp.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://zr.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ge.jianghongdianzi.cn

================================================================================
来源：http://vo.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://kn.bjjhwx.cn

================================================================================
来源：http://cn.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://yo.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pw.bookmarksfly.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xu.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qh.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cw.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dk.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://yb.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://zj.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gp.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://ef.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fr.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cf.jctech888.com.cn

JS:   arr.push(4);
来源：http://hb.muxihuayi.cn

TS:   arr.push(4);
来源：http://co.hahajie.cn

Java: list.add(4);
来源：http://en.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://ap.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://wr.huanxung.cn

C#:   list.Add(4);
来源：http://yx.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://xs.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://cs.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lf.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://if.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://kd.9csxet.cn

Java: list.add(0, 0);
来源：http://ab.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sx.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kl.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://tz.huanxung.cn

[D04] 删除元素
来源：http://ch.shxzukj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://em.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dn.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zu.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://dd.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://os.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hl.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qa.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kj.521024.cn

[D05] 访问与修改元素
来源：http://im.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cp.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ub.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gh.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://ht.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://ny.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://tn.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zf.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uz.colortex.cn

[D06] 数组长度
来源：http://mr.gzmigu.cn

Py:   len(arr)
来源：http://sh.yuexingan06.cn

PHP:  count($arr);
来源：http://jn.nszjky.cn

JS:   arr.length
来源：http://qb.szsharing.cn

TS:   arr.length
来源：http://wc.jianghongdianzi.cn

Java: list.size();
来源：http://lp.newstarts.cn

Go:   len(arr)
来源：http://hs.colortex.cn

Ruby: arr.length; arr.size
来源：http://bl.chemitech.net.cn

C#:   list.Count;
来源：http://tv.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://kh.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dr.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xm.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://by.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://yy.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://iv.szsharing.cn

Go:   arr[1:4]
来源：http://iq.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://di.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://kh.lnxyls.cn

[D08] 合并两个数组
来源：http://cc.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://sv.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://uh.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qy.bjjhwx.cn

TS:   [...a, ...b];
来源：http://xm.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wy.gzmigu.cn

Go:   append(a, b...)
来源：http://nb.colortex.cn

Ruby: a + b;  a.concat(b)
来源：http://ba.521024.cn

C#:   a.Concat(b).ToList()
来源：http://ie.nicolike.cn

[D09] 排序（升序）
来源：http://tp.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://kf.shxzskj.cn

PHP:  sort($arr);
来源：http://jt.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gp.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mi.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ux.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rg.szsharing.cn

Ruby: arr.sort
来源：http://th.nszjky.cn

C#:   list.Sort();
来源：http://fv.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ir.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wj.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hd.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yc.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://il.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ga.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rl.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ze.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ya.jianghongdianzi.cn

[D11] 反转数组
来源：http://kg.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yk.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://rh.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ya.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://rt.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://cv.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://it.9csxet.cn

Ruby: arr.reverse
来源：http://oh.hahajie.cn

C#:   list.Reverse();
来源：http://ub.nszjky.cn

[D12] 查找元素下标
来源：http://su.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://ms.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fn.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ei.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gr.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vb.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://et.huixiangedu.cn

Ruby: arr.index(x)
来源：http://kt.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://nr.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://nt.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ff.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sn.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://pu.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://ke.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://to.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jw.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hu.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pp.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://di.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://po.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xl.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://yu.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://jd.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uy.huixinmuqiang.cn

Go:   // 手写循环
来源：http://oa.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gj.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://my.yuexingan06.cn

[D15] 去重
来源：http://jw.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xc.9csxet.cn

PHP:  array_unique($arr);
来源：http://rz.asd995.cn

JS:   [...new Set(arr)]
来源：http://nv.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://xr.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fz.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ej.newstarts.cn

Ruby: arr.uniq
来源：http://py.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://bz.chemitech.net.cn

[D16] 求和与平均值
来源：http://ni.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rd.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mw.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nk.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mg.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://br.lnxyls.cn

Go:   // 手写循环累加
来源：http://ub.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://by.jctech888.com.cn

C#:   list.Sum();  list.Average()
来源：http://qt.wgjwhj.cn

[D17] 最大值与最小值
来源：http://wh.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://lj.haigaiapp.cn

PHP:  max($arr);  min($arr);
来源：http://dl.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ag.gzmigu.cn

TS:   Math.max(...arr);
来源：http://at.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qg.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qf.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://mx.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://mv.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://lj.chemitech.net.cn


<!-- 参考信息 -->