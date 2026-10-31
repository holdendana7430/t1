代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://jn.jctech888.com.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bq.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uj.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://gr.newstarts.cn

C#:   string Greet(string name = "World") => name;
来源：http://mh.shxzukj.cn

[C03] 可变参数
来源：http://bo.521024.cn

Py:   def total(*args): return sum(args)
来源：http://ia.muxihuayi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://la.bookmarksfly.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ft.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qq.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rm.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ga.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rc.panjiajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vx.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://li.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qi.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jl.muxihuayi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uu.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hc.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://yw.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://gi.yuexingan06.cn

Ruby: f(a: 1, b: 2)
来源：http://gu.shxzukj.cn

C#:   f(a: 1, b: 2)
来源：http://ct.nicolike.cn

[C05] 返回多个值
来源：http://la.szxytkj.cn

Py:   return a, b
来源：http://uj.shxzskj.cn

PHP:  return [$a, $b];
来源：http://jc.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ng.521024.cn

TS:   return { a, b };
来源：http://fm.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sh.panjiajie.cn

Go:   return a, b
来源：http://bc.szxytkj.cn

Ruby: return a, b
来源：http://ah.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://vc.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://sm.szsharing.cn

Py:   square = lambda x: x * x
来源：http://kt.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yf.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://uf.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://pi.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xf.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pe.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://ye.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vt.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://kd.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uc.shxzskj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rd.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kz.huanxung.cn

TS:   arr.map(String)
来源：http://op.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bi.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oz.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://uh.nicolike.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sb.nszjky.cn

[C08] 闭包
来源：http://ml.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wf.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hv.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vs.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sj.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qs.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iu.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://de.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vz.shxzukj.cn

[C09] 递归
来源：http://lt.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qa.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ce.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://og.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xa.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dl.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zr.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wf.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nb.hahajie.cn

[C10] 变量作用域
来源：http://ia.bjjhwx.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dc.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zu.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zu.shxzskj.cn

TS:   同 JS
来源：http://dx.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://sj.gzmigu.cn

Go:   花括号块级作用域
来源：http://wv.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ik.bookmarksfly.cn

C#:   块级作用域
来源：http://kw.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://pu.9csxet.cn

Py:   from module import func
来源：http://sq.newstarts.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://di.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ea.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dc.jctech888.com.cn

Java: import java.util.List;
来源：http://zl.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iu.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://zx.bjjhwx.cn

C#:   using System.Text;
来源：http://nz.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://ts.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://yx.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://kr.yuntaijiaju.cn

JS:   (() => { console.log("run"); })();
来源：http://ac.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://zy.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rd.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://uv.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://mg.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ac.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://hb.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oi.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iu.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rm.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://za.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://to.szxytkj.cn

Go:   func add(a, b int) int
来源：http://cq.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ij.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cz.lnxyls.cn

[C14] 泛型函数
来源：http://ha.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xy.bjjhwx.cn

PHP:  // 无泛型
来源：http://bk.shtwfgs.cn

JS:   // 无泛型
来源：http://ek.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://um.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gi.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lr.9csxet.cn

Ruby: # 无泛型
来源：http://uo.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mw.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://uz.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gg.jianghongdianzi.cn

PHP:  [$a, $b] = $pair;
来源：http://kv.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xj.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cr.lnxyls.cn

Java: // 无解构
来源：http://we.bjjhwx.cn

Go:   // 无解构
来源：http://we.jctech888.com.cn

Ruby: a, b = pair
来源：http://yi.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://lq.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://bd.nicolike.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aj.szxytkj.cn

PHP:  // 无重载
来源：http://sf.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cq.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://ba.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ix.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://qa.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://qt.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sf.bjjhwx.cn

================================================================================
来源：http://ga.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ub.521024.cn

================================================================================
来源：http://mr.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://sk.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mr.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bi.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sf.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yw.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fb.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://fv.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://bw.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ds.521024.cn

[D02] 追加元素到末尾
来源：http://qk.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dp.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://re.hahajie.cn

JS:   arr.push(4);
来源：http://yc.9csxet.cn

TS:   arr.push(4);
来源：http://vl.hnjuh.cn

Java: list.add(4);
来源：http://ok.colortex.cn

Go:   arr = append(arr, 4)
来源：http://dq.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://lh.shxzukj.cn

C#:   list.Add(4);
来源：http://xy.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://ur.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://rs.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xe.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qw.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://me.haigaiapp.cn

Java: list.add(0, 0);
来源：http://ii.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xm.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uy.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://iw.colortex.cn

[D04] 删除元素
来源：http://zn.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tp.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uf.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ik.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://ze.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ml.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lu.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sy.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fn.hahajie.cn

[D05] 访问与修改元素
来源：http://rc.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://er.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iv.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tt.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://za.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://vp.bjjhwx.cn

Go:   arr[0]; arr[0] = 9
来源：http://ca.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://in.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jg.bookmarksfly.cn

[D06] 数组长度
来源：http://ot.newstarts.cn

Py:   len(arr)
来源：http://xm.521024.cn

PHP:  count($arr);
来源：http://uu.lnxyls.cn

JS:   arr.length
来源：http://du.hnjuh.cn

TS:   arr.length
来源：http://nr.shxzskj.cn

Java: list.size();
来源：http://hf.lnxyls.cn

Go:   len(arr)
来源：http://ug.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://np.bjjhwx.cn

C#:   list.Count;
来源：http://nk.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://pd.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vp.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ln.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://op.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://lp.9csxet.cn

Java: list.subList(1, 4);
来源：http://hv.shxzskj.cn

Go:   arr[1:4]
来源：http://nn.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://ne.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://xx.shxzskj.cn

[D08] 合并两个数组
来源：http://jj.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://ub.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://ye.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ul.colortex.cn

TS:   [...a, ...b];
来源：http://ts.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zv.nszjky.cn

Go:   append(a, b...)
来源：http://qi.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://kh.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://zo.muxihuayi.cn

[D09] 排序（升序）
来源：http://ic.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://ln.gzmigu.cn

PHP:  sort($arr);
来源：http://zu.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bu.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xu.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jl.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lz.nszjky.cn

Ruby: arr.sort
来源：http://dh.haigaiapp.cn

C#:   list.Sort();
来源：http://qs.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qf.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wf.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lp.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vb.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zb.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dt.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rr.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dl.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yx.colortex.cn

[D11] 反转数组
来源：http://dc.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rv.hahajie.cn

PHP:  array_reverse($arr);
来源：http://my.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rf.szsharing.cn

TS:   [...arr].reverse();
来源：http://oe.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://gw.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://mw.hahajie.cn

Ruby: arr.reverse
来源：http://vb.bookmarksfly.cn

C#:   list.Reverse();
来源：http://yo.szxytkj.cn

[D12] 查找元素下标
来源：http://yc.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://fj.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eq.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nq.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fn.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://du.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://jr.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ru.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://kj.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://ah.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ks.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qh.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://tg.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://of.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rm.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qa.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ga.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vk.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://bw.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sm.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://er.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://zd.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://mh.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zy.wgjwhj.cn

Go:   // 手写循环
来源：http://ko.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rl.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nm.huixiangedu.cn

[D15] 去重
来源：http://om.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nd.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://gu.asd995.cn

JS:   [...new Set(arr)]
来源：http://mv.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://ry.newstarts.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ma.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ll.szsharing.cn

Ruby: arr.uniq
来源：http://fg.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://dn.lnxyls.cn

[D16] 求和与平均值
来源：http://xh.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ud.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bi.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pn.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://so.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wh.nszjky.cn

Go:   // 手写循环累加
来源：http://zl.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://us.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://zc.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ob.asd995.cn

Py:   max(arr);  min(arr)
来源：http://xv.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://kq.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zc.521024.cn

TS:   Math.max(...arr);
来源：http://ns.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dj.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://up.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://hg.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://ky.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ey.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ip.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://xh.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fs.shxzukj.cn

TS:   nested.flat();
来源：http://zr.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tm.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://bc.bjjhwx.cn

Ruby: nested.flatten
来源：http://ea.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://op.shxzskj.cn

[D19] 按字段分组
来源：http://bb.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lb.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xt.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ql.lnxyls.cn


<!-- 参考信息 -->