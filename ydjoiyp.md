代发 wailian999

Java: if (data == null) return;
来源：http://ll.521024.cn

Go:   if data == nil { return }
来源：http://mr.huixinmuqiang.cn

Ruby: return if data.nil?
来源：http://ix.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://uc.szxytkj.cn

================================================================================
来源：http://tj.jianghongdianzi.cn

C. 函数与作用域
来源：http://vo.nszjky.cn

================================================================================
来源：http://qv.shtwfgs.cn

[C01] 定义函数
来源：http://ov.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://xo.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wy.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://uv.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xu.shtwfgs.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sd.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cl.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://od.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ua.nicolike.cn

[C02] 默认参数
来源：http://rl.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://ot.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qp.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://wh.szxytkj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uq.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yr.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kf.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://sk.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://xn.jianghongdianzi.cn

[C03] 可变参数
来源：http://hj.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://mk.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vl.jianghongdianzi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fq.chemitech.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ka.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://us.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mn.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ur.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tl.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://zt.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ez.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hm.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zo.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oq.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://fu.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://ik.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://mb.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://ap.colortex.cn

[C05] 返回多个值
来源：http://uo.bjjhwx.cn

Py:   return a, b
来源：http://pj.panjiajie.cn

PHP:  return [$a, $b];
来源：http://wf.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wm.hnjuh.cn

TS:   return { a, b };
来源：http://vx.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sj.bjjhwx.cn

Go:   return a, b
来源：http://ii.panjiajie.cn

Ruby: return a, b
来源：http://dr.panjiajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://zq.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://tp.newstarts.cn

Py:   square = lambda x: x * x
来源：http://ej.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://by.huanxung.cn

JS:   const square = x => x * x;
来源：http://kt.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://zp.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pd.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://us.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://za.nszjky.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ns.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://vn.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wf.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gr.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cl.shxzskj.cn

TS:   arr.map(String)
来源：http://em.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ty.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ik.szsharing.cn

Ruby: arr.map(&:upcase)
来源：http://jk.haigaiapp.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jz.hnjuh.cn

[C08] 闭包
来源：http://wi.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wf.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mp.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hq.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pq.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cm.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tc.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cr.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nt.nicolike.cn

[C09] 递归
来源：http://xa.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eh.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ze.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ih.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zt.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wu.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xj.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lk.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fg.hnjuh.cn

[C10] 变量作用域
来源：http://ai.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nl.shxzukj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jk.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gp.nicolike.cn

TS:   同 JS
来源：http://rg.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://om.gzmigu.cn

Go:   花括号块级作用域
来源：http://wt.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bf.521024.cn

C#:   块级作用域
来源：http://ii.haigaiapp.cn

[C11] 模块导入与导出
来源：http://xg.asd995.cn

Py:   from module import func
来源：http://zs.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rh.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://te.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sr.huanxung.cn

Java: import java.util.List;
来源：http://sm.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oq.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ua.shxzukj.cn

C#:   using System.Text;
来源：http://xp.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://jv.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://kb.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://sr.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://qy.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://mj.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ap.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://ih.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://zy.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fz.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://wa.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dy.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xj.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aj.shxzukj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://np.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://yt.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://it.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oj.shxzukj.cn

[C14] 泛型函数
来源：http://dh.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ld.asd995.cn

PHP:  // 无泛型
来源：http://pd.shtwfgs.cn

JS:   // 无泛型
来源：http://cz.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iy.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qv.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fa.hnjuh.cn

Ruby: # 无泛型
来源：http://xx.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aq.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://og.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xg.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://vf.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fp.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mv.bjjhwx.cn

Java: // 无解构
来源：http://pj.szsharing.cn

Go:   // 无解构
来源：http://ou.shtwfgs.cn

Ruby: a, b = pair
来源：http://te.yuexingan06.cn

C#:   var (a, b) = pair;
来源：http://mq.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://gi.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yo.panjiajie.cn

PHP:  // 无重载
来源：http://rm.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://da.nicolike.cn

TS:   // 用联合类型或重载签名声明
来源：http://ix.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rr.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://ln.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://md.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ce.shxzukj.cn

================================================================================
来源：http://pp.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://go.haigaiapp.cn

================================================================================
来源：http://id.colortex.cn

[D01] 创建数组 / 列表
来源：http://el.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ya.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vg.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qx.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yj.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kw.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://dp.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://oj.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fx.hnjuh.cn

[D02] 追加元素到末尾
来源：http://sx.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rd.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jz.jctech888.com.cn

JS:   arr.push(4);
来源：http://bw.9csxet.cn

TS:   arr.push(4);
来源：http://yp.colortex.cn

Java: list.add(4);
来源：http://kt.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://om.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://pm.hahajie.cn

C#:   list.Add(4);
来源：http://wr.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://eg.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://yp.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lj.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kk.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://on.colortex.cn

Java: list.add(0, 0);
来源：http://kf.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kr.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://af.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://yp.chemitech.net.cn

[D04] 删除元素
来源：http://of.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tb.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hw.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://be.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://vz.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hf.shxzskj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://je.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sy.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yx.yuexingan06.cn

[D05] 访问与修改元素
来源：http://vb.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pc.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yw.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mb.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://jl.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://dl.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://pg.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tp.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fh.muxihuayi.cn

[D06] 数组长度
来源：http://yn.hahajie.cn

Py:   len(arr)
来源：http://zv.bjjhwx.cn

PHP:  count($arr);
来源：http://kx.lnxyls.cn

JS:   arr.length
来源：http://tx.lnxyls.cn

TS:   arr.length
来源：http://bo.jianghongdianzi.cn

Java: list.size();
来源：http://rq.lnxyls.cn

Go:   len(arr)
来源：http://yu.szsharing.cn

Ruby: arr.length; arr.size
来源：http://ez.huanxung.cn

C#:   list.Count;
来源：http://rk.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://uw.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sz.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dd.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://me.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://if.9csxet.cn

Java: list.subList(1, 4);
来源：http://gq.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://ea.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://ez.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://bx.bookmarksfly.cn

[D08] 合并两个数组
来源：http://fp.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://jw.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://pu.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vr.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ic.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://df.9csxet.cn

Go:   append(a, b...)
来源：http://nr.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://fo.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://ne.yuexingan06.cn

[D09] 排序（升序）
来源：http://ab.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://hn.szsharing.cn

PHP:  sort($arr);
来源：http://wu.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qp.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cm.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cp.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bm.9csxet.cn

Ruby: arr.sort
来源：http://hu.huixinmuqiang.cn

C#:   list.Sort();
来源：http://rj.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://px.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eh.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nv.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gv.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jd.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xy.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cr.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ae.szxytkj.cn

[D11] 反转数组
来源：http://wp.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jz.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://dh.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pa.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://he.lnxyls.cn

Java: Collections.reverse(list);
来源：http://rf.chemitech.net.cn

Go:   slices.Reverse(arr)
来源：http://zq.hnjuh.cn

Ruby: arr.reverse
来源：http://uq.panjiajie.cn

C#:   list.Reverse();
来源：http://vq.shtwfgs.cn

[D12] 查找元素下标
来源：http://qt.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://em.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ns.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zf.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mg.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://er.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://bm.hnjuh.cn

Ruby: arr.index(x)
来源：http://fr.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://xr.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://vs.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iw.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cx.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://mc.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://wn.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xk.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bx.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://le.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ui.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://un.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jp.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gq.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://xa.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://ve.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vs.lnxyls.cn

Go:   // 手写循环
来源：http://aw.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pc.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vb.yuntaijiaju.cn

[D15] 去重
来源：http://rj.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nx.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://zb.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://er.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://cg.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gb.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dp.lnxyls.cn

Ruby: arr.uniq
来源：http://fv.colortex.cn

C#:   list.Distinct().ToList()
来源：http://le.shtwfgs.cn

[D16] 求和与平均值
来源：http://hm.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nr.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uy.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kd.panjiajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ad.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zr.haigaiapp.cn

Go:   // 手写循环累加
来源：http://aq.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qg.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://iw.shxzukj.cn

[D17] 最大值与最小值
来源：http://rh.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://zh.szsharing.cn


<!-- 参考信息 -->