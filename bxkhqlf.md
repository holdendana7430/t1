代发 wailian999

Go:   a && b || !c
来源：http://bb.9csxet.cn

Ruby: a && b || !c
来源：http://wk.lnxyls.cn

C#:   a && b || !c
来源：http://xd.wgjwhj.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mi.panjiajie.cn

Py:   if not data: return
来源：http://rj.hnjuh.cn

PHP:  if (!$data) { return; }
来源：http://dn.yuntaijiaju.cn

JS:   if (!data) return;
来源：http://em.shxzukj.cn

TS:   if (!data) return;
来源：http://ih.hahajie.cn

Java: if (data == null) return;
来源：http://yq.lnxyls.cn

Go:   if data == nil { return }
来源：http://kr.shxzskj.cn

Ruby: return if data.nil?
来源：http://bk.gzmigu.cn

C#:   if (data == null) return;
来源：http://pq.chemitech.net.cn

================================================================================
来源：http://np.521024.cn

C. 函数与作用域
来源：http://kf.shtwfgs.cn

================================================================================
来源：http://cg.haigaiapp.cn

[C01] 定义函数
来源：http://np.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://wc.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://el.chemitech.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://br.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dz.hnjuh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hk.shxzskj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yr.shxzukj.cn

Ruby: def add(a, b); a + b; end
来源：http://wj.huixinmuqiang.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cl.shxzukj.cn

[C02] 默认参数
来源：http://da.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://cl.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bq.panjiajie.cn

JS:   function greet(name = "World") { return name; }
来源：http://si.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mj.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ng.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kz.szsharing.cn

Ruby: def greet(name = "World") = name
来源：http://hz.521024.cn

C#:   string Greet(string name = "World") => name;
来源：http://fh.9csxet.cn

[C03] 可变参数
来源：http://wk.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://ik.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xa.panjiajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fq.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tp.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dw.huixinmuqiang.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kv.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ir.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qz.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://gx.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ff.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lt.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yf.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hp.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://du.szxytkj.cn

Go:   // 无：用配置结构体参数
来源：http://rk.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://tf.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://po.yuexingan06.cn

[C05] 返回多个值
来源：http://pe.jctech888.com.cn

Py:   return a, b
来源：http://ta.colortex.cn

PHP:  return [$a, $b];
来源：http://yc.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xx.shtwfgs.cn

TS:   return { a, b };
来源：http://um.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yi.shxzukj.cn

Go:   return a, b
来源：http://yy.huanxung.cn

Ruby: return a, b
来源：http://hw.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://op.szxytkj.cn

[C06] 匿名函数 / lambda
来源：http://gv.hahajie.cn

Py:   square = lambda x: x * x
来源：http://ud.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tt.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://js.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://tc.newstarts.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dg.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oj.hahajie.cn

Ruby: square = ->(x) { x * x }
来源：http://lb.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cn.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://bq.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yj.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ik.colortex.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ms.hahajie.cn

TS:   arr.map(String)
来源：http://yj.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dx.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fb.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://nt.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xq.colortex.cn

[C08] 闭包
来源：http://az.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wl.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jj.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vl.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jy.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qv.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pu.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ja.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uw.bookmarksfly.cn

[C09] 递归
来源：http://nm.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bv.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rk.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qj.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rr.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ms.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://je.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://en.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yq.asd995.cn

[C10] 变量作用域
来源：http://cj.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rw.huixiangedu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qw.shtwfgs.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ge.shxzukj.cn

TS:   同 JS
来源：http://aq.asd995.cn

Java: 方法内为块级作用域
来源：http://fc.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://sp.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rd.bookmarksfly.cn

C#:   块级作用域
来源：http://ja.asd995.cn

[C11] 模块导入与导出
来源：http://hh.9csxet.cn

Py:   from module import func
来源：http://ru.haigaiapp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jy.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pw.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://st.panjiajie.cn

Java: import java.util.List;
来源：http://rk.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uw.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://lr.huanxung.cn

C#:   using System.Text;
来源：http://nt.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://qy.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://mh.yuntaijiaju.cn

PHP:  (function () { echo "run"; })();
来源：http://sg.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://as.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://wm.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rm.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ot.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ce.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qc.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://le.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ms.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kd.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gu.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vt.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cd.colortex.cn

Go:   func add(a, b int) int
来源：http://nq.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kx.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ao.szsharing.cn

[C14] 泛型函数
来源：http://gq.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xs.521024.cn

PHP:  // 无泛型
来源：http://gu.bookmarksfly.cn

JS:   // 无泛型
来源：http://dw.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xq.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://za.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ny.nszjky.cn

Ruby: # 无泛型
来源：http://pr.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uc.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://bi.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sg.hnjuh.cn

PHP:  [$a, $b] = $pair;
来源：http://kr.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pt.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uh.9csxet.cn

Java: // 无解构
来源：http://um.huixinmuqiang.cn

Go:   // 无解构
来源：http://jf.asd995.cn

Ruby: a, b = pair
来源：http://gh.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://fx.newstarts.cn

[C16] 函数 / 方法重载
来源：http://pt.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ad.huixinmuqiang.cn

PHP:  // 无重载
来源：http://cd.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bo.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://dd.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hy.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://kf.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://wq.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ij.lnxyls.cn

================================================================================
来源：http://jj.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://vo.bookmarksfly.cn

================================================================================
来源：http://na.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://ov.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pj.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://un.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://es.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lt.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cs.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://uv.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://kv.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zs.shxzskj.cn

[D02] 追加元素到末尾
来源：http://pe.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uw.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oy.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://gz.chemitech.net.cn

TS:   arr.push(4);
来源：http://pn.9csxet.cn

Java: list.add(4);
来源：http://pz.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://rp.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://vf.colortex.cn

C#:   list.Add(4);
来源：http://kp.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ke.521024.cn

Py:   arr.insert(0, 0)
来源：http://qd.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://in.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sl.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://ul.haigaiapp.cn

Java: list.add(0, 0);
来源：http://tw.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ps.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jd.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://sf.bjjhwx.cn

[D04] 删除元素
来源：http://qx.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gl.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cy.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xb.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://ur.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ji.nicolike.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jb.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ou.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cm.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://dy.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fz.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kj.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hk.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://hw.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ac.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://mh.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bm.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cu.huixiangedu.cn

[D06] 数组长度
来源：http://nn.shxzukj.cn

Py:   len(arr)
来源：http://lq.chemitech.net.cn

PHP:  count($arr);
来源：http://sd.newstarts.cn

JS:   arr.length
来源：http://hk.bookmarksfly.cn

TS:   arr.length
来源：http://cd.nicolike.cn

Java: list.size();
来源：http://yn.muxihuayi.cn

Go:   len(arr)
来源：http://ro.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://oc.jianghongdianzi.cn

C#:   list.Count;
来源：http://qx.szsharing.cn

[D07] 切片 / 取子数组
来源：http://cz.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ev.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jw.colortex.cn

JS:   arr.slice(1, 4);
来源：http://la.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://xq.hahajie.cn

Java: list.subList(1, 4);
来源：http://rp.nicolike.cn

Go:   arr[1:4]
来源：http://ih.gzmigu.cn

Ruby: arr[1, 3]
来源：http://rr.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://bi.hahajie.cn

[D08] 合并两个数组
来源：http://bq.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://bb.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://ci.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ht.hahajie.cn

TS:   [...a, ...b];
来源：http://dy.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jd.szsharing.cn

Go:   append(a, b...)
来源：http://qb.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://ox.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://rt.szxytkj.cn

[D09] 排序（升序）
来源：http://he.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://dg.haigaiapp.cn

PHP:  sort($arr);
来源：http://lu.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cx.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tm.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dz.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yk.yuexingan06.cn

Ruby: arr.sort
来源：http://kf.asd995.cn

C#:   list.Sort();
来源：http://fu.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://je.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pd.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tb.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xp.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rk.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oj.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ao.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kt.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bw.jianghongdianzi.cn

[D11] 反转数组
来源：http://gt.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://db.newstarts.cn

PHP:  array_reverse($arr);
来源：http://pu.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ms.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://aq.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://km.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://fy.gzmigu.cn

Ruby: arr.reverse
来源：http://ek.9csxet.cn

C#:   list.Reverse();
来源：http://ar.gzmigu.cn

[D12] 查找元素下标
来源：http://hg.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://pd.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dv.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://td.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iq.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://na.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://mx.muxihuayi.cn

Ruby: arr.index(x)
来源：http://lv.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://ni.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://pp.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ty.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uu.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://bi.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://fq.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ir.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mq.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eh.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qh.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://yd.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tq.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bu.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://tc.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://xs.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dd.wgjwhj.cn

Go:   // 手写循环
来源：http://hs.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pg.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bv.shtwfgs.cn

[D15] 去重
来源：http://wg.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hk.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://jd.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://ke.9csxet.cn

TS:   [...new Set(arr)]
来源：http://by.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aw.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bq.shxzukj.cn

Ruby: arr.uniq
来源：http://io.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://rf.shxzukj.cn

[D16] 求和与平均值
来源：http://zq.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eg.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nl.jctech888.com.cn


<!-- 参考信息 -->