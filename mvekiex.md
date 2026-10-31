代发 wailian999

Py:   def add(a, b): return a + b
来源：http://bu.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uk.nicolike.cn

JS:   function add(a, b) { return a + b; }
来源：http://eh.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vf.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ne.newstarts.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rp.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://dv.muxihuayi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sn.huixiangedu.cn

[C02] 默认参数
来源：http://fk.521024.cn

Py:   def greet(name="World"): return name
来源：http://xb.hahajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dc.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://fy.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://gw.shxzskj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gx.muxihuayi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rh.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://at.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://xr.yuntaijiaju.cn

[C03] 可变参数
来源：http://nl.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://xq.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eh.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gc.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lh.shtwfgs.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://id.hahajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bs.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fb.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bw.huixinmuqiang.cn

[C04] 命名参数 / 关键字参数
来源：http://bx.colortex.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ed.huanxung.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ug.jianghongdianzi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cd.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://em.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://ho.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://kb.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://lg.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://du.shxzskj.cn

[C05] 返回多个值
来源：http://kp.nszjky.cn

Py:   return a, b
来源：http://vo.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://wf.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iv.bookmarksfly.cn

TS:   return { a, b };
来源：http://rl.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ca.jctech888.com.cn

Go:   return a, b
来源：http://yf.szxytkj.cn

Ruby: return a, b
来源：http://ap.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://ew.yuexingan06.cn

[C06] 匿名函数 / lambda
来源：http://gp.9csxet.cn

Py:   square = lambda x: x * x
来源：http://xx.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ct.lnxyls.cn

JS:   const square = x => x * x;
来源：http://dv.chemitech.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://xk.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zg.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rl.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://rb.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bi.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://eg.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cm.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ta.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://si.panjiajie.cn

TS:   arr.map(String)
来源：http://ok.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ff.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wi.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://mq.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jt.newstarts.cn

[C08] 闭包
来源：http://xt.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mu.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ek.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nm.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ma.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zy.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xk.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ia.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vq.jianghongdianzi.cn

[C09] 递归
来源：http://kv.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yp.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qa.szxytkj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gm.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yz.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lr.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://up.nicolike.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tz.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tn.szsharing.cn

[C10] 变量作用域
来源：http://rv.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cp.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ns.bookmarksfly.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://te.gzmigu.cn

TS:   同 JS
来源：http://hb.colortex.cn

Java: 方法内为块级作用域
来源：http://tf.wgjwhj.cn

Go:   花括号块级作用域
来源：http://xm.szsharing.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xj.hahajie.cn

C#:   块级作用域
来源：http://zi.huixiangedu.cn

[C11] 模块导入与导出
来源：http://vi.szxytkj.cn

Py:   from module import func
来源：http://bp.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cj.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xr.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xj.shxzskj.cn

Java: import java.util.List;
来源：http://xr.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cm.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://xy.lnxyls.cn

C#:   using System.Text;
来源：http://qy.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://jd.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://kx.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://hk.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://bq.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://kg.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ds.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://kb.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://ky.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hu.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://kl.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://et.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vm.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fp.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jw.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bx.hahajie.cn

Go:   func add(a, b int) int
来源：http://rp.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://le.szxytkj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oh.hnjuh.cn

[C14] 泛型函数
来源：http://tm.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oz.9csxet.cn

PHP:  // 无泛型
来源：http://sh.bjjhwx.cn

JS:   // 无泛型
来源：http://xd.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jy.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lp.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fm.yuexingan06.cn

Ruby: # 无泛型
来源：http://wp.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vd.asd995.cn

[C15] 解构 / 展开参数
来源：http://ss.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ns.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://qp.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dd.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oc.szxytkj.cn

Java: // 无解构
来源：http://yd.bjjhwx.cn

Go:   // 无解构
来源：http://od.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://ik.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://nt.9csxet.cn

[C16] 函数 / 方法重载
来源：http://jy.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vc.asd995.cn

PHP:  // 无重载
来源：http://id.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hx.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://rg.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mx.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://bu.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://ts.lnxyls.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ou.bjjhwx.cn

================================================================================
来源：http://yf.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://uv.yuexingan06.cn

================================================================================
来源：http://ow.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://tp.newstarts.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hy.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ww.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://li.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zd.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fk.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://zh.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://ao.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wi.shtwfgs.cn

[D02] 追加元素到末尾
来源：http://ca.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ue.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ug.huanxung.cn

JS:   arr.push(4);
来源：http://zf.wgjwhj.cn

TS:   arr.push(4);
来源：http://nm.gzmigu.cn

Java: list.add(4);
来源：http://sf.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://jd.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://ty.shtwfgs.cn

C#:   list.Add(4);
来源：http://aw.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://ev.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://cd.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mm.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dq.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://yz.asd995.cn

Java: list.add(0, 0);
来源：http://vd.jianghongdianzi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bu.panjiajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ih.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://zd.haigaiapp.cn

[D04] 删除元素
来源：http://yz.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ff.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mf.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jq.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://oa.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bs.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://te.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://us.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zm.panjiajie.cn

[D05] 访问与修改元素
来源：http://ev.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qy.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gu.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ed.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://mu.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://mo.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://ud.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wp.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ue.panjiajie.cn

[D06] 数组长度
来源：http://is.huixiangedu.cn

Py:   len(arr)
来源：http://tb.521024.cn

PHP:  count($arr);
来源：http://qt.gzmigu.cn

JS:   arr.length
来源：http://ii.panjiajie.cn

TS:   arr.length
来源：http://ve.521024.cn

Java: list.size();
来源：http://gf.hahajie.cn

Go:   len(arr)
来源：http://gn.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://dy.bjjhwx.cn

C#:   list.Count;
来源：http://sl.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://ic.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cg.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vr.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://dk.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://zb.colortex.cn

Java: list.subList(1, 4);
来源：http://ap.shtwfgs.cn

Go:   arr[1:4]
来源：http://bv.hnjuh.cn

Ruby: arr[1, 3]
来源：http://vd.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://cl.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://xl.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://dh.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://gz.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://it.szsharing.cn

TS:   [...a, ...b];
来源：http://yi.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lh.huixiangedu.cn

Go:   append(a, b...)
来源：http://ws.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://kq.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://mx.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://fg.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://zj.9csxet.cn

PHP:  sort($arr);
来源：http://qk.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://at.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mg.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://he.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sy.521024.cn

Ruby: arr.sort
来源：http://vg.yuntaijiaju.cn

C#:   list.Sort();
来源：http://dh.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jl.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://im.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qy.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sq.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://so.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://en.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oo.shtwfgs.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sd.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oc.huixinmuqiang.cn

[D11] 反转数组
来源：http://up.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nw.newstarts.cn

PHP:  array_reverse($arr);
来源：http://vf.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ex.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://kb.szxytkj.cn

Java: Collections.reverse(list);
来源：http://fz.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://tw.nicolike.cn

Ruby: arr.reverse
来源：http://tr.nszjky.cn

C#:   list.Reverse();
来源：http://be.nicolike.cn

[D12] 查找元素下标
来源：http://tc.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://fm.colortex.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bd.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://me.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ik.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rh.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://bv.wgjwhj.cn

Ruby: arr.index(x)
来源：http://nj.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://bl.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://je.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ge.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zk.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://kg.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://iu.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nd.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vm.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yv.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://te.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://rf.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zj.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://te.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://fh.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://em.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://za.nicolike.cn

Go:   // 手写循环
来源：http://au.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fq.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pe.lnxyls.cn

[D15] 去重
来源：http://ha.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cs.hahajie.cn

PHP:  array_unique($arr);
来源：http://fg.huanxung.cn

JS:   [...new Set(arr)]
来源：http://tg.colortex.cn

TS:   [...new Set(arr)]
来源：http://np.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wa.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jt.haigaiapp.cn

Ruby: arr.uniq
来源：http://lf.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://ks.panjiajie.cn

[D16] 求和与平均值
来源：http://vd.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fz.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hd.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bb.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wr.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://za.shxzukj.cn

Go:   // 手写循环累加
来源：http://st.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lj.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://oi.huanxung.cn

[D17] 最大值与最小值
来源：http://av.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://un.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://iw.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ey.shxzukj.cn

TS:   Math.max(...arr);
来源：http://eg.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vp.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rz.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://mt.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://gq.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://wn.lnxyls.cn


<!-- 参考信息 -->