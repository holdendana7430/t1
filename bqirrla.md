代发 wailian999

Go:   a && b || !c
来源：http://nr.huanxung.cn

Ruby: a && b || !c
来源：http://eb.huanxung.cn

C#:   a && b || !c
来源：http://bz.szxytkj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fl.szsharing.cn

Py:   if not data: return
来源：http://pd.huixinmuqiang.cn

PHP:  if (!$data) { return; }
来源：http://tx.haigaiapp.cn

JS:   if (!data) return;
来源：http://ev.shxzskj.cn

TS:   if (!data) return;
来源：http://ll.bjjhwx.cn

Java: if (data == null) return;
来源：http://xa.shxzukj.cn

Go:   if data == nil { return }
来源：http://af.szsharing.cn

Ruby: return if data.nil?
来源：http://iq.bookmarksfly.cn

C#:   if (data == null) return;
来源：http://pd.lnxyls.cn

================================================================================
来源：http://fn.szsharing.cn

C. 函数与作用域
来源：http://ls.newstarts.cn

================================================================================
来源：http://vr.yuexingan06.cn

[C01] 定义函数
来源：http://kr.yuntaijiaju.cn

Py:   def add(a, b): return a + b
来源：http://gx.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ma.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://yi.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zg.chemitech.net.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ph.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ge.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://dj.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oi.muxihuayi.cn

[C02] 默认参数
来源：http://bo.newstarts.cn

Py:   def greet(name="World"): return name
来源：http://jk.muxihuayi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ti.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://ni.lnxyls.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hj.shxzukj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tq.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yj.huixinmuqiang.cn

Ruby: def greet(name = "World") = name
来源：http://wo.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://sb.hahajie.cn

[C03] 可变参数
来源：http://lr.huixinmuqiang.cn

Py:   def total(*args): return sum(args)
来源：http://on.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pz.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xz.huixinmuqiang.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uh.jctech888.com.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ko.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vi.yuexingan06.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zn.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://eo.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://is.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://by.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ev.newstarts.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fs.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ob.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://zg.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://aa.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://lo.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://ks.521024.cn

[C05] 返回多个值
来源：http://gl.521024.cn

Py:   return a, b
来源：http://ev.gzmigu.cn

PHP:  return [$a, $b];
来源：http://nq.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://og.9csxet.cn

TS:   return { a, b };
来源：http://rn.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ke.panjiajie.cn

Go:   return a, b
来源：http://vg.szsharing.cn

Ruby: return a, b
来源：http://wo.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://cq.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://qw.asd995.cn

Py:   square = lambda x: x * x
来源：http://li.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ap.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://if.nszjky.cn

TS:   const square = (x: number): number => x * x;
来源：http://to.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zz.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://er.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://nv.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xb.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://zb.bookmarksfly.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gy.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ut.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lv.haigaiapp.cn

TS:   arr.map(String)
来源：http://hq.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tb.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://co.huixiangedu.cn

Ruby: arr.map(&:upcase)
来源：http://ok.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://du.jctech888.com.cn

[C08] 闭包
来源：http://zt.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tz.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dz.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ae.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://df.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zz.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hy.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xo.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ii.shxzskj.cn

[C09] 递归
来源：http://qj.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wl.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rx.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yb.huanxung.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://du.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hm.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xy.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ak.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ak.hnjuh.cn

[C10] 变量作用域
来源：http://sf.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ox.colortex.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zm.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nq.shxzskj.cn

TS:   同 JS
来源：http://ts.gzmigu.cn

Java: 方法内为块级作用域
来源：http://ir.newstarts.cn

Go:   花括号块级作用域
来源：http://jd.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qg.huanxung.cn

C#:   块级作用域
来源：http://xx.colortex.cn

[C11] 模块导入与导出
来源：http://ko.colortex.cn

Py:   from module import func
来源：http://jj.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uv.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wu.huixinmuqiang.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bu.asd995.cn

Java: import java.util.List;
来源：http://og.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wy.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://bu.szsharing.cn

C#:   using System.Text;
来源：http://mx.521024.cn

[C12] 立即执行函数 IIFE
来源：http://cd.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://sb.lnxyls.cn

PHP:  (function () { echo "run"; })();
来源：http://cy.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://pe.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://nb.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fp.yuntaijiaju.cn

Go:   func() { fmt.Println("run") }()
来源：http://lt.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://ba.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xh.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://lp.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ze.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qo.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fp.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tv.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xk.gzmigu.cn

Go:   func add(a, b int) int
来源：http://bu.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ci.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oy.9csxet.cn

[C14] 泛型函数
来源：http://zj.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gi.panjiajie.cn

PHP:  // 无泛型
来源：http://uv.huanxung.cn

JS:   // 无泛型
来源：http://sg.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xi.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jq.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jh.gzmigu.cn

Ruby: # 无泛型
来源：http://jz.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qg.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://ma.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lc.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://ga.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fy.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ve.haigaiapp.cn

Java: // 无解构
来源：http://yq.newstarts.cn

Go:   // 无解构
来源：http://iv.szsharing.cn

Ruby: a, b = pair
来源：http://fd.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://em.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ps.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ei.huanxung.cn

PHP:  // 无重载
来源：http://kt.bjjhwx.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ix.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://be.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rt.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://wd.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://qw.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uk.jianghongdianzi.cn

================================================================================
来源：http://pa.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://yr.szsharing.cn

================================================================================
来源：http://ey.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://in.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://no.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lq.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qx.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kd.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wo.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://dl.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://ny.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://al.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://mt.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hl.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://re.haigaiapp.cn

JS:   arr.push(4);
来源：http://cv.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://vm.bjjhwx.cn

Java: list.add(4);
来源：http://nf.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://ef.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ki.szsharing.cn

C#:   list.Add(4);
来源：http://rp.hahajie.cn

[D03] 在指定位置插入元素
来源：http://rf.521024.cn

Py:   arr.insert(0, 0)
来源：http://ys.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dg.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xv.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://io.newstarts.cn

Java: list.add(0, 0);
来源：http://ni.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xn.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rw.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://eg.jctech888.com.cn

[D04] 删除元素
来源：http://ma.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wh.shtwfgs.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pd.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zq.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://yl.huanxung.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jp.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sr.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kj.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://be.huixiangedu.cn

[D05] 访问与修改元素
来源：http://ju.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://se.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dl.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dj.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://mi.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://dk.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://eg.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hq.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ho.szxytkj.cn

[D06] 数组长度
来源：http://hz.asd995.cn

Py:   len(arr)
来源：http://en.shxzukj.cn

PHP:  count($arr);
来源：http://zh.jianghongdianzi.cn

JS:   arr.length
来源：http://jr.hnjuh.cn

TS:   arr.length
来源：http://ow.huixiangedu.cn

Java: list.size();
来源：http://qk.gzmigu.cn

Go:   len(arr)
来源：http://qk.yuexingan06.cn

Ruby: arr.length; arr.size
来源：http://fg.panjiajie.cn

C#:   list.Count;
来源：http://zy.521024.cn

[D07] 切片 / 取子数组
来源：http://bp.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zy.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zr.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://ep.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://fq.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://jd.szsharing.cn

Go:   arr[1:4]
来源：http://en.newstarts.cn

Ruby: arr[1, 3]
来源：http://cj.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://gj.nicolike.cn

[D08] 合并两个数组
来源：http://po.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://dx.521024.cn

PHP:  array_merge($a, $b);
来源：http://li.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eb.bjjhwx.cn

TS:   [...a, ...b];
来源：http://do.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://og.bookmarksfly.cn

Go:   append(a, b...)
来源：http://rx.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://jy.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://zp.colortex.cn

[D09] 排序（升序）
来源：http://yo.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://on.haigaiapp.cn

PHP:  sort($arr);
来源：http://dz.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zw.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hk.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kt.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zl.shtwfgs.cn

Ruby: arr.sort
来源：http://ci.huanxung.cn

C#:   list.Sort();
来源：http://yr.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cn.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sa.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kc.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iq.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://an.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qd.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ak.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gl.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jp.huixinmuqiang.cn

[D11] 反转数组
来源：http://co.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://aw.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://bb.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://me.panjiajie.cn

TS:   [...arr].reverse();
来源：http://kd.huanxung.cn

Java: Collections.reverse(list);
来源：http://fb.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://mf.colortex.cn

Ruby: arr.reverse
来源：http://an.panjiajie.cn

C#:   list.Reverse();
来源：http://yk.nicolike.cn

[D12] 查找元素下标
来源：http://vf.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://hg.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yq.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jz.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jk.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zl.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://sw.9csxet.cn

Ruby: arr.index(x)
来源：http://fr.colortex.cn

C#:   list.IndexOf(x);
来源：http://uv.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://wu.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jn.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kt.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://aw.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://vh.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cz.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ph.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fd.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://am.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://mz.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gt.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oq.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://xi.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://bd.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ho.colortex.cn

Go:   // 手写循环
来源：http://he.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ji.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ai.asd995.cn

[D15] 去重
来源：http://cl.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ym.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://ht.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://tj.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://yh.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fs.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://du.hahajie.cn

Ruby: arr.uniq
来源：http://jw.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://eg.hnjuh.cn

[D16] 求和与平均值
来源：http://io.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vn.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://el.panjiajie.cn


<!-- 参考信息 -->