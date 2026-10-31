代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gh.yuexingan06.cn

Java: x instanceof Number
来源：http://jl.huixinmuqiang.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wt.hnjuh.cn

Ruby: x.is_a?(Numeric)
来源：http://ot.wgjwhj.cn

C#:   x is int or double or decimal
来源：http://rf.chemitech.net.cn

[B14] 判断值是否在集合内
来源：http://hp.muxihuayi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ju.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ch.chemitech.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://mm.shxzskj.cn

TS:   [1, 2, 3].includes(x)
来源：http://nx.jctech888.com.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://mq.panjiajie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pt.huanxung.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yq.colortex.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qy.szsharing.cn

[B15] 布尔运算与取反
来源：http://qa.9csxet.cn

Py:   a and b or not c
来源：http://gw.shxzukj.cn

PHP:  $a && $b || !$c
来源：http://fp.wgjwhj.cn

JS:   a && b || !c
来源：http://ta.muxihuayi.cn

TS:   a && b || !c
来源：http://qe.9csxet.cn

Java: a && b || !c
来源：http://by.521024.cn

Go:   a && b || !c
来源：http://my.hnjuh.cn

Ruby: a && b || !c
来源：http://eb.jianghongdianzi.cn

C#:   a && b || !c
来源：http://cj.huixinmuqiang.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qy.hahajie.cn

Py:   if not data: return
来源：http://ko.shxzskj.cn

PHP:  if (!$data) { return; }
来源：http://xa.lnxyls.cn

JS:   if (!data) return;
来源：http://yb.shxzukj.cn

TS:   if (!data) return;
来源：http://ry.521024.cn

Java: if (data == null) return;
来源：http://gl.szxytkj.cn

Go:   if data == nil { return }
来源：http://ox.colortex.cn

Ruby: return if data.nil?
来源：http://xp.yuntaijiaju.cn

C#:   if (data == null) return;
来源：http://nn.shtwfgs.cn

================================================================================
来源：http://pu.panjiajie.cn

C. 函数与作用域
来源：http://cn.huixiangedu.cn

================================================================================
来源：http://hf.panjiajie.cn

[C01] 定义函数
来源：http://op.szxytkj.cn

Py:   def add(a, b): return a + b
来源：http://ns.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://um.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://nr.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jb.lnxyls.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://pk.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xo.haigaiapp.cn

Ruby: def add(a, b); a + b; end
来源：http://bq.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iz.huixinmuqiang.cn

[C02] 默认参数
来源：http://fw.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://fw.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pc.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://im.jianghongdianzi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xf.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ne.newstarts.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zl.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://no.colortex.cn

C#:   string Greet(string name = "World") => name;
来源：http://la.jctech888.com.cn

[C03] 可变参数
来源：http://pe.wgjwhj.cn

Py:   def total(*args): return sum(args)
来源：http://um.hnjuh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oz.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tp.shxzskj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://or.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://by.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fz.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gd.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qm.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://en.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uf.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uh.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ym.hahajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zp.nicolike.cn

Java: // 无：用 Builder 模式或 record
来源：http://ql.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://tl.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://tb.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://fe.hnjuh.cn

[C05] 返回多个值
来源：http://tu.haigaiapp.cn

Py:   return a, b
来源：http://mo.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://tj.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ye.9csxet.cn

TS:   return { a, b };
来源：http://zg.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cy.521024.cn

Go:   return a, b
来源：http://xj.chemitech.net.cn

Ruby: return a, b
来源：http://bf.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://ac.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://yb.nicolike.cn

Py:   square = lambda x: x * x
来源：http://sw.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vl.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://cy.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ga.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yv.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://am.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://yn.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uk.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://ma.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aj.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://by.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dy.colortex.cn

TS:   arr.map(String)
来源：http://wx.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ai.9csxet.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hj.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://ar.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://au.gzmigu.cn

[C08] 闭包
来源：http://jm.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gy.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cf.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jd.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uy.huanxung.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aa.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mi.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kc.nicolike.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tv.bjjhwx.cn

[C09] 递归
来源：http://hm.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zj.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vc.nicolike.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rb.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://od.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xj.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ma.szxytkj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yo.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gv.shtwfgs.cn

[C10] 变量作用域
来源：http://fh.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uj.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hi.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hw.jianghongdianzi.cn

TS:   同 JS
来源：http://xa.gzmigu.cn

Java: 方法内为块级作用域
来源：http://gm.hahajie.cn

Go:   花括号块级作用域
来源：http://lp.shxzskj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ir.gzmigu.cn

C#:   块级作用域
来源：http://sr.haigaiapp.cn

[C11] 模块导入与导出
来源：http://dx.9csxet.cn

Py:   from module import func
来源：http://ve.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ik.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sc.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ib.yuntaijiaju.cn

Java: import java.util.List;
来源：http://hg.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kz.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://jl.asd995.cn

C#:   using System.Text;
来源：http://ef.521024.cn

[C12] 立即执行函数 IIFE
来源：http://ys.521024.cn

Py:   (lambda: print("run"))()
来源：http://oe.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://mf.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://bv.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://hu.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ak.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ab.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://rp.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://dz.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://xt.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nk.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ow.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qq.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fg.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hl.szsharing.cn

Go:   func add(a, b int) int
来源：http://nd.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qg.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jh.huixinmuqiang.cn

[C14] 泛型函数
来源：http://lz.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qj.gzmigu.cn

PHP:  // 无泛型
来源：http://my.panjiajie.cn

JS:   // 无泛型
来源：http://cd.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hu.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://px.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pl.521024.cn

Ruby: # 无泛型
来源：http://it.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mi.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://he.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jy.nicolike.cn

PHP:  [$a, $b] = $pair;
来源：http://dt.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bo.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://aj.huixiangedu.cn

Java: // 无解构
来源：http://hy.shtwfgs.cn

Go:   // 无解构
来源：http://go.nszjky.cn

Ruby: a, b = pair
来源：http://rq.colortex.cn

C#:   var (a, b) = pair;
来源：http://cu.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://gn.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gv.chemitech.net.cn

PHP:  // 无重载
来源：http://ea.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eo.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://cm.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xj.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://ec.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://tk.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fw.nszjky.cn

================================================================================
来源：http://vo.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://yg.yuntaijiaju.cn

================================================================================
来源：http://tq.panjiajie.cn

[D01] 创建数组 / 列表
来源：http://xu.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ti.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gq.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jp.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pw.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fr.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://lb.muxihuayi.cn

Ruby: arr = [1, 2, 3]
来源：http://kb.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ff.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://ij.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tl.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kp.szsharing.cn

JS:   arr.push(4);
来源：http://we.szxytkj.cn

TS:   arr.push(4);
来源：http://dh.hahajie.cn

Java: list.add(4);
来源：http://li.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://uh.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://qe.wgjwhj.cn

C#:   list.Add(4);
来源：http://hi.hahajie.cn

[D03] 在指定位置插入元素
来源：http://wb.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://xs.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tl.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ep.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://hi.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://gx.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kq.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wd.asd995.cn

C#:   list.Insert(0, 0);
来源：http://tf.bjjhwx.cn

[D04] 删除元素
来源：http://az.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nd.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pf.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uo.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://ql.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uo.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lp.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hm.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pd.hnjuh.cn

[D05] 访问与修改元素
来源：http://af.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ae.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uy.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vb.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://zp.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://et.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://gh.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kd.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://np.gzmigu.cn

[D06] 数组长度
来源：http://tm.muxihuayi.cn

Py:   len(arr)
来源：http://py.jctech888.com.cn

PHP:  count($arr);
来源：http://lj.nszjky.cn

JS:   arr.length
来源：http://vh.jianghongdianzi.cn

TS:   arr.length
来源：http://uq.szxytkj.cn

Java: list.size();
来源：http://ht.9csxet.cn

Go:   len(arr)
来源：http://tj.newstarts.cn

Ruby: arr.length; arr.size
来源：http://gr.shxzukj.cn

C#:   list.Count;
来源：http://jw.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://qd.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tl.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bi.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://eq.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://ur.shxzukj.cn

Java: list.subList(1, 4);
来源：http://tl.yuexingan06.cn

Go:   arr[1:4]
来源：http://at.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://pz.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://xw.gzmigu.cn

[D08] 合并两个数组
来源：http://is.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://ol.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://zh.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qv.nicolike.cn

TS:   [...a, ...b];
来源：http://qn.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zk.haigaiapp.cn

Go:   append(a, b...)
来源：http://yp.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://oc.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://zl.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://ll.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://yz.bjjhwx.cn

PHP:  sort($arr);
来源：http://ez.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hc.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://we.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ea.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eq.lnxyls.cn

Ruby: arr.sort
来源：http://xr.szxytkj.cn

C#:   list.Sort();
来源：http://jo.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qk.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hn.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wt.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vu.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vb.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zf.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sy.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nf.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hq.panjiajie.cn

[D11] 反转数组
来源：http://ua.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yx.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://mi.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oj.gzmigu.cn

TS:   [...arr].reverse();
来源：http://vw.gzmigu.cn

Java: Collections.reverse(list);
来源：http://lw.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://kf.haigaiapp.cn

Ruby: arr.reverse
来源：http://ba.bjjhwx.cn

C#:   list.Reverse();
来源：http://aq.asd995.cn

[D12] 查找元素下标
来源：http://wy.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://rl.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dq.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qi.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bn.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rd.521024.cn

Go:   slices.Index(arr, x)
来源：http://nl.panjiajie.cn

Ruby: arr.index(x)
来源：http://gm.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://zk.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://jp.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ex.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iz.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://hn.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://do.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sm.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xw.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gt.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kp.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://pr.newstarts.cn


<!-- 参考信息 -->