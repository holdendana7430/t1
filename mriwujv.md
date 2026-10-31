代发 wailian999

PHP:  $a && $b || !$c
来源：http://pb.jianghongdianzi.cn

JS:   a && b || !c
来源：http://zy.jianghongdianzi.cn

TS:   a && b || !c
来源：http://ls.hnjuh.cn

Java: a && b || !c
来源：http://mn.hahajie.cn

Go:   a && b || !c
来源：http://gv.colortex.cn

Ruby: a && b || !c
来源：http://rg.nicolike.cn

C#:   a && b || !c
来源：http://fw.lnxyls.cn

[B16] 卫语句：不满足条件提前返回
来源：http://nz.huixiangedu.cn

Py:   if not data: return
来源：http://fv.asd995.cn

PHP:  if (!$data) { return; }
来源：http://tx.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://gg.bookmarksfly.cn

TS:   if (!data) return;
来源：http://du.lnxyls.cn

Java: if (data == null) return;
来源：http://ft.asd995.cn

Go:   if data == nil { return }
来源：http://fj.shxzukj.cn

Ruby: return if data.nil?
来源：http://zb.newstarts.cn

C#:   if (data == null) return;
来源：http://pd.muxihuayi.cn

================================================================================
来源：http://tb.panjiajie.cn

C. 函数与作用域
来源：http://dv.bjjhwx.cn

================================================================================
来源：http://kk.jctech888.com.cn

[C01] 定义函数
来源：http://jx.nicolike.cn

Py:   def add(a, b): return a + b
来源：http://vz.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gp.hahajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://aa.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jd.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xg.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bh.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ap.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rv.szsharing.cn

[C02] 默认参数
来源：http://nu.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://ty.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://by.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://xq.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://to.bookmarksfly.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ev.huixinmuqiang.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zh.szxytkj.cn

Ruby: def greet(name = "World") = name
来源：http://qk.huixinmuqiang.cn

C#:   string Greet(string name = "World") => name;
来源：http://cy.hahajie.cn

[C03] 可变参数
来源：http://jr.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ea.521024.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wq.chemitech.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gd.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xo.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fm.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rw.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://wi.9csxet.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fa.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://mj.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ch.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eq.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rc.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xv.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://zb.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://hu.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://ou.521024.cn

C#:   f(a: 1, b: 2)
来源：http://wz.muxihuayi.cn

[C05] 返回多个值
来源：http://bc.yuntaijiaju.cn

Py:   return a, b
来源：http://fj.newstarts.cn

PHP:  return [$a, $b];
来源：http://mq.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qm.lnxyls.cn

TS:   return { a, b };
来源：http://vk.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zm.chemitech.net.cn

Go:   return a, b
来源：http://ls.chemitech.net.cn

Ruby: return a, b
来源：http://cu.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://yw.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://re.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://tp.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://os.shtwfgs.cn

JS:   const square = x => x * x;
来源：http://ga.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://il.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://it.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ba.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://no.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sd.bjjhwx.cn

[C07] 把函数作为参数传入
来源：http://is.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mm.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ox.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://au.szxytkj.cn

TS:   arr.map(String)
来源：http://gk.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mz.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qc.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://bs.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ke.shtwfgs.cn

[C08] 闭包
来源：http://jw.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ed.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pk.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://is.nicolike.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ug.nszjky.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lo.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tp.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qj.yuexingan06.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://or.wgjwhj.cn

[C09] 递归
来源：http://ni.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lb.shxzukj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rg.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tn.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rg.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qj.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rw.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xb.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vt.yuexingan06.cn

[C10] 变量作用域
来源：http://dm.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rt.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ax.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vc.chemitech.net.cn

TS:   同 JS
来源：http://yw.hahajie.cn

Java: 方法内为块级作用域
来源：http://ip.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://eu.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://og.huixinmuqiang.cn

C#:   块级作用域
来源：http://gj.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://po.jianghongdianzi.cn

Py:   from module import func
来源：http://ew.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ac.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://he.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ys.haigaiapp.cn

Java: import java.util.List;
来源：http://bf.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pm.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ad.yuntaijiaju.cn

C#:   using System.Text;
来源：http://hj.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://js.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://th.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://hs.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://we.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://vb.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hy.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://nx.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://gh.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sm.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://of.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ej.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ll.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ci.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zq.9csxet.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pw.gzmigu.cn

Go:   func add(a, b int) int
来源：http://cy.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aj.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qj.colortex.cn

[C14] 泛型函数
来源：http://it.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xz.9csxet.cn

PHP:  // 无泛型
来源：http://hf.newstarts.cn

JS:   // 无泛型
来源：http://ai.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qs.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hg.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dj.szxytkj.cn

Ruby: # 无泛型
来源：http://so.huanxung.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gc.521024.cn

[C15] 解构 / 展开参数
来源：http://pk.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ba.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://kp.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pz.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tc.jctech888.com.cn

Java: // 无解构
来源：http://lv.jianghongdianzi.cn

Go:   // 无解构
来源：http://ma.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://kj.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://jj.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://cg.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jl.muxihuayi.cn

PHP:  // 无重载
来源：http://gy.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://es.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://cp.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gt.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://rn.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://oc.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gx.panjiajie.cn

================================================================================
来源：http://dg.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://wr.521024.cn

================================================================================
来源：http://ly.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://hd.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://td.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vx.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hr.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fo.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ye.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ib.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://qy.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zm.szsharing.cn

[D02] 追加元素到末尾
来源：http://hf.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xc.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oy.gzmigu.cn

JS:   arr.push(4);
来源：http://td.shxzukj.cn

TS:   arr.push(4);
来源：http://sm.muxihuayi.cn

Java: list.add(4);
来源：http://ts.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ut.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://qj.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://rm.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://bv.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://tg.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tt.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cb.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://zq.yuexingan06.cn

Java: list.add(0, 0);
来源：http://fs.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kk.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lk.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://et.huanxung.cn

[D04] 删除元素
来源：http://tw.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zx.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nd.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xm.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://eh.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xa.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aw.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qf.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ya.bjjhwx.cn

[D05] 访问与修改元素
来源：http://jz.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mv.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://da.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dl.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://rk.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://nc.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://he.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ce.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gn.bookmarksfly.cn

[D06] 数组长度
来源：http://pr.nszjky.cn

Py:   len(arr)
来源：http://mp.muxihuayi.cn

PHP:  count($arr);
来源：http://fx.panjiajie.cn

JS:   arr.length
来源：http://dg.panjiajie.cn

TS:   arr.length
来源：http://qc.szsharing.cn

Java: list.size();
来源：http://db.szsharing.cn

Go:   len(arr)
来源：http://en.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://kd.nicolike.cn

C#:   list.Count;
来源：http://dj.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://bu.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bw.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vy.521024.cn

JS:   arr.slice(1, 4);
来源：http://iy.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://kb.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://ud.shxzskj.cn

Go:   arr[1:4]
来源：http://jl.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://sh.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://hw.szxytkj.cn

[D08] 合并两个数组
来源：http://dk.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://ob.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://ae.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dd.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://hf.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nk.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://zl.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://bw.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://ef.newstarts.cn

[D09] 排序（升序）
来源：http://mk.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://yy.newstarts.cn

PHP:  sort($arr);
来源：http://ds.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ll.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xr.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vw.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fu.bookmarksfly.cn

Ruby: arr.sort
来源：http://mu.bjjhwx.cn

C#:   list.Sort();
来源：http://oi.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qo.shxzukj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ht.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wo.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ii.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://od.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kf.shtwfgs.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wc.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hr.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kr.bjjhwx.cn

[D11] 反转数组
来源：http://wo.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oh.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://yj.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rl.nicolike.cn

TS:   [...arr].reverse();
来源：http://iw.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://fy.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://ha.huixiangedu.cn

Ruby: arr.reverse
来源：http://xt.haigaiapp.cn

C#:   list.Reverse();
来源：http://eb.chemitech.net.cn

[D12] 查找元素下标
来源：http://lu.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://op.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dd.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pn.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dc.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wy.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://nr.yuexingan06.cn

Ruby: arr.index(x)
来源：http://qd.nicolike.cn

C#:   list.IndexOf(x);
来源：http://ce.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://gj.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nc.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vr.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://wc.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://rz.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oc.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tu.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fc.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zo.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://fu.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pq.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qx.9csxet.cn

JS:   arr.map(x => x * 2)
来源：http://pq.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://mn.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kc.huanxung.cn

Go:   // 手写循环
来源：http://zg.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zf.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mb.huixiangedu.cn

[D15] 去重
来源：http://um.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yk.hahajie.cn

PHP:  array_unique($arr);
来源：http://xh.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://sw.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://mm.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ri.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bz.shxzukj.cn

Ruby: arr.uniq
来源：http://hk.yuexingan06.cn


<!-- 参考信息 -->