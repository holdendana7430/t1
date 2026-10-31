代发 wailian999

Py:   def add(a, b): return a + b
来源：http://da.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wp.nszjky.cn

JS:   function add(a, b) { return a + b; }
来源：http://gz.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ej.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ea.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vn.yuexingan06.cn

Ruby: def add(a, b); a + b; end
来源：http://xg.nicolike.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ij.yuntaijiaju.cn

[C02] 默认参数
来源：http://tp.gzmigu.cn

Py:   def greet(name="World"): return name
来源：http://di.nszjky.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vz.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://tv.shxzukj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ry.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ck.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://to.lnxyls.cn

Ruby: def greet(name = "World") = name
来源：http://gh.nicolike.cn

C#:   string Greet(string name = "World") => name;
来源：http://sz.haigaiapp.cn

[C03] 可变参数
来源：http://be.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://sg.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://od.nszjky.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mj.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uc.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wa.yuexingan06.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cb.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gz.bookmarksfly.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cw.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://jw.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lp.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ak.colortex.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kn.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dj.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://ck.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://ql.bjjhwx.cn

Ruby: f(a: 1, b: 2)
来源：http://ro.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://tf.szsharing.cn

[C05] 返回多个值
来源：http://jv.shxzskj.cn

Py:   return a, b
来源：http://kj.nicolike.cn

PHP:  return [$a, $b];
来源：http://mh.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yc.huixiangedu.cn

TS:   return { a, b };
来源：http://nk.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ix.hnjuh.cn

Go:   return a, b
来源：http://eq.521024.cn

Ruby: return a, b
来源：http://fa.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://rl.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://xp.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://zp.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vg.hahajie.cn

JS:   const square = x => x * x;
来源：http://at.panjiajie.cn

TS:   const square = (x: number): number => x * x;
来源：http://sq.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ua.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dp.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://xg.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bu.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://hx.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qq.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://fy.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yy.gzmigu.cn

TS:   arr.map(String)
来源：http://xb.huixiangedu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ju.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jl.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://ke.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hp.colortex.cn

[C08] 闭包
来源：http://wn.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://of.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rg.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yp.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://im.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gv.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ek.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tq.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yt.szsharing.cn

[C09] 递归
来源：http://iq.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ek.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dc.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jh.bjjhwx.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mi.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gv.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mj.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hx.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eb.shxzskj.cn

[C10] 变量作用域
来源：http://zu.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gn.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mw.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ch.szxytkj.cn

TS:   同 JS
来源：http://ze.asd995.cn

Java: 方法内为块级作用域
来源：http://ef.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://im.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lt.colortex.cn

C#:   块级作用域
来源：http://ac.huixiangedu.cn

[C11] 模块导入与导出
来源：http://ph.muxihuayi.cn

Py:   from module import func
来源：http://sd.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zq.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mr.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://da.yuexingan06.cn

Java: import java.util.List;
来源：http://vf.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ma.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://am.shxzskj.cn

C#:   using System.Text;
来源：http://tw.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://xc.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ki.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://rq.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://by.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://ui.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rv.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://me.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://gv.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pg.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://zc.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pc.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://su.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://er.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rh.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qv.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://qn.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dv.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mu.gzmigu.cn

[C14] 泛型函数
来源：http://ok.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oe.chemitech.net.cn

PHP:  // 无泛型
来源：http://oh.huanxung.cn

JS:   // 无泛型
来源：http://gx.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pq.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://he.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nw.huanxung.cn

Ruby: # 无泛型
来源：http://ok.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gz.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://ke.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fe.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://vw.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ar.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oq.shtwfgs.cn

Java: // 无解构
来源：http://gj.chemitech.net.cn

Go:   // 无解构
来源：http://dy.wgjwhj.cn

Ruby: a, b = pair
来源：http://ob.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://av.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://hb.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rs.shxzskj.cn

PHP:  // 无重载
来源：http://lf.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dr.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://qc.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xa.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://kl.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://rz.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xp.shxzukj.cn

================================================================================
来源：http://df.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://yd.szxytkj.cn

================================================================================
来源：http://mm.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://bb.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yw.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wp.wgjwhj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ku.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://io.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wd.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://bs.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://gx.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oj.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://np.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ld.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rp.hnjuh.cn

JS:   arr.push(4);
来源：http://lp.chemitech.net.cn

TS:   arr.push(4);
来源：http://vo.shxzskj.cn

Java: list.add(4);
来源：http://ek.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://jo.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://dp.asd995.cn

C#:   list.Add(4);
来源：http://uu.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://zl.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://hs.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cd.hnjuh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sg.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ww.nicolike.cn

Java: list.add(0, 0);
来源：http://uh.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yb.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pa.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ve.yuntaijiaju.cn

[D04] 删除元素
来源：http://ug.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hg.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dc.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yi.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://hg.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vo.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ty.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pn.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vt.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://rg.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uh.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ce.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yk.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://tv.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://fb.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ap.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ei.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qm.chemitech.net.cn

[D06] 数组长度
来源：http://wv.szsharing.cn

Py:   len(arr)
来源：http://yu.521024.cn

PHP:  count($arr);
来源：http://lc.yuexingan06.cn

JS:   arr.length
来源：http://mf.haigaiapp.cn

TS:   arr.length
来源：http://ty.yuexingan06.cn

Java: list.size();
来源：http://jd.shtwfgs.cn

Go:   len(arr)
来源：http://wa.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://jl.colortex.cn

C#:   list.Count;
来源：http://hr.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://io.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wk.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://du.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://jv.asd995.cn

TS:   arr.slice(1, 4);
来源：http://yv.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://xa.haigaiapp.cn

Go:   arr[1:4]
来源：http://ds.szxytkj.cn

Ruby: arr[1, 3]
来源：http://ve.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://zv.shxzskj.cn

[D08] 合并两个数组
来源：http://rz.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://oh.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://zs.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sv.hahajie.cn

TS:   [...a, ...b];
来源：http://lj.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wo.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://rs.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://nz.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://ls.haigaiapp.cn

[D09] 排序（升序）
来源：http://ao.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rm.panjiajie.cn

PHP:  sort($arr);
来源：http://qp.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dj.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://og.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yc.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yr.nszjky.cn

Ruby: arr.sort
来源：http://zn.huixiangedu.cn

C#:   list.Sort();
来源：http://lm.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hc.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cl.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://io.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ez.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cw.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://da.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zk.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yk.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ys.szxytkj.cn

[D11] 反转数组
来源：http://dk.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bp.newstarts.cn

PHP:  array_reverse($arr);
来源：http://hi.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bm.panjiajie.cn

TS:   [...arr].reverse();
来源：http://vo.9csxet.cn

Java: Collections.reverse(list);
来源：http://xv.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://mq.nszjky.cn

Ruby: arr.reverse
来源：http://uh.huanxung.cn

C#:   list.Reverse();
来源：http://dy.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://cd.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://ba.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ip.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eq.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cy.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fv.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://aq.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://jb.huanxung.cn

C#:   list.IndexOf(x);
来源：http://bs.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://lk.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rp.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ff.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://op.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://vi.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xt.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ij.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://if.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bk.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://ep.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xr.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kv.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://dx.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://wn.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xa.nszjky.cn

Go:   // 手写循环
来源：http://ej.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ii.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dk.nszjky.cn

[D15] 去重
来源：http://xf.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ce.nicolike.cn

PHP:  array_unique($arr);
来源：http://bs.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://sn.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://mv.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ow.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gu.wgjwhj.cn

Ruby: arr.uniq
来源：http://cn.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://kh.yuexingan06.cn

[D16] 求和与平均值
来源：http://nm.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vm.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cj.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://np.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oa.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rh.colortex.cn

Go:   // 手写循环累加
来源：http://wo.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rz.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://bd.haigaiapp.cn

[D17] 最大值与最小值
来源：http://vk.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://tw.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://xh.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nv.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://cs.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xx.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ou.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://qn.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://yk.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://fn.haigaiapp.cn


<!-- 参考信息 -->