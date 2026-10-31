代发 wailian999

================================================================================
来源：http://bh.9csxet.cn

C. 函数与作用域
来源：http://jq.huixinmuqiang.cn

================================================================================
来源：http://ug.hahajie.cn

[C01] 定义函数
来源：http://ir.huixinmuqiang.cn

Py:   def add(a, b): return a + b
来源：http://le.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uv.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://lm.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hf.jianghongdianzi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iy.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ff.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://th.huanxung.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zy.yuntaijiaju.cn

[C02] 默认参数
来源：http://hw.haigaiapp.cn

Py:   def greet(name="World"): return name
来源：http://hh.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ni.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://sn.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yw.huanxung.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yd.gzmigu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xe.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://co.wgjwhj.cn

C#:   string Greet(string name = "World") => name;
来源：http://yz.9csxet.cn

[C03] 可变参数
来源：http://mn.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://vj.szsharing.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cg.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ii.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hk.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xk.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ie.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wr.huanxung.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tu.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://te.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tg.nszjky.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ph.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ja.gzmigu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://co.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ch.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://dk.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://er.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://qa.bookmarksfly.cn

[C05] 返回多个值
来源：http://tp.huixiangedu.cn

Py:   return a, b
来源：http://th.hahajie.cn

PHP:  return [$a, $b];
来源：http://lw.yuntaijiaju.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vp.hahajie.cn

TS:   return { a, b };
来源：http://ub.lnxyls.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://eb.huanxung.cn

Go:   return a, b
来源：http://or.muxihuayi.cn

Ruby: return a, b
来源：http://oq.colortex.cn

C#:   return (a, b);              // ValueTuple
来源：http://ys.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://zh.9csxet.cn

Py:   square = lambda x: x * x
来源：http://ac.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://da.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://oj.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://nm.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ch.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ft.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://ml.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wq.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://xd.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hf.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jh.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ko.jctech888.com.cn

TS:   arr.map(String)
来源：http://pw.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yc.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hs.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://ls.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lk.shxzukj.cn

[C08] 闭包
来源：http://ql.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tq.asd995.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jt.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zu.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yk.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ee.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ac.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://al.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ss.nszjky.cn

[C09] 递归
来源：http://ee.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ez.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vj.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jr.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oy.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://id.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lj.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ae.huixiangedu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sj.hahajie.cn

[C10] 变量作用域
来源：http://mf.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qp.asd995.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vq.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hs.521024.cn

TS:   同 JS
来源：http://ou.hahajie.cn

Java: 方法内为块级作用域
来源：http://sb.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://uz.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uj.newstarts.cn

C#:   块级作用域
来源：http://dq.nicolike.cn

[C11] 模块导入与导出
来源：http://px.haigaiapp.cn

Py:   from module import func
来源：http://or.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sh.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fp.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dn.panjiajie.cn

Java: import java.util.List;
来源：http://fo.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zu.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://sm.huanxung.cn

C#:   using System.Text;
来源：http://ky.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://ye.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://pw.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://qu.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://xf.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://xz.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vy.nszjky.cn

Go:   func() { fmt.Println("run") }()
来源：http://az.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://im.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ek.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://os.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gm.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qc.huixinmuqiang.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tb.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kk.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pe.lnxyls.cn

Go:   func add(a, b int) int
来源：http://ba.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wk.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://if.gzmigu.cn

[C14] 泛型函数
来源：http://og.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pj.chemitech.net.cn

PHP:  // 无泛型
来源：http://sv.gzmigu.cn

JS:   // 无泛型
来源：http://xa.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pm.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hm.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yq.nszjky.cn

Ruby: # 无泛型
来源：http://vn.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yg.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://ry.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lc.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://wi.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lc.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ed.9csxet.cn

Java: // 无解构
来源：http://ze.haigaiapp.cn

Go:   // 无解构
来源：http://nt.bjjhwx.cn

Ruby: a, b = pair
来源：http://zh.521024.cn

C#:   var (a, b) = pair;
来源：http://ct.nicolike.cn

[C16] 函数 / 方法重载
来源：http://kh.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yr.szxytkj.cn

PHP:  // 无重载
来源：http://ev.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bu.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://rh.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://au.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://hc.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://ub.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wq.lnxyls.cn

================================================================================
来源：http://kh.colortex.cn

D. 数组 / 列表 / 集合
来源：http://es.9csxet.cn

================================================================================
来源：http://eh.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://yw.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nb.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://il.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ok.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ou.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cc.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://pa.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://lm.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tl.panjiajie.cn

[D02] 追加元素到末尾
来源：http://ch.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xa.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pb.gzmigu.cn

JS:   arr.push(4);
来源：http://tp.asd995.cn

TS:   arr.push(4);
来源：http://yg.bookmarksfly.cn

Java: list.add(4);
来源：http://vf.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://km.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://ej.huixiangedu.cn

C#:   list.Add(4);
来源：http://tg.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://wc.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://ty.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kc.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lb.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://co.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://nb.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pc.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vi.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://xi.huixiangedu.cn

[D04] 删除元素
来源：http://jk.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pw.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dq.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://af.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://qa.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ae.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ir.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ky.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vp.yuexingan06.cn

[D05] 访问与修改元素
来源：http://do.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dq.huanxung.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ra.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bs.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://vi.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://fe.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://wi.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cu.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://er.hnjuh.cn

[D06] 数组长度
来源：http://fc.hnjuh.cn

Py:   len(arr)
来源：http://ib.chemitech.net.cn

PHP:  count($arr);
来源：http://sn.nicolike.cn

JS:   arr.length
来源：http://ct.szxytkj.cn

TS:   arr.length
来源：http://ga.9csxet.cn

Java: list.size();
来源：http://vs.huixiangedu.cn

Go:   len(arr)
来源：http://nb.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://tv.gzmigu.cn

C#:   list.Count;
来源：http://fj.colortex.cn

[D07] 切片 / 取子数组
来源：http://gj.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ke.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://di.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://yy.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://jy.huanxung.cn

Java: list.subList(1, 4);
来源：http://qc.yuexingan06.cn

Go:   arr[1:4]
来源：http://if.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://do.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://ef.wgjwhj.cn

[D08] 合并两个数组
来源：http://fw.colortex.cn

Py:   a + b;  a.extend(b)
来源：http://oh.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://zx.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yh.shxzukj.cn

TS:   [...a, ...b];
来源：http://uw.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ph.asd995.cn

Go:   append(a, b...)
来源：http://iu.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://hc.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://le.szsharing.cn

[D09] 排序（升序）
来源：http://hr.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zg.huanxung.cn

PHP:  sort($arr);
来源：http://xn.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wx.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://de.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oh.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ha.huixiangedu.cn

Ruby: arr.sort
来源：http://hs.shxzskj.cn

C#:   list.Sort();
来源：http://tn.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yw.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ic.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ts.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dr.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hf.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sv.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fd.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rp.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oe.yuntaijiaju.cn

[D11] 反转数组
来源：http://lj.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ti.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://vm.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fg.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://if.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://ep.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://wl.gzmigu.cn

Ruby: arr.reverse
来源：http://cv.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://sz.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://dj.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://ur.huixiangedu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dh.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nq.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oh.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ee.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://hi.chemitech.net.cn

Ruby: arr.index(x)
来源：http://xe.colortex.cn

C#:   list.IndexOf(x);
来源：http://ai.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://rq.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uy.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gv.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://qs.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://aj.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sd.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pp.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://so.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vs.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://ls.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kk.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aq.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://kp.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://nt.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ij.huixinmuqiang.cn

Go:   // 手写循环
来源：http://fc.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://br.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xq.asd995.cn

[D15] 去重
来源：http://os.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ai.nicolike.cn

PHP:  array_unique($arr);
来源：http://ne.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://qm.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://kf.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xm.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zs.huixiangedu.cn

Ruby: arr.uniq
来源：http://pc.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://fi.muxihuayi.cn

[D16] 求和与平均值
来源：http://ni.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://in.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xd.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hw.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://au.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pf.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://bx.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bi.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://vb.nicolike.cn

[D17] 最大值与最小值
来源：http://ge.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://mn.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://yt.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vh.nicolike.cn

TS:   Math.max(...arr);
来源：http://zf.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fw.bookmarksfly.cn


<!-- 参考信息 -->