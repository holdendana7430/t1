代发 wailian999

[C02] 默认参数
来源：http://wa.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://ts.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yb.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://uc.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yv.szsharing.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ef.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sr.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://py.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://ea.colortex.cn

[C03] 可变参数
来源：http://ui.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://mz.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xk.hnjuh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vr.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lz.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yf.huixiangedu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://be.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ex.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lh.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://dk.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qq.yuntaijiaju.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lc.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gr.shxzukj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xm.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://av.huixiangedu.cn

Go:   // 无：用配置结构体参数
来源：http://mz.gzmigu.cn

Ruby: f(a: 1, b: 2)
来源：http://hl.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://up.chemitech.net.cn

[C05] 返回多个值
来源：http://mg.muxihuayi.cn

Py:   return a, b
来源：http://dz.panjiajie.cn

PHP:  return [$a, $b];
来源：http://ah.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nf.gzmigu.cn

TS:   return { a, b };
来源：http://fv.bookmarksfly.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vu.shtwfgs.cn

Go:   return a, b
来源：http://so.521024.cn

Ruby: return a, b
来源：http://jv.muxihuayi.cn

C#:   return (a, b);              // ValueTuple
来源：http://pd.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://gj.521024.cn

Py:   square = lambda x: x * x
来源：http://hl.yuexingan06.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qo.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://rl.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://hw.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yw.szsharing.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gj.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://eg.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lh.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://cs.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fe.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rf.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://an.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://so.nszjky.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dl.yuntaijiaju.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cy.szxytkj.cn

Ruby: arr.map(&:upcase)
来源：http://bs.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ec.hahajie.cn

[C08] 闭包
来源：http://dd.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dr.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nq.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qv.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sy.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lb.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kv.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tk.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hj.muxihuayi.cn

[C09] 递归
来源：http://ya.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mr.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ht.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rw.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zs.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://to.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fa.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wb.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nq.shxzukj.cn

[C10] 变量作用域
来源：http://eg.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://le.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ey.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gl.nszjky.cn

TS:   同 JS
来源：http://hg.lnxyls.cn

Java: 方法内为块级作用域
来源：http://yv.muxihuayi.cn

Go:   花括号块级作用域
来源：http://oa.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hl.lnxyls.cn

C#:   块级作用域
来源：http://wt.lnxyls.cn

[C11] 模块导入与导出
来源：http://mo.huixiangedu.cn

Py:   from module import func
来源：http://wm.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hv.chemitech.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gc.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bl.shtwfgs.cn

Java: import java.util.List;
来源：http://dc.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fr.szsharing.cn

Ruby: require "json"; require_relative "./util"
来源：http://sa.muxihuayi.cn

C#:   using System.Text;
来源：http://sg.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://hj.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://yc.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://il.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://hd.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://eu.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hl.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://hl.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://jc.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kg.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://uh.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nw.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xu.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pk.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jg.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kt.521024.cn

Go:   func add(a, b int) int
来源：http://wr.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ob.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tt.szxytkj.cn

[C14] 泛型函数
来源：http://oh.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ka.haigaiapp.cn

PHP:  // 无泛型
来源：http://ij.colortex.cn

JS:   // 无泛型
来源：http://lc.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ie.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lk.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ah.newstarts.cn

Ruby: # 无泛型
来源：http://eh.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lm.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://hc.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vo.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://wc.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nw.huixinmuqiang.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ns.521024.cn

Java: // 无解构
来源：http://sj.shxzskj.cn

Go:   // 无解构
来源：http://tf.asd995.cn

Ruby: a, b = pair
来源：http://gr.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://mc.bookmarksfly.cn

[C16] 函数 / 方法重载
来源：http://xj.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ul.gzmigu.cn

PHP:  // 无重载
来源：http://vl.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qu.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://wx.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://id.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://al.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://kf.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dk.gzmigu.cn

================================================================================
来源：http://lb.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://ra.lnxyls.cn

================================================================================
来源：http://cq.newstarts.cn

[D01] 创建数组 / 列表
来源：http://zy.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ue.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://do.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yn.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gg.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uq.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://bf.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://ax.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wr.huanxung.cn

[D02] 追加元素到末尾
来源：http://qx.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gk.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hd.bookmarksfly.cn

JS:   arr.push(4);
来源：http://sx.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://lj.haigaiapp.cn

Java: list.add(4);
来源：http://bc.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://fw.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://wz.bjjhwx.cn

C#:   list.Add(4);
来源：http://ne.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://tq.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://um.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dx.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qj.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://xu.gzmigu.cn

Java: list.add(0, 0);
来源：http://ye.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qz.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ox.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://wh.chemitech.net.cn

[D04] 删除元素
来源：http://cl.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yj.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://di.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dz.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://dd.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ax.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ms.huixinmuqiang.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tg.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ot.wgjwhj.cn

[D05] 访问与修改元素
来源：http://fu.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://or.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ug.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rz.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://gy.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://sg.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://ge.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hl.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xh.asd995.cn

[D06] 数组长度
来源：http://gp.huanxung.cn

Py:   len(arr)
来源：http://zz.9csxet.cn

PHP:  count($arr);
来源：http://ig.muxihuayi.cn

JS:   arr.length
来源：http://wr.newstarts.cn

TS:   arr.length
来源：http://kc.muxihuayi.cn

Java: list.size();
来源：http://zt.jctech888.com.cn

Go:   len(arr)
来源：http://ek.nicolike.cn

Ruby: arr.length; arr.size
来源：http://dp.jianghongdianzi.cn

C#:   list.Count;
来源：http://tg.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://os.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xy.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lc.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://pm.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://uv.shxzukj.cn

Java: list.subList(1, 4);
来源：http://wg.nszjky.cn

Go:   arr[1:4]
来源：http://xw.huanxung.cn

Ruby: arr[1, 3]
来源：http://rm.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://vy.9csxet.cn

[D08] 合并两个数组
来源：http://hw.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://yq.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://zu.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ju.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ka.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dq.szxytkj.cn

Go:   append(a, b...)
来源：http://vs.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://tt.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://ul.yuexingan06.cn

[D09] 排序（升序）
来源：http://dk.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://zs.muxihuayi.cn

PHP:  sort($arr);
来源：http://vr.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ff.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tu.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hs.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://up.jianghongdianzi.cn

Ruby: arr.sort
来源：http://bv.huixinmuqiang.cn

C#:   list.Sort();
来源：http://rn.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cz.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yh.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bk.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qq.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zb.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mm.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://et.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ga.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qj.yuntaijiaju.cn

[D11] 反转数组
来源：http://qz.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pq.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://kd.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fe.asd995.cn

TS:   [...arr].reverse();
来源：http://aw.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ti.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://wp.jctech888.com.cn

Ruby: arr.reverse
来源：http://we.chemitech.net.cn

C#:   list.Reverse();
来源：http://gd.huixiangedu.cn

[D12] 查找元素下标
来源：http://pj.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://zb.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ie.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hw.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vz.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nr.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://zw.521024.cn

Ruby: arr.index(x)
来源：http://rn.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://xf.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://zg.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://co.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wa.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://ox.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://kb.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rb.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ud.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nh.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sy.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://kp.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gq.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pt.521024.cn

JS:   arr.map(x => x * 2)
来源：http://hi.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://gi.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zh.shxzskj.cn

Go:   // 手写循环
来源：http://jf.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wb.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zd.szsharing.cn

[D15] 去重
来源：http://et.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jh.gzmigu.cn

PHP:  array_unique($arr);
来源：http://xp.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://xz.nicolike.cn

TS:   [...new Set(arr)]
来源：http://vr.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gb.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bh.asd995.cn

Ruby: arr.uniq
来源：http://gj.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://el.bjjhwx.cn

[D16] 求和与平均值
来源：http://yb.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wp.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ys.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://my.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ti.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ym.haigaiapp.cn

Go:   // 手写循环累加
来源：http://uo.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sf.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://ef.521024.cn

[D17] 最大值与最小值
来源：http://zz.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://pg.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://sh.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ex.szxytkj.cn

TS:   Math.max(...arr);
来源：http://se.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tv.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rv.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://pf.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://pp.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://ky.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gw.521024.cn

PHP:  array_merge(...$nested);
来源：http://pp.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dv.521024.cn

TS:   nested.flat();
来源：http://tu.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xa.newstarts.cn

Go:   // 手写双层循环
来源：http://nh.newstarts.cn

Ruby: nested.flatten
来源：http://tw.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tv.huixinmuqiang.cn


<!-- 参考信息 -->