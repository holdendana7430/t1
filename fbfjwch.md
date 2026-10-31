代发 wailian999

Java: if (data == null) return;
来源：http://ci.szsharing.cn

Go:   if data == nil { return }
来源：http://za.hnjuh.cn

Ruby: return if data.nil?
来源：http://sc.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://lu.nszjky.cn

================================================================================
来源：http://uz.521024.cn

C. 函数与作用域
来源：http://vx.9csxet.cn

================================================================================
来源：http://my.yuntaijiaju.cn

[C01] 定义函数
来源：http://yr.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://dk.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vy.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://uo.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ug.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://yc.jctech888.com.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bi.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://oi.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xa.nicolike.cn

[C02] 默认参数
来源：http://jo.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://uk.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lc.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://nb.chemitech.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rs.huixiangedu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vr.hahajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ya.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://bl.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://pm.huixiangedu.cn

[C03] 可变参数
来源：http://ks.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://pa.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wf.yuexingan06.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qn.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nh.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wc.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fx.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://et.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://om.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://ah.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gd.9csxet.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jk.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dp.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://co.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://jw.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://ie.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://fc.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://jm.9csxet.cn

[C05] 返回多个值
来源：http://hv.yuexingan06.cn

Py:   return a, b
来源：http://sn.nicolike.cn

PHP:  return [$a, $b];
来源：http://vo.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xk.huanxung.cn

TS:   return { a, b };
来源：http://xb.huanxung.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ys.nicolike.cn

Go:   return a, b
来源：http://rv.colortex.cn

Ruby: return a, b
来源：http://rb.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://eq.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://gb.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://fb.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hd.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://mn.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://fw.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rh.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lv.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://ze.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dw.nszjky.cn

[C07] 把函数作为参数传入
来源：http://dt.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uv.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lp.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xh.szsharing.cn

TS:   arr.map(String)
来源：http://vw.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yz.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xt.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://ri.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://si.shtwfgs.cn

[C08] 闭包
来源：http://ze.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://av.shtwfgs.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gf.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jh.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lf.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://co.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hf.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pf.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bl.haigaiapp.cn

[C09] 递归
来源：http://wb.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ko.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ua.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ju.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tx.nszjky.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qx.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yq.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tl.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lw.haigaiapp.cn

[C10] 变量作用域
来源：http://yy.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vr.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nk.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ef.chemitech.net.cn

TS:   同 JS
来源：http://oe.shxzskj.cn

Java: 方法内为块级作用域
来源：http://uu.haigaiapp.cn

Go:   花括号块级作用域
来源：http://fq.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ep.bjjhwx.cn

C#:   块级作用域
来源：http://cj.521024.cn

[C11] 模块导入与导出
来源：http://yh.yuntaijiaju.cn

Py:   from module import func
来源：http://ln.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://my.shxzukj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nr.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kg.muxihuayi.cn

Java: import java.util.List;
来源：http://lc.huixiangedu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rr.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://hx.jianghongdianzi.cn

C#:   using System.Text;
来源：http://mq.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://ef.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://ur.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://yf.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://di.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://vu.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ty.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://tw.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://dx.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cx.yuntaijiaju.cn

[C13] 类型声明 / 类型注解
来源：http://ny.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kt.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://as.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yk.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zl.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gm.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://qx.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rw.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wl.bjjhwx.cn

[C14] 泛型函数
来源：http://du.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fk.nszjky.cn

PHP:  // 无泛型
来源：http://mz.shxzskj.cn

JS:   // 无泛型
来源：http://vw.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qz.bjjhwx.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kl.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gl.newstarts.cn

Ruby: # 无泛型
来源：http://xp.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qe.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://uy.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oq.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://vk.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aq.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ed.nszjky.cn

Java: // 无解构
来源：http://sd.huanxung.cn

Go:   // 无解构
来源：http://up.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://mw.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://pn.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ug.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bg.haigaiapp.cn

PHP:  // 无重载
来源：http://bx.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wj.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://uv.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ln.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://mw.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://py.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://et.szsharing.cn

================================================================================
来源：http://eq.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://uy.gzmigu.cn

================================================================================
来源：http://lf.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://br.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://em.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yz.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://is.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sc.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ly.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://fk.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://ux.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hu.shxzukj.cn

[D02] 追加元素到末尾
来源：http://mj.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pq.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hv.nszjky.cn

JS:   arr.push(4);
来源：http://ou.bookmarksfly.cn

TS:   arr.push(4);
来源：http://yk.chemitech.net.cn

Java: list.add(4);
来源：http://rs.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://je.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://yp.colortex.cn

C#:   list.Add(4);
来源：http://ma.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://jm.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://xq.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vy.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dt.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://ba.jctech888.com.cn

Java: list.add(0, 0);
来源：http://sd.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qk.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pg.asd995.cn

C#:   list.Insert(0, 0);
来源：http://cq.szxytkj.cn

[D04] 删除元素
来源：http://pm.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kf.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ic.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vx.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://hn.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rg.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kl.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://is.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qk.hahajie.cn

[D05] 访问与修改元素
来源：http://uf.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://za.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yt.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dz.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://vw.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://zg.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ga.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jo.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://td.huanxung.cn

[D06] 数组长度
来源：http://zi.nszjky.cn

Py:   len(arr)
来源：http://cn.521024.cn

PHP:  count($arr);
来源：http://yp.shxzskj.cn

JS:   arr.length
来源：http://mp.huixinmuqiang.cn

TS:   arr.length
来源：http://lv.colortex.cn

Java: list.size();
来源：http://rw.shxzukj.cn

Go:   len(arr)
来源：http://rg.colortex.cn

Ruby: arr.length; arr.size
来源：http://ky.nszjky.cn

C#:   list.Count;
来源：http://no.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://nt.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://km.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hk.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://oz.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://hd.hahajie.cn

Java: list.subList(1, 4);
来源：http://uj.hnjuh.cn

Go:   arr[1:4]
来源：http://gv.asd995.cn

Ruby: arr[1, 3]
来源：http://ww.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://fj.wgjwhj.cn

[D08] 合并两个数组
来源：http://oe.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://bl.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://hk.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cr.gzmigu.cn

TS:   [...a, ...b];
来源：http://tu.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nt.hnjuh.cn

Go:   append(a, b...)
来源：http://ht.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://lw.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://fs.colortex.cn

[D09] 排序（升序）
来源：http://dp.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://dg.hnjuh.cn

PHP:  sort($arr);
来源：http://bf.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xr.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://or.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://op.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jb.wgjwhj.cn

Ruby: arr.sort
来源：http://xn.jianghongdianzi.cn

C#:   list.Sort();
来源：http://bw.nszjky.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lh.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://th.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dr.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yw.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ey.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ae.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bn.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sz.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ak.wgjwhj.cn

[D11] 反转数组
来源：http://iv.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zn.asd995.cn

PHP:  array_reverse($arr);
来源：http://sy.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ou.hahajie.cn

TS:   [...arr].reverse();
来源：http://qa.asd995.cn

Java: Collections.reverse(list);
来源：http://kj.shxzukj.cn

Go:   slices.Reverse(arr)
来源：http://gm.shxzskj.cn

Ruby: arr.reverse
来源：http://nx.bookmarksfly.cn

C#:   list.Reverse();
来源：http://rt.wgjwhj.cn

[D12] 查找元素下标
来源：http://ie.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://re.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uj.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qa.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://za.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hj.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://ue.shxzukj.cn

Ruby: arr.index(x)
来源：http://bb.nicolike.cn

C#:   list.IndexOf(x);
来源：http://bw.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://ya.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://io.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ir.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://gi.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://se.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://so.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zh.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gd.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iv.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://yj.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nh.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cg.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://kr.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://ks.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://go.wgjwhj.cn

Go:   // 手写循环
来源：http://sv.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ct.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hy.bookmarksfly.cn

[D15] 去重
来源：http://kd.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nj.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://vf.asd995.cn

JS:   [...new Set(arr)]
来源：http://zn.szsharing.cn

TS:   [...new Set(arr)]
来源：http://jw.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wq.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ka.lnxyls.cn

Ruby: arr.uniq
来源：http://ib.bookmarksfly.cn

C#:   list.Distinct().ToList()
来源：http://mf.bookmarksfly.cn

[D16] 求和与平均值
来源：http://bv.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sg.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rq.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pq.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qx.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ku.huanxung.cn

Go:   // 手写循环累加
来源：http://kr.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://js.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://lh.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://je.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ph.jianghongdianzi.cn


<!-- 参考信息 -->