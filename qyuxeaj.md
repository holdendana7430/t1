代发 wailian999

Py:   if not data: return
来源：http://ak.yuexingan06.cn

PHP:  if (!$data) { return; }
来源：http://qi.szxytkj.cn

JS:   if (!data) return;
来源：http://hk.9csxet.cn

TS:   if (!data) return;
来源：http://vo.szxytkj.cn

Java: if (data == null) return;
来源：http://xp.hnjuh.cn

Go:   if data == nil { return }
来源：http://wv.newstarts.cn

Ruby: return if data.nil?
来源：http://uw.bjjhwx.cn

C#:   if (data == null) return;
来源：http://wj.shxzskj.cn

================================================================================
来源：http://uw.bjjhwx.cn

C. 函数与作用域
来源：http://hn.colortex.cn

================================================================================
来源：http://wr.haigaiapp.cn

[C01] 定义函数
来源：http://ia.asd995.cn

Py:   def add(a, b): return a + b
来源：http://ld.muxihuayi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lx.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://ao.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gs.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rg.szxytkj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://gu.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://ju.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iz.muxihuayi.cn

[C02] 默认参数
来源：http://qn.shtwfgs.cn

Py:   def greet(name="World"): return name
来源：http://te.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wx.shxzukj.cn

JS:   function greet(name = "World") { return name; }
来源：http://wr.gzmigu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mq.szxytkj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yy.asd995.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ve.huixiangedu.cn

Ruby: def greet(name = "World") = name
来源：http://bi.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://yf.shxzskj.cn

[C03] 可变参数
来源：http://lu.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://tu.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zq.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://va.yuntaijiaju.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bm.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cb.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hg.lnxyls.cn

Ruby: def total(*nums); nums.sum; end
来源：http://no.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ze.9csxet.cn

[C04] 命名参数 / 关键字参数
来源：http://kw.haigaiapp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fv.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hg.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://di.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nw.muxihuayi.cn

Java: // 无：用 Builder 模式或 record
来源：http://sn.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://bd.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://kd.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://hy.shxzukj.cn

[C05] 返回多个值
来源：http://tx.colortex.cn

Py:   return a, b
来源：http://do.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://mx.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fy.yuexingan06.cn

TS:   return { a, b };
来源：http://jk.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ox.wgjwhj.cn

Go:   return a, b
来源：http://po.shxzukj.cn

Ruby: return a, b
来源：http://nn.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://eh.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://pu.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://hy.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://on.gzmigu.cn

JS:   const square = x => x * x;
来源：http://cw.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://qj.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fy.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tp.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://uo.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wl.nszjky.cn

[C07] 把函数作为参数传入
来源：http://aq.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jc.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vw.bookmarksfly.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tg.shxzukj.cn

TS:   arr.map(String)
来源：http://yg.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uq.hahajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gj.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://gz.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gu.jianghongdianzi.cn

[C08] 闭包
来源：http://sz.szxytkj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qi.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wb.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://na.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ce.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ft.newstarts.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vn.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vj.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eb.jianghongdianzi.cn

[C09] 递归
来源：http://mk.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ou.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://up.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xp.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bj.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://se.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cx.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jk.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://he.colortex.cn

[C10] 变量作用域
来源：http://ye.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fm.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iq.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://im.shxzskj.cn

TS:   同 JS
来源：http://kr.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://iy.newstarts.cn

Go:   花括号块级作用域
来源：http://jv.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://px.nszjky.cn

C#:   块级作用域
来源：http://yq.huixiangedu.cn

[C11] 模块导入与导出
来源：http://ax.hnjuh.cn

Py:   from module import func
来源：http://am.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://if.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://th.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jp.yuexingan06.cn

Java: import java.util.List;
来源：http://pk.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://go.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://eh.asd995.cn

C#:   using System.Text;
来源：http://cg.521024.cn

[C12] 立即执行函数 IIFE
来源：http://uk.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://mv.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://cs.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://hx.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://ub.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dv.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://ue.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://ro.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qb.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://aa.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://js.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uf.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gw.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dq.huixinmuqiang.cn

Java: int add(int a, int b) { return a + b; }
来源：http://od.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://kx.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gl.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://np.chemitech.net.cn

[C14] 泛型函数
来源：http://os.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ju.hnjuh.cn

PHP:  // 无泛型
来源：http://vo.shxzukj.cn

JS:   // 无泛型
来源：http://qu.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oa.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kw.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ol.521024.cn

Ruby: # 无泛型
来源：http://zf.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ma.nszjky.cn

[C15] 解构 / 展开参数
来源：http://dc.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ro.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://yx.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nh.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xx.bjjhwx.cn

Java: // 无解构
来源：http://cd.hnjuh.cn

Go:   // 无解构
来源：http://rj.asd995.cn

Ruby: a, b = pair
来源：http://kh.nszjky.cn

C#:   var (a, b) = pair;
来源：http://xs.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://se.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vw.nszjky.cn

PHP:  // 无重载
来源：http://cr.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pl.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://ln.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nk.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://rm.huanxung.cn

Ruby: # 无重载：靠动态参数
来源：http://mq.yuexingan06.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lm.chemitech.net.cn

================================================================================
来源：http://nf.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://rf.hahajie.cn

================================================================================
来源：http://wy.hahajie.cn

[D01] 创建数组 / 列表
来源：http://wq.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://sy.shtwfgs.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nt.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vl.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xt.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yj.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://ny.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://ib.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cq.panjiajie.cn

[D02] 追加元素到末尾
来源：http://nj.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vm.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ol.szxytkj.cn

JS:   arr.push(4);
来源：http://pn.huixiangedu.cn

TS:   arr.push(4);
来源：http://cx.bjjhwx.cn

Java: list.add(4);
来源：http://yi.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://jh.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://oc.gzmigu.cn

C#:   list.Add(4);
来源：http://av.hahajie.cn

[D03] 在指定位置插入元素
来源：http://ik.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://eh.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pi.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ab.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ue.wgjwhj.cn

Java: list.add(0, 0);
来源：http://zk.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zu.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qq.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://wn.huixinmuqiang.cn

[D04] 删除元素
来源：http://xc.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sm.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vs.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mh.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://qb.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qf.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ci.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ho.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rh.bjjhwx.cn

[D05] 访问与修改元素
来源：http://yg.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qr.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wy.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mt.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://nw.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ig.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ok.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ca.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://is.huixiangedu.cn

[D06] 数组长度
来源：http://wl.bookmarksfly.cn

Py:   len(arr)
来源：http://ah.hnjuh.cn

PHP:  count($arr);
来源：http://ja.hnjuh.cn

JS:   arr.length
来源：http://fk.shxzskj.cn

TS:   arr.length
来源：http://vi.huixiangedu.cn

Java: list.size();
来源：http://ct.hnjuh.cn

Go:   len(arr)
来源：http://hg.hahajie.cn

Ruby: arr.length; arr.size
来源：http://or.shtwfgs.cn

C#:   list.Count;
来源：http://jy.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://kw.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rm.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://md.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://li.521024.cn

TS:   arr.slice(1, 4);
来源：http://so.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://gt.szsharing.cn

Go:   arr[1:4]
来源：http://gf.szxytkj.cn

Ruby: arr[1, 3]
来源：http://nf.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://ms.nszjky.cn

[D08] 合并两个数组
来源：http://fp.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://ja.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://wl.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dr.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://gd.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sr.gzmigu.cn

Go:   append(a, b...)
来源：http://va.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://bw.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://lp.newstarts.cn

[D09] 排序（升序）
来源：http://hx.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://oi.shtwfgs.cn

PHP:  sort($arr);
来源：http://xh.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xp.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ry.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oe.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oa.colortex.cn

Ruby: arr.sort
来源：http://nz.bookmarksfly.cn

C#:   list.Sort();
来源：http://yh.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iv.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hq.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wa.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dn.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ua.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vm.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yr.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pj.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dz.bookmarksfly.cn

[D11] 反转数组
来源：http://hu.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jj.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://bz.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tu.hnjuh.cn

TS:   [...arr].reverse();
来源：http://di.521024.cn

Java: Collections.reverse(list);
来源：http://as.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://ze.521024.cn

Ruby: arr.reverse
来源：http://rc.hnjuh.cn

C#:   list.Reverse();
来源：http://sc.muxihuayi.cn

[D12] 查找元素下标
来源：http://ql.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://lw.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gv.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xm.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kr.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ch.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://ha.haigaiapp.cn

Ruby: arr.index(x)
来源：http://fv.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://ic.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://rk.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dn.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ng.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://zd.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://ju.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ti.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://es.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jn.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nq.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://aq.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ue.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yu.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://ml.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://ki.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ds.nicolike.cn

Go:   // 手写循环
来源：http://ot.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qu.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wk.yuntaijiaju.cn

[D15] 去重
来源：http://fj.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vh.nszjky.cn

PHP:  array_unique($arr);
来源：http://yt.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://vu.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://fd.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://up.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jk.colortex.cn

Ruby: arr.uniq
来源：http://fu.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://yj.jctech888.com.cn

[D16] 求和与平均值
来源：http://bp.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xf.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bj.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yx.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zn.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ov.nszjky.cn

Go:   // 手写循环累加
来源：http://hb.yuntaijiaju.cn


<!-- 参考信息 -->