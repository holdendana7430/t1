代发 wailian999

================================================================================
来源：http://fx.newstarts.cn

C. 函数与作用域
来源：http://fd.521024.cn

================================================================================
来源：http://cw.lnxyls.cn

[C01] 定义函数
来源：http://oz.chemitech.net.cn

Py:   def add(a, b): return a + b
来源：http://of.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mc.asd995.cn

JS:   function add(a, b) { return a + b; }
来源：http://nz.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qn.yuntaijiaju.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ai.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ea.wgjwhj.cn

Ruby: def add(a, b); a + b; end
来源：http://iu.521024.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mt.newstarts.cn

[C02] 默认参数
来源：http://du.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://wk.szsharing.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tz.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ei.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cx.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rt.shxzskj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pu.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://oj.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://fx.wgjwhj.cn

[C03] 可变参数
来源：http://vn.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://ac.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vy.521024.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pi.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lo.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://la.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ks.jctech888.com.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kb.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://il.colortex.cn

[C04] 命名参数 / 关键字参数
来源：http://lc.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vg.chemitech.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qv.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hp.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tz.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://pk.haigaiapp.cn

Go:   // 无：用配置结构体参数
来源：http://kd.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://vo.hahajie.cn

C#:   f(a: 1, b: 2)
来源：http://zq.9csxet.cn

[C05] 返回多个值
来源：http://mo.chemitech.net.cn

Py:   return a, b
来源：http://fo.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://oj.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://do.yuntaijiaju.cn

TS:   return { a, b };
来源：http://ue.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://py.shxzskj.cn

Go:   return a, b
来源：http://ph.newstarts.cn

Ruby: return a, b
来源：http://tl.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://dz.colortex.cn

[C06] 匿名函数 / lambda
来源：http://jk.hahajie.cn

Py:   square = lambda x: x * x
来源：http://oq.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qg.521024.cn

JS:   const square = x => x * x;
来源：http://vi.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://bi.hnjuh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ci.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hq.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://en.colortex.cn

C#:   Func<int, int> square = x => x * x;
来源：http://my.szsharing.cn

[C07] 把函数作为参数传入
来源：http://zm.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mc.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gg.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xc.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://rj.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kl.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qc.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://id.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qj.huanxung.cn

[C08] 闭包
来源：http://wj.wgjwhj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zl.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vd.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yc.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bs.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mc.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uy.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cg.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xi.lnxyls.cn

[C09] 递归
来源：http://iy.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xi.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hr.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ol.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yk.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://en.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tb.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qz.szxytkj.cn

[C10] 变量作用域
来源：http://kh.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ta.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gh.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uz.szxytkj.cn

TS:   同 JS
来源：http://cx.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://sr.asd995.cn

Go:   花括号块级作用域
来源：http://gd.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://is.9csxet.cn

C#:   块级作用域
来源：http://cz.nicolike.cn

[C11] 模块导入与导出
来源：http://ur.hahajie.cn

Py:   from module import func
来源：http://xn.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kq.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mo.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xu.muxihuayi.cn

Java: import java.util.List;
来源：http://go.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ds.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://cm.wgjwhj.cn

C#:   using System.Text;
来源：http://fo.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://sw.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://tb.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://dk.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://cu.bookmarksfly.cn

TS:   (() => { console.log("run"); })();
来源：http://qs.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://um.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://hr.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://ty.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fr.521024.cn

[C13] 类型声明 / 类型注解
来源：http://bq.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ls.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ui.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ff.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cs.hahajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zb.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://iq.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cl.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ir.gzmigu.cn

[C14] 泛型函数
来源：http://bi.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ka.lnxyls.cn

PHP:  // 无泛型
来源：http://xv.bjjhwx.cn

JS:   // 无泛型
来源：http://rl.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vc.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fk.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zp.jctech888.com.cn

Ruby: # 无泛型
来源：http://ah.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wp.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://jb.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://li.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://ha.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gl.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://by.haigaiapp.cn

Java: // 无解构
来源：http://sc.huixiangedu.cn

Go:   // 无解构
来源：http://va.chemitech.net.cn

Ruby: a, b = pair
来源：http://gq.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://sk.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://tz.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cc.shxzskj.cn

PHP:  // 无重载
来源：http://ut.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xv.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://hj.bookmarksfly.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://is.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://fa.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://il.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qy.521024.cn

================================================================================
来源：http://ko.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://sc.haigaiapp.cn

================================================================================
来源：http://pn.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://jy.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://td.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zf.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://us.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ti.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://we.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://mn.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://je.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jd.szsharing.cn

[D02] 追加元素到末尾
来源：http://dx.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cv.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ax.wgjwhj.cn

JS:   arr.push(4);
来源：http://sy.yuexingan06.cn

TS:   arr.push(4);
来源：http://yk.newstarts.cn

Java: list.add(4);
来源：http://ur.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://oh.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://go.szxytkj.cn

C#:   list.Add(4);
来源：http://iu.hahajie.cn

[D03] 在指定位置插入元素
来源：http://wc.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://vy.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gm.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xu.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://rx.nszjky.cn

Java: list.add(0, 0);
来源：http://ef.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://br.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ny.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ah.9csxet.cn

[D04] 删除元素
来源：http://pq.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ue.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qj.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tk.521024.cn

TS:   arr.splice(0, 1);
来源：http://lo.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zh.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dl.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pz.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nn.chemitech.net.cn

[D05] 访问与修改元素
来源：http://mz.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dt.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hg.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dk.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://cf.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://yc.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://he.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ub.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ri.huanxung.cn

[D06] 数组长度
来源：http://lq.newstarts.cn

Py:   len(arr)
来源：http://ip.colortex.cn

PHP:  count($arr);
来源：http://mb.yuntaijiaju.cn

JS:   arr.length
来源：http://wz.bookmarksfly.cn

TS:   arr.length
来源：http://qu.yuexingan06.cn

Java: list.size();
来源：http://sm.nszjky.cn

Go:   len(arr)
来源：http://zl.hahajie.cn

Ruby: arr.length; arr.size
来源：http://jg.bjjhwx.cn

C#:   list.Count;
来源：http://ir.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://qe.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ly.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sp.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://vo.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://wn.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://tu.9csxet.cn

Go:   arr[1:4]
来源：http://zo.lnxyls.cn

Ruby: arr[1, 3]
来源：http://aw.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://wa.asd995.cn

[D08] 合并两个数组
来源：http://vn.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://hl.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://oq.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wn.lnxyls.cn

TS:   [...a, ...b];
来源：http://vp.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dw.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://bi.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://rl.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://xo.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://hn.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://an.huanxung.cn

PHP:  sort($arr);
来源：http://cg.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://az.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qm.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bp.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dv.chemitech.net.cn

Ruby: arr.sort
来源：http://fo.bjjhwx.cn

C#:   list.Sort();
来源：http://fl.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gd.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vg.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wy.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iz.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uc.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zq.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ij.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xv.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ta.lnxyls.cn

[D11] 反转数组
来源：http://hx.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://br.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://jd.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sm.gzmigu.cn

TS:   [...arr].reverse();
来源：http://ps.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://jv.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://hm.bjjhwx.cn

Ruby: arr.reverse
来源：http://xm.haigaiapp.cn

C#:   list.Reverse();
来源：http://iy.gzmigu.cn

[D12] 查找元素下标
来源：http://zw.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://kr.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hc.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cw.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pz.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ep.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://pp.nszjky.cn

Ruby: arr.index(x)
来源：http://si.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://zd.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://jl.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fc.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zt.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://nm.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://lu.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pm.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jv.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cc.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mm.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://kd.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://al.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ba.521024.cn

JS:   arr.map(x => x * 2)
来源：http://ig.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://kg.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iu.9csxet.cn

Go:   // 手写循环
来源：http://wl.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qe.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qc.chemitech.net.cn

[D15] 去重
来源：http://gv.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lp.szsharing.cn

PHP:  array_unique($arr);
来源：http://bc.nszjky.cn

JS:   [...new Set(arr)]
来源：http://vo.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://ye.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://je.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://by.hnjuh.cn

Ruby: arr.uniq
来源：http://fa.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://ni.9csxet.cn

[D16] 求和与平均值
来源：http://ev.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lr.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qm.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gy.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tv.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rl.nszjky.cn

Go:   // 手写循环累加
来源：http://ju.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.521024.cn

C#:   list.Sum();  list.Average()
来源：http://uf.chemitech.net.cn

[D17] 最大值与最小值
来源：http://fk.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://rh.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://dl.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kn.521024.cn

TS:   Math.max(...arr);
来源：http://uy.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wf.521024.cn


<!-- 参考信息 -->