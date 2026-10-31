代发 wailian999

PHP:  $a && $b || !$c
来源：http://rx.shtwfgs.cn

JS:   a && b || !c
来源：http://ut.wgjwhj.cn

TS:   a && b || !c
来源：http://wv.huanxung.cn

Java: a && b || !c
来源：http://mn.hnjuh.cn

Go:   a && b || !c
来源：http://mz.szxytkj.cn

Ruby: a && b || !c
来源：http://uz.hahajie.cn

C#:   a && b || !c
来源：http://bu.yuntaijiaju.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lq.yuntaijiaju.cn

Py:   if not data: return
来源：http://vg.yuntaijiaju.cn

PHP:  if (!$data) { return; }
来源：http://pf.gzmigu.cn

JS:   if (!data) return;
来源：http://ge.gzmigu.cn

TS:   if (!data) return;
来源：http://jb.nszjky.cn

Java: if (data == null) return;
来源：http://qe.jctech888.com.cn

Go:   if data == nil { return }
来源：http://hh.hahajie.cn

Ruby: return if data.nil?
来源：http://zn.huixiangedu.cn

C#:   if (data == null) return;
来源：http://af.haigaiapp.cn

================================================================================
来源：http://ek.nszjky.cn

C. 函数与作用域
来源：http://uc.521024.cn

================================================================================
来源：http://os.hahajie.cn

[C01] 定义函数
来源：http://ep.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://zp.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yb.jctech888.com.cn

JS:   function add(a, b) { return a + b; }
来源：http://ni.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xj.hahajie.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://an.shxzukj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sy.bjjhwx.cn

Ruby: def add(a, b); a + b; end
来源：http://st.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ei.szsharing.cn

[C02] 默认参数
来源：http://kl.bookmarksfly.cn

Py:   def greet(name="World"): return name
来源：http://sg.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://er.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://fq.haigaiapp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rh.muxihuayi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wu.bookmarksfly.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vt.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://qp.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://gh.shxzukj.cn

[C03] 可变参数
来源：http://fo.yuexingan06.cn

Py:   def total(*args): return sum(args)
来源：http://ib.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ol.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ep.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gs.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rw.bookmarksfly.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ab.yuntaijiaju.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hp.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://az.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://cj.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ey.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xy.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qj.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ag.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://ui.shxzukj.cn

Go:   // 无：用配置结构体参数
来源：http://bw.9csxet.cn

Ruby: f(a: 1, b: 2)
来源：http://lo.jctech888.com.cn

C#:   f(a: 1, b: 2)
来源：http://il.haigaiapp.cn

[C05] 返回多个值
来源：http://nm.521024.cn

Py:   return a, b
来源：http://mw.gzmigu.cn

PHP:  return [$a, $b];
来源：http://hz.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sc.shtwfgs.cn

TS:   return { a, b };
来源：http://cz.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ru.hahajie.cn

Go:   return a, b
来源：http://xt.bookmarksfly.cn

Ruby: return a, b
来源：http://me.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ru.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://pi.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://dw.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eb.muxihuayi.cn

JS:   const square = x => x * x;
来源：http://lh.bookmarksfly.cn

TS:   const square = (x: number): number => x * x;
来源：http://ao.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ke.gzmigu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kh.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://us.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hq.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://si.gzmigu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fd.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kl.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ks.bookmarksfly.cn

TS:   arr.map(String)
来源：http://qd.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tz.huixinmuqiang.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yc.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://at.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ve.nicolike.cn

[C08] 闭包
来源：http://xb.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zx.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://op.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nv.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rb.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mo.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wb.521024.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wj.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://it.shxzukj.cn

[C09] 递归
来源：http://yw.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dr.lnxyls.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ux.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://se.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ta.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://am.jctech888.com.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ff.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tk.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zk.huixinmuqiang.cn

[C10] 变量作用域
来源：http://sf.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xa.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xl.jctech888.com.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yz.hnjuh.cn

TS:   同 JS
来源：http://no.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://uj.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://ur.shtwfgs.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mb.shtwfgs.cn

C#:   块级作用域
来源：http://io.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://ji.huanxung.cn

Py:   from module import func
来源：http://po.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ix.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ol.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sv.huixinmuqiang.cn

Java: import java.util.List;
来源：http://gx.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qq.nszjky.cn

Ruby: require "json"; require_relative "./util"
来源：http://bz.jctech888.com.cn

C#:   using System.Text;
来源：http://hg.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://jq.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://zj.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://ku.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://ji.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://qi.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tr.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ll.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://bt.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wy.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://kd.9csxet.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oo.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bv.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hq.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fw.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gx.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://qn.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jx.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hy.hahajie.cn

[C14] 泛型函数
来源：http://fb.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jp.shxzskj.cn

PHP:  // 无泛型
来源：http://us.gzmigu.cn

JS:   // 无泛型
来源：http://po.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rz.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pl.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nf.huixiangedu.cn

Ruby: # 无泛型
来源：http://zz.szsharing.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pf.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://aj.szsharing.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://je.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://yi.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tf.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cl.yuexingan06.cn

Java: // 无解构
来源：http://sa.jianghongdianzi.cn

Go:   // 无解构
来源：http://yq.huixiangedu.cn

Ruby: a, b = pair
来源：http://iu.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://zw.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://li.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://up.chemitech.net.cn

PHP:  // 无重载
来源：http://yz.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hp.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://ov.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ly.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://lu.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://jc.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://eb.lnxyls.cn

================================================================================
来源：http://cq.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://yy.lnxyls.cn

================================================================================
来源：http://xv.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://rb.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tz.521024.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kw.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cw.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kb.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xs.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://ui.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://vt.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cg.panjiajie.cn

[D02] 追加元素到末尾
来源：http://wu.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xa.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mx.muxihuayi.cn

JS:   arr.push(4);
来源：http://ro.panjiajie.cn

TS:   arr.push(4);
来源：http://uk.huixinmuqiang.cn

Java: list.add(4);
来源：http://cf.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://ou.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ue.shtwfgs.cn

C#:   list.Add(4);
来源：http://nt.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://id.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://wd.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tu.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://je.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://sf.yuexingan06.cn

Java: list.add(0, 0);
来源：http://gc.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://is.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tq.asd995.cn

C#:   list.Insert(0, 0);
来源：http://ze.asd995.cn

[D04] 删除元素
来源：http://yp.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vk.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fi.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://am.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://ho.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vm.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lz.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xo.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://al.huanxung.cn

[D05] 访问与修改元素
来源：http://bq.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hv.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ga.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qc.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://uf.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://dl.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://sw.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wj.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://df.szxytkj.cn

[D06] 数组长度
来源：http://rv.jctech888.com.cn

Py:   len(arr)
来源：http://qh.hahajie.cn

PHP:  count($arr);
来源：http://vl.shxzukj.cn

JS:   arr.length
来源：http://li.huanxung.cn

TS:   arr.length
来源：http://ow.9csxet.cn

Java: list.size();
来源：http://nb.521024.cn

Go:   len(arr)
来源：http://zh.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://gm.nicolike.cn

C#:   list.Count;
来源：http://cx.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://zv.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ih.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vx.asd995.cn

JS:   arr.slice(1, 4);
来源：http://rv.colortex.cn

TS:   arr.slice(1, 4);
来源：http://cn.colortex.cn

Java: list.subList(1, 4);
来源：http://sg.hnjuh.cn

Go:   arr[1:4]
来源：http://kk.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://jr.521024.cn

C#:   list.GetRange(1, 3);
来源：http://aa.gzmigu.cn

[D08] 合并两个数组
来源：http://uk.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://rl.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://de.huixinmuqiang.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ba.asd995.cn

TS:   [...a, ...b];
来源：http://pp.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uq.huixiangedu.cn

Go:   append(a, b...)
来源：http://bv.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://pg.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://co.lnxyls.cn

[D09] 排序（升序）
来源：http://vl.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vi.huanxung.cn

PHP:  sort($arr);
来源：http://tx.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lq.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ce.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://in.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rn.colortex.cn

Ruby: arr.sort
来源：http://xb.lnxyls.cn

C#:   list.Sort();
来源：http://wj.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jj.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dn.huixinmuqiang.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bu.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gk.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yp.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ie.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://od.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://im.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jp.shtwfgs.cn

[D11] 反转数组
来源：http://ng.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://af.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://bz.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ss.hnjuh.cn

TS:   [...arr].reverse();
来源：http://vm.colortex.cn

Java: Collections.reverse(list);
来源：http://oh.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://gg.shxzskj.cn

Ruby: arr.reverse
来源：http://ej.asd995.cn

C#:   list.Reverse();
来源：http://xj.hnjuh.cn

[D12] 查找元素下标
来源：http://vb.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://wn.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ms.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ge.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pt.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cu.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://yk.chemitech.net.cn

Ruby: arr.index(x)
来源：http://cw.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://xb.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://gd.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://el.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rf.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://uf.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://dt.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jx.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://th.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cp.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ge.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://tu.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jl.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://px.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://kt.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://mb.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dj.nszjky.cn

Go:   // 手写循环
来源：http://xw.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cf.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zw.bjjhwx.cn

[D15] 去重
来源：http://jp.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pk.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://ad.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://qt.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://qk.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zg.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sf.haigaiapp.cn

Ruby: arr.uniq
来源：http://ii.shtwfgs.cn


<!-- 参考信息 -->