代发 wailian999

C#:   x is int or double or decimal
来源：http://rh.gzmigu.cn

[B14] 判断值是否在集合内
来源：http://ph.colortex.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://no.shxzskj.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ug.huixiangedu.cn

JS:   [1, 2, 3].includes(x)
来源：http://bm.colortex.cn

TS:   [1, 2, 3].includes(x)
来源：http://wj.521024.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tw.bjjhwx.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ak.haigaiapp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jc.asd995.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ol.haigaiapp.cn

[B15] 布尔运算与取反
来源：http://ts.haigaiapp.cn

Py:   a and b or not c
来源：http://uz.bjjhwx.cn

PHP:  $a && $b || !$c
来源：http://ah.jctech888.com.cn

JS:   a && b || !c
来源：http://it.yuexingan06.cn

TS:   a && b || !c
来源：http://qy.521024.cn

Java: a && b || !c
来源：http://ho.huixinmuqiang.cn

Go:   a && b || !c
来源：http://kd.colortex.cn

Ruby: a && b || !c
来源：http://ut.shtwfgs.cn

C#:   a && b || !c
来源：http://sq.huixiangedu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fg.hahajie.cn

Py:   if not data: return
来源：http://ma.hahajie.cn

PHP:  if (!$data) { return; }
来源：http://st.huixinmuqiang.cn

JS:   if (!data) return;
来源：http://ju.jctech888.com.cn

TS:   if (!data) return;
来源：http://gl.bjjhwx.cn

Java: if (data == null) return;
来源：http://wx.shtwfgs.cn

Go:   if data == nil { return }
来源：http://kd.yuntaijiaju.cn

Ruby: return if data.nil?
来源：http://rs.nicolike.cn

C#:   if (data == null) return;
来源：http://ng.yuntaijiaju.cn

================================================================================
来源：http://xs.hnjuh.cn

C. 函数与作用域
来源：http://ii.haigaiapp.cn

================================================================================
来源：http://tr.huixiangedu.cn

[C01] 定义函数
来源：http://wf.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://pz.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ku.huanxung.cn

JS:   function add(a, b) { return a + b; }
来源：http://wf.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lc.nszjky.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ao.yuexingan06.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xw.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://gp.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yi.colortex.cn

[C02] 默认参数
来源：http://hi.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://uj.nicolike.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://nj.szsharing.cn

JS:   function greet(name = "World") { return name; }
来源：http://ag.bjjhwx.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://td.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jn.haigaiapp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sr.colortex.cn

Ruby: def greet(name = "World") = name
来源：http://jb.jctech888.com.cn

C#:   string Greet(string name = "World") => name;
来源：http://yk.521024.cn

[C03] 可变参数
来源：http://et.muxihuayi.cn

Py:   def total(*args): return sum(args)
来源：http://ff.wgjwhj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eh.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qu.wgjwhj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://py.bjjhwx.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jt.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fg.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xv.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jw.yuexingan06.cn

[C04] 命名参数 / 关键字参数
来源：http://pi.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lo.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nr.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ak.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kd.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://ns.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://cz.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://yj.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://vd.yuntaijiaju.cn

[C05] 返回多个值
来源：http://xl.shtwfgs.cn

Py:   return a, b
来源：http://pt.shxzskj.cn

PHP:  return [$a, $b];
来源：http://ck.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sf.muxihuayi.cn

TS:   return { a, b };
来源：http://bs.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qf.jctech888.com.cn

Go:   return a, b
来源：http://ir.bookmarksfly.cn

Ruby: return a, b
来源：http://ey.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://vr.newstarts.cn

[C06] 匿名函数 / lambda
来源：http://rh.asd995.cn

Py:   square = lambda x: x * x
来源：http://bt.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://la.huanxung.cn

JS:   const square = x => x * x;
来源：http://no.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://gc.yuexingan06.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jv.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nl.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://xr.haigaiapp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://to.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://tb.jianghongdianzi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rm.wgjwhj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zy.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bh.nicolike.cn

TS:   arr.map(String)
来源：http://tk.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zl.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ri.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://ve.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kg.lnxyls.cn

[C08] 闭包
来源：http://uq.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dk.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cx.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://md.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gc.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tw.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ej.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yp.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uo.asd995.cn

[C09] 递归
来源：http://iw.hahajie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zm.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://is.huixiangedu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fs.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ee.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://br.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lt.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rs.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ek.shtwfgs.cn

[C10] 变量作用域
来源：http://jx.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sz.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wx.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zq.bookmarksfly.cn

TS:   同 JS
来源：http://xu.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://oh.nicolike.cn

Go:   花括号块级作用域
来源：http://yc.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ec.nicolike.cn

C#:   块级作用域
来源：http://eo.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://ks.chemitech.net.cn

Py:   from module import func
来源：http://qq.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fz.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qo.szxytkj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dw.hahajie.cn

Java: import java.util.List;
来源：http://ue.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mg.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://nr.gzmigu.cn

C#:   using System.Text;
来源：http://wo.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://aw.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://ut.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://ls.gzmigu.cn

JS:   (() => { console.log("run"); })();
来源：http://kl.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://nm.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qx.bookmarksfly.cn

Go:   func() { fmt.Println("run") }()
来源：http://nn.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://vo.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uj.nicolike.cn

[C13] 类型声明 / 类型注解
来源：http://nu.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vz.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pl.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ug.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kx.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qj.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://il.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tp.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kv.shtwfgs.cn

[C14] 泛型函数
来源：http://ot.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bt.colortex.cn

PHP:  // 无泛型
来源：http://ri.colortex.cn

JS:   // 无泛型
来源：http://lk.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wb.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aa.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://id.jctech888.com.cn

Ruby: # 无泛型
来源：http://zw.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cw.huanxung.cn

[C15] 解构 / 展开参数
来源：http://bp.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ss.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://pa.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nb.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oo.haigaiapp.cn

Java: // 无解构
来源：http://pq.huixinmuqiang.cn

Go:   // 无解构
来源：http://at.shtwfgs.cn

Ruby: a, b = pair
来源：http://oc.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://ex.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://ci.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nh.jctech888.com.cn

PHP:  // 无重载
来源：http://dg.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lz.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://yz.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sd.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://lg.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://da.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zc.haigaiapp.cn

================================================================================
来源：http://ek.asd995.cn

D. 数组 / 列表 / 集合
来源：http://na.hahajie.cn

================================================================================
来源：http://fp.newstarts.cn

[D01] 创建数组 / 列表
来源：http://bo.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://np.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ji.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sy.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gq.panjiajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jm.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://ef.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://ft.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hu.9csxet.cn

[D02] 追加元素到末尾
来源：http://nf.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aq.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xz.hahajie.cn

JS:   arr.push(4);
来源：http://pl.asd995.cn

TS:   arr.push(4);
来源：http://zf.9csxet.cn

Java: list.add(4);
来源：http://hq.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://cu.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ue.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://ph.huixiangedu.cn

[D03] 在指定位置插入元素
来源：http://dc.colortex.cn

Py:   arr.insert(0, 0)
来源：http://bz.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://im.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://er.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://os.521024.cn

Java: list.add(0, 0);
来源：http://zq.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ee.yuexingan06.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zu.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://td.huixiangedu.cn

[D04] 删除元素
来源：http://lf.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nr.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://de.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://em.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://pq.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lj.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ac.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mq.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pq.hahajie.cn

[D05] 访问与修改元素
来源：http://wj.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ov.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://et.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pl.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://rx.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://yf.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://lb.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eo.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aw.9csxet.cn

[D06] 数组长度
来源：http://zj.huanxung.cn

Py:   len(arr)
来源：http://kc.yuexingan06.cn

PHP:  count($arr);
来源：http://rm.nszjky.cn

JS:   arr.length
来源：http://lx.szxytkj.cn

TS:   arr.length
来源：http://rb.gzmigu.cn

Java: list.size();
来源：http://aw.asd995.cn

Go:   len(arr)
来源：http://ez.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://rc.hnjuh.cn

C#:   list.Count;
来源：http://es.colortex.cn

[D07] 切片 / 取子数组
来源：http://sh.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iz.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kb.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://qs.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://gm.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://ml.nszjky.cn

Go:   arr[1:4]
来源：http://px.shxzskj.cn

Ruby: arr[1, 3]
来源：http://fm.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://et.huixiangedu.cn

[D08] 合并两个数组
来源：http://cw.521024.cn

Py:   a + b;  a.extend(b)
来源：http://ud.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://vu.bookmarksfly.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ef.szxytkj.cn

TS:   [...a, ...b];
来源：http://ws.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zp.nicolike.cn

Go:   append(a, b...)
来源：http://sp.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://rn.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://nl.gzmigu.cn

[D09] 排序（升序）
来源：http://to.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://jf.wgjwhj.cn

PHP:  sort($arr);
来源：http://yp.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kn.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rc.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mh.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dg.huanxung.cn

Ruby: arr.sort
来源：http://cz.chemitech.net.cn

C#:   list.Sort();
来源：http://uc.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ii.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jb.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xs.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yp.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yc.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wb.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://er.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sj.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ye.521024.cn

[D11] 反转数组
来源：http://qd.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dq.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://gx.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vh.panjiajie.cn

TS:   [...arr].reverse();
来源：http://vz.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://pm.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://pq.colortex.cn

Ruby: arr.reverse
来源：http://gz.521024.cn

C#:   list.Reverse();
来源：http://tr.bookmarksfly.cn

[D12] 查找元素下标
来源：http://sq.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://jj.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uj.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://we.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cf.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ct.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://gc.asd995.cn

Ruby: arr.index(x)
来源：http://dn.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://oo.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ln.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wb.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wb.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://dn.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://yi.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nw.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rq.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zu.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sf.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://in.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nj.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zc.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://an.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://co.szsharing.cn


<!-- 参考信息 -->