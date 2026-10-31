代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://zz.gzmigu.cn

TS:   [1, 2, 3].includes(x)
来源：http://np.szsharing.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://eh.gzmigu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bv.chemitech.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gd.yuntaijiaju.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nd.hnjuh.cn

[B15] 布尔运算与取反
来源：http://bo.521024.cn

Py:   a and b or not c
来源：http://eh.huixiangedu.cn

PHP:  $a && $b || !$c
来源：http://bo.haigaiapp.cn

JS:   a && b || !c
来源：http://qw.szxytkj.cn

TS:   a && b || !c
来源：http://jz.yuntaijiaju.cn

Java: a && b || !c
来源：http://gs.huixinmuqiang.cn

Go:   a && b || !c
来源：http://yl.szsharing.cn

Ruby: a && b || !c
来源：http://wp.hahajie.cn

C#:   a && b || !c
来源：http://dm.shxzukj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yx.szxytkj.cn

Py:   if not data: return
来源：http://mh.jianghongdianzi.cn

PHP:  if (!$data) { return; }
来源：http://jo.gzmigu.cn

JS:   if (!data) return;
来源：http://hf.newstarts.cn

TS:   if (!data) return;
来源：http://wx.bjjhwx.cn

Java: if (data == null) return;
来源：http://ap.hahajie.cn

Go:   if data == nil { return }
来源：http://xk.chemitech.net.cn

Ruby: return if data.nil?
来源：http://ak.huanxung.cn

C#:   if (data == null) return;
来源：http://rt.asd995.cn

================================================================================
来源：http://lr.9csxet.cn

C. 函数与作用域
来源：http://nu.panjiajie.cn

================================================================================
来源：http://kq.wgjwhj.cn

[C01] 定义函数
来源：http://gv.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://ng.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://qo.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yl.521024.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sm.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ai.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://et.gzmigu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zc.nszjky.cn

[C02] 默认参数
来源：http://xz.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://vs.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://at.huixiangedu.cn

JS:   function greet(name = "World") { return name; }
来源：http://wf.yuntaijiaju.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fc.jianghongdianzi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yz.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://po.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://qu.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://yw.chemitech.net.cn

[C03] 可变参数
来源：http://js.521024.cn

Py:   def total(*args): return sum(args)
来源：http://lt.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xu.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ig.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tj.szsharing.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oq.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rt.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nu.yuexingan06.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sj.yuntaijiaju.cn

[C04] 命名参数 / 关键字参数
来源：http://lq.9csxet.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wg.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wy.chemitech.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wx.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rc.gzmigu.cn

Java: // 无：用 Builder 模式或 record
来源：http://rd.lnxyls.cn

Go:   // 无：用配置结构体参数
来源：http://ib.bookmarksfly.cn

Ruby: f(a: 1, b: 2)
来源：http://jv.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://my.521024.cn

[C05] 返回多个值
来源：http://tr.huixiangedu.cn

Py:   return a, b
来源：http://mn.gzmigu.cn

PHP:  return [$a, $b];
来源：http://ep.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xj.nicolike.cn

TS:   return { a, b };
来源：http://xd.asd995.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://or.hnjuh.cn

Go:   return a, b
来源：http://qt.newstarts.cn

Ruby: return a, b
来源：http://qy.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://cl.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://ye.lnxyls.cn

Py:   square = lambda x: x * x
来源：http://xw.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mz.hnjuh.cn

JS:   const square = x => x * x;
来源：http://vz.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://gn.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://il.521024.cn

Go:   sq := func(x int) int { return x * x }
来源：http://da.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://de.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bk.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://de.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wj.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hs.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qe.nszjky.cn

TS:   arr.map(String)
来源：http://jc.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cg.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hm.hahajie.cn

Ruby: arr.map(&:upcase)
来源：http://de.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mx.hnjuh.cn

[C08] 闭包
来源：http://vl.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iv.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xc.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ky.shxzskj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vx.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fi.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rc.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jh.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xa.nicolike.cn

[C09] 递归
来源：http://bs.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mv.nicolike.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xk.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uw.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gd.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nr.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wy.shxzukj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ny.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tg.hahajie.cn

[C10] 变量作用域
来源：http://no.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://od.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qi.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uq.jianghongdianzi.cn

TS:   同 JS
来源：http://ny.hnjuh.cn

Java: 方法内为块级作用域
来源：http://yh.9csxet.cn

Go:   花括号块级作用域
来源：http://lq.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mr.hahajie.cn

C#:   块级作用域
来源：http://st.bjjhwx.cn

[C11] 模块导入与导出
来源：http://by.shxzukj.cn

Py:   from module import func
来源：http://rl.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ip.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rd.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xb.nszjky.cn

Java: import java.util.List;
来源：http://bd.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://re.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://xl.szxytkj.cn

C#:   using System.Text;
来源：http://ta.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://dp.jianghongdianzi.cn

Py:   (lambda: print("run"))()
来源：http://rd.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://dl.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://fc.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://qu.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pg.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://tf.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://ie.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://db.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://sw.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ao.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nc.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://un.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hf.chemitech.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xm.lnxyls.cn

Go:   func add(a, b int) int
来源：http://fd.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ot.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pd.chemitech.net.cn

[C14] 泛型函数
来源：http://jr.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://np.huanxung.cn

PHP:  // 无泛型
来源：http://lr.shxzukj.cn

JS:   // 无泛型
来源：http://ow.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bp.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jk.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ij.colortex.cn

Ruby: # 无泛型
来源：http://xh.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dh.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://eg.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bp.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://nr.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iq.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qg.nszjky.cn

Java: // 无解构
来源：http://jq.wgjwhj.cn

Go:   // 无解构
来源：http://vi.nszjky.cn

Ruby: a, b = pair
来源：http://fr.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://pc.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://zu.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ri.asd995.cn

PHP:  // 无重载
来源：http://vx.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sf.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://gt.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cu.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://rp.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://ly.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mc.haigaiapp.cn

================================================================================
来源：http://um.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://qi.szxytkj.cn

================================================================================
来源：http://ri.newstarts.cn

[D01] 创建数组 / 列表
来源：http://yt.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hn.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yr.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lu.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ze.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://me.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://kz.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://ir.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://so.gzmigu.cn

[D02] 追加元素到末尾
来源：http://pf.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pj.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wt.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://mc.huanxung.cn

TS:   arr.push(4);
来源：http://oi.shxzskj.cn

Java: list.add(4);
来源：http://wm.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://jx.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://zv.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://vf.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://qn.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://zc.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mj.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mt.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://lz.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ma.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ne.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kh.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://zt.chemitech.net.cn

[D04] 删除元素
来源：http://nc.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iz.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dj.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qm.521024.cn

TS:   arr.splice(0, 1);
来源：http://nj.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://re.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lx.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://li.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://of.wgjwhj.cn

[D05] 访问与修改元素
来源：http://vh.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mb.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hn.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tv.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://zd.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://jn.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://sp.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://th.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yy.szxytkj.cn

[D06] 数组长度
来源：http://qj.hnjuh.cn

Py:   len(arr)
来源：http://ok.wgjwhj.cn

PHP:  count($arr);
来源：http://bp.jctech888.com.cn

JS:   arr.length
来源：http://ks.yuexingan06.cn

TS:   arr.length
来源：http://pq.wgjwhj.cn

Java: list.size();
来源：http://eq.shxzskj.cn

Go:   len(arr)
来源：http://oa.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://ql.panjiajie.cn

C#:   list.Count;
来源：http://vw.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://nw.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hn.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nl.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://za.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://zi.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://ap.szxytkj.cn

Go:   arr[1:4]
来源：http://nt.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://bd.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://mm.yuexingan06.cn

[D08] 合并两个数组
来源：http://mn.521024.cn

Py:   a + b;  a.extend(b)
来源：http://rx.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://yt.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vm.szsharing.cn

TS:   [...a, ...b];
来源：http://rs.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xl.szxytkj.cn

Go:   append(a, b...)
来源：http://ox.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://yi.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://bm.hahajie.cn

[D09] 排序（升序）
来源：http://qo.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://tw.hnjuh.cn

PHP:  sort($arr);
来源：http://tf.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rb.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hj.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ar.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dp.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ta.jianghongdianzi.cn

C#:   list.Sort();
来源：http://uc.wgjwhj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ht.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oo.huanxung.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uh.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://au.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kw.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dc.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://to.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kp.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nq.shxzskj.cn

[D11] 反转数组
来源：http://bi.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vd.huanxung.cn

PHP:  array_reverse($arr);
来源：http://ec.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://an.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ru.asd995.cn

Java: Collections.reverse(list);
来源：http://sq.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://wd.shtwfgs.cn

Ruby: arr.reverse
来源：http://bl.hahajie.cn

C#:   list.Reverse();
来源：http://ap.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://bx.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://fh.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ij.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qu.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bx.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lq.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://yz.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://fb.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://xr.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://uf.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tk.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://il.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://qj.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://yi.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ne.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mu.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wu.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tw.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://rh.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wr.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ca.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://py.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://je.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rj.521024.cn

Go:   // 手写循环
来源：http://om.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jo.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nj.yuntaijiaju.cn


<!-- 参考信息 -->