代发 wailian999

Java: if (data == null) return;
来源：http://ia.huanxung.cn

Go:   if data == nil { return }
来源：http://kl.jctech888.com.cn

Ruby: return if data.nil?
来源：http://et.newstarts.cn

C#:   if (data == null) return;
来源：http://xl.szxytkj.cn

================================================================================
来源：http://vk.shtwfgs.cn

C. 函数与作用域
来源：http://on.huixinmuqiang.cn

================================================================================
来源：http://ye.bjjhwx.cn

[C01] 定义函数
来源：http://lv.gzmigu.cn

Py:   def add(a, b): return a + b
来源：http://aw.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bp.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://nv.huanxung.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://no.haigaiapp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wv.nicolike.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ea.szsharing.cn

Ruby: def add(a, b); a + b; end
来源：http://ae.yuntaijiaju.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ls.muxihuayi.cn

[C02] 默认参数
来源：http://ry.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://js.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ab.yuntaijiaju.cn

JS:   function greet(name = "World") { return name; }
来源：http://th.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://la.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ke.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fp.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://sa.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://xt.wgjwhj.cn

[C03] 可变参数
来源：http://xs.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://vc.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mg.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://de.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mi.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rt.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pr.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dy.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xy.hahajie.cn

[C04] 命名参数 / 关键字参数
来源：http://sd.nszjky.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://za.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aw.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gj.newstarts.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ud.wgjwhj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ms.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://jf.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://xt.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://rt.lnxyls.cn

[C05] 返回多个值
来源：http://yu.shtwfgs.cn

Py:   return a, b
来源：http://hr.szxytkj.cn

PHP:  return [$a, $b];
来源：http://be.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cp.9csxet.cn

TS:   return { a, b };
来源：http://ic.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vv.szxytkj.cn

Go:   return a, b
来源：http://gx.hahajie.cn

Ruby: return a, b
来源：http://dk.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://vk.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://wg.panjiajie.cn

Py:   square = lambda x: x * x
来源：http://va.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://if.521024.cn

JS:   const square = x => x * x;
来源：http://mg.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://uo.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tb.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ci.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://da.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dh.9csxet.cn

[C07] 把函数作为参数传入
来源：http://dv.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ar.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ye.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://en.shtwfgs.cn

TS:   arr.map(String)
来源：http://kw.bookmarksfly.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://yd.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bv.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://jp.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ff.huixiangedu.cn

[C08] 闭包
来源：http://vj.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mm.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jz.colortex.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tn.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nc.hahajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gu.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kd.hahajie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ly.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kw.huixiangedu.cn

[C09] 递归
来源：http://uc.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tu.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nx.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ru.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dy.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ce.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mq.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://df.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ry.muxihuayi.cn

[C10] 变量作用域
来源：http://cb.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bz.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://un.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xt.shxzukj.cn

TS:   同 JS
来源：http://vu.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://wl.hnjuh.cn

Go:   花括号块级作用域
来源：http://hf.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qa.hnjuh.cn

C#:   块级作用域
来源：http://ol.lnxyls.cn

[C11] 模块导入与导出
来源：http://ft.wgjwhj.cn

Py:   from module import func
来源：http://pg.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aa.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dk.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rt.yuntaijiaju.cn

Java: import java.util.List;
来源：http://eg.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xn.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://dd.asd995.cn

C#:   using System.Text;
来源：http://oj.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://pr.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://cf.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://gb.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://yq.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://yq.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dv.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://vt.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://oa.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ci.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://ct.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gt.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vj.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sd.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ic.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qf.lnxyls.cn

Go:   func add(a, b int) int
来源：http://mt.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kk.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jc.hahajie.cn

[C14] 泛型函数
来源：http://df.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ga.nszjky.cn

PHP:  // 无泛型
来源：http://nj.bookmarksfly.cn

JS:   // 无泛型
来源：http://ez.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tc.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zu.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wo.bookmarksfly.cn

Ruby: # 无泛型
来源：http://is.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fv.asd995.cn

[C15] 解构 / 展开参数
来源：http://mm.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vu.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://pm.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hq.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ss.colortex.cn

Java: // 无解构
来源：http://eu.huanxung.cn

Go:   // 无解构
来源：http://as.shtwfgs.cn

Ruby: a, b = pair
来源：http://xm.asd995.cn

C#:   var (a, b) = pair;
来源：http://tk.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://ng.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://la.lnxyls.cn

PHP:  // 无重载
来源：http://kh.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zu.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://vr.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uy.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://xu.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://xo.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wq.szxytkj.cn

================================================================================
来源：http://mx.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://es.muxihuayi.cn

================================================================================
来源：http://nj.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://ht.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bc.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uu.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xx.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ru.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pp.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://tj.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://rb.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kv.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://vu.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wu.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://si.bjjhwx.cn

JS:   arr.push(4);
来源：http://nh.wgjwhj.cn

TS:   arr.push(4);
来源：http://sd.chemitech.net.cn

Java: list.add(4);
来源：http://af.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://jg.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://xf.hahajie.cn

C#:   list.Add(4);
来源：http://ei.521024.cn

[D03] 在指定位置插入元素
来源：http://yc.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://rf.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ro.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ni.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://ej.szsharing.cn

Java: list.add(0, 0);
来源：http://la.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yw.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://co.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://ne.muxihuayi.cn

[D04] 删除元素
来源：http://rx.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wh.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eq.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sp.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://kc.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qm.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ra.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cs.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bp.wgjwhj.cn

[D05] 访问与修改元素
来源：http://fq.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cr.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dw.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rc.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://qo.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://uk.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://pb.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zq.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://po.colortex.cn

[D06] 数组长度
来源：http://bu.nszjky.cn

Py:   len(arr)
来源：http://na.nicolike.cn

PHP:  count($arr);
来源：http://gw.gzmigu.cn

JS:   arr.length
来源：http://re.shxzskj.cn

TS:   arr.length
来源：http://aa.shxzukj.cn

Java: list.size();
来源：http://oi.bookmarksfly.cn

Go:   len(arr)
来源：http://sw.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://fn.newstarts.cn

C#:   list.Count;
来源：http://gv.521024.cn

[D07] 切片 / 取子数组
来源：http://ge.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qo.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bm.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://lj.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://rm.nszjky.cn

Java: list.subList(1, 4);
来源：http://kg.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://bl.newstarts.cn

Ruby: arr[1, 3]
来源：http://tu.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://wo.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://wn.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://zx.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://ru.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qr.panjiajie.cn

TS:   [...a, ...b];
来源：http://ul.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://io.9csxet.cn

Go:   append(a, b...)
来源：http://tt.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://fs.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://iw.wgjwhj.cn

[D09] 排序（升序）
来源：http://oq.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ll.yuexingan06.cn

PHP:  sort($arr);
来源：http://xc.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://in.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jx.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://br.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://st.hahajie.cn

Ruby: arr.sort
来源：http://na.newstarts.cn

C#:   list.Sort();
来源：http://du.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ra.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lx.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eu.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rk.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://en.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hm.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ck.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gf.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uw.yuntaijiaju.cn

[D11] 反转数组
来源：http://ud.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pm.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://kt.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qt.nicolike.cn

TS:   [...arr].reverse();
来源：http://zs.lnxyls.cn

Java: Collections.reverse(list);
来源：http://qn.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://ic.nszjky.cn

Ruby: arr.reverse
来源：http://vy.9csxet.cn

C#:   list.Reverse();
来源：http://ai.lnxyls.cn

[D12] 查找元素下标
来源：http://ov.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://tb.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ag.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qo.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://th.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hg.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://iu.chemitech.net.cn

Ruby: arr.index(x)
来源：http://hs.521024.cn

C#:   list.IndexOf(x);
来源：http://xz.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://gi.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qs.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://le.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://br.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://jw.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ml.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dl.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fv.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ns.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://iv.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bu.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gh.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://oa.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://rn.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gx.jianghongdianzi.cn

Go:   // 手写循环
来源：http://ub.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vf.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zt.haigaiapp.cn

[D15] 去重
来源：http://nx.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://za.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://hk.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://jh.newstarts.cn

TS:   [...new Set(arr)]
来源：http://nn.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eq.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ds.9csxet.cn

Ruby: arr.uniq
来源：http://to.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://fd.szsharing.cn

[D16] 求和与平均值
来源：http://zz.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ie.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bw.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rd.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lw.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ig.shxzukj.cn

Go:   // 手写循环累加
来源：http://em.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://th.panjiajie.cn

[D17] 最大值与最小值
来源：http://it.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://ww.nicolike.cn


<!-- 参考信息 -->