代发 wailian999

Py:   def add(a, b): return a + b
来源：http://ca.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wm.gzmigu.cn

JS:   function add(a, b) { return a + b; }
来源：http://ns.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eq.nicolike.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bb.shtwfgs.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nr.newstarts.cn

Ruby: def add(a, b); a + b; end
来源：http://qp.9csxet.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ob.yuntaijiaju.cn

[C02] 默认参数
来源：http://ou.huixinmuqiang.cn

Py:   def greet(name="World"): return name
来源：http://oj.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://oa.chemitech.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://lj.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wm.9csxet.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wm.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qx.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://ef.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://gj.shxzukj.cn

[C03] 可变参数
来源：http://mr.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://sq.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jq.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ef.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://si.chemitech.net.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qz.yuntaijiaju.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ry.shxzukj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uh.newstarts.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dh.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://fj.nicolike.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zu.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vh.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cv.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oi.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://tx.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://nc.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://bm.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://db.bookmarksfly.cn

[C05] 返回多个值
来源：http://fk.yuntaijiaju.cn

Py:   return a, b
来源：http://bb.asd995.cn

PHP:  return [$a, $b];
来源：http://lt.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qo.szxytkj.cn

TS:   return { a, b };
来源：http://ac.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xf.yuntaijiaju.cn

Go:   return a, b
来源：http://zy.yuexingan06.cn

Ruby: return a, b
来源：http://vu.huanxung.cn

C#:   return (a, b);              // ValueTuple
来源：http://jz.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://eb.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://zc.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sr.9csxet.cn

JS:   const square = x => x * x;
来源：http://uh.gzmigu.cn

TS:   const square = (x: number): number => x * x;
来源：http://du.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jg.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bw.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://zb.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xl.szsharing.cn

[C07] 把函数作为参数传入
来源：http://tr.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://em.lnxyls.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zi.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xx.wgjwhj.cn

TS:   arr.map(String)
来源：http://cw.shtwfgs.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://at.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xq.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://ou.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tw.wgjwhj.cn

[C08] 闭包
来源：http://df.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://av.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://st.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ds.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dt.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gr.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uo.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sf.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kv.shtwfgs.cn

[C09] 递归
来源：http://ht.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zt.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://km.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aj.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ko.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xu.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yr.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hn.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cc.bookmarksfly.cn

[C10] 变量作用域
来源：http://tx.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://si.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://go.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xf.shxzukj.cn

TS:   同 JS
来源：http://vf.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ri.asd995.cn

Go:   花括号块级作用域
来源：http://et.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uk.newstarts.cn

C#:   块级作用域
来源：http://xd.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://nb.jctech888.com.cn

Py:   from module import func
来源：http://ik.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://iy.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xt.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dy.shxzskj.cn

Java: import java.util.List;
来源：http://yj.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nt.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://ab.yuexingan06.cn

C#:   using System.Text;
来源：http://xd.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://un.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://nc.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://uk.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://iw.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://nw.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sa.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://pg.jianghongdianzi.cn

Ruby: -> { puts "run" }.call
来源：http://tw.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cr.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://iq.huanxung.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oq.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://al.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://th.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xl.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://iv.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://ph.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yz.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fy.shtwfgs.cn

[C14] 泛型函数
来源：http://az.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bp.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://qx.huixiangedu.cn

JS:   // 无泛型
来源：http://eu.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tx.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vt.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://km.shtwfgs.cn

Ruby: # 无泛型
来源：http://vs.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://co.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://at.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ui.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://qo.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qs.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hl.shtwfgs.cn

Java: // 无解构
来源：http://ak.hahajie.cn

Go:   // 无解构
来源：http://ih.hahajie.cn

Ruby: a, b = pair
来源：http://rh.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://cb.huanxung.cn

[C16] 函数 / 方法重载
来源：http://if.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fr.shxzskj.cn

PHP:  // 无重载
来源：http://gx.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nu.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://tp.nicolike.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ch.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://om.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://ct.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rd.muxihuayi.cn

================================================================================
来源：http://sg.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://bb.panjiajie.cn

================================================================================
来源：http://ex.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://eg.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pz.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yh.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bk.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ga.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ss.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://vx.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://pj.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://du.colortex.cn

[D02] 追加元素到末尾
来源：http://ll.haigaiapp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aa.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://he.colortex.cn

JS:   arr.push(4);
来源：http://bl.gzmigu.cn

TS:   arr.push(4);
来源：http://jt.huixiangedu.cn

Java: list.add(4);
来源：http://mr.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://bs.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://jc.nszjky.cn

C#:   list.Add(4);
来源：http://pa.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://pa.521024.cn

Py:   arr.insert(0, 0)
来源：http://pr.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ic.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://al.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://kc.muxihuayi.cn

Java: list.add(0, 0);
来源：http://jq.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ee.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cp.asd995.cn

C#:   list.Insert(0, 0);
来源：http://at.yuexingan06.cn

[D04] 删除元素
来源：http://ol.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://df.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zh.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bz.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://qk.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://md.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oz.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gf.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://te.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://ow.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lb.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ur.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://je.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://gu.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://bq.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://dv.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://th.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uj.shtwfgs.cn

[D06] 数组长度
来源：http://qh.shxzskj.cn

Py:   len(arr)
来源：http://el.gzmigu.cn

PHP:  count($arr);
来源：http://xb.shtwfgs.cn

JS:   arr.length
来源：http://px.nicolike.cn

TS:   arr.length
来源：http://vg.chemitech.net.cn

Java: list.size();
来源：http://fj.wgjwhj.cn

Go:   len(arr)
来源：http://qm.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://sj.szsharing.cn

C#:   list.Count;
来源：http://pe.szsharing.cn

[D07] 切片 / 取子数组
来源：http://uv.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yl.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hc.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://lr.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://pn.hahajie.cn

Java: list.subList(1, 4);
来源：http://df.shxzskj.cn

Go:   arr[1:4]
来源：http://qk.hnjuh.cn

Ruby: arr[1, 3]
来源：http://au.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://jr.newstarts.cn

[D08] 合并两个数组
来源：http://ku.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://ps.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://ap.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yh.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://qe.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lz.muxihuayi.cn

Go:   append(a, b...)
来源：http://cq.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://hz.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://cq.colortex.cn

[D09] 排序（升序）
来源：http://tk.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://wp.bookmarksfly.cn

PHP:  sort($arr);
来源：http://mn.yuntaijiaju.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://df.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fc.hnjuh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://um.hahajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iy.shxzskj.cn

Ruby: arr.sort
来源：http://rx.lnxyls.cn

C#:   list.Sort();
来源：http://ri.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ge.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hf.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mp.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oy.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gr.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mg.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gq.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mh.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pz.hnjuh.cn

[D11] 反转数组
来源：http://cm.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rx.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://ih.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zw.panjiajie.cn

TS:   [...arr].reverse();
来源：http://nr.szsharing.cn

Java: Collections.reverse(list);
来源：http://pu.hahajie.cn

Go:   slices.Reverse(arr)
来源：http://lw.nszjky.cn

Ruby: arr.reverse
来源：http://cs.shxzskj.cn

C#:   list.Reverse();
来源：http://ha.szxytkj.cn

[D12] 查找元素下标
来源：http://zn.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://hr.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kk.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://es.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xx.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yk.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://gp.huixiangedu.cn

Ruby: arr.index(x)
来源：http://zm.newstarts.cn

C#:   list.IndexOf(x);
来源：http://xs.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://ec.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://it.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rn.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://yr.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://si.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sr.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sj.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rt.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vr.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://wh.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ak.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zg.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://fp.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://wz.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ex.colortex.cn

Go:   // 手写循环
来源：http://jg.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://it.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qf.haigaiapp.cn

[D15] 去重
来源：http://kc.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bh.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://jh.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://am.colortex.cn

TS:   [...new Set(arr)]
来源：http://mt.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lq.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ee.panjiajie.cn

Ruby: arr.uniq
来源：http://zy.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://pf.hnjuh.cn

[D16] 求和与平均值
来源：http://vy.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nw.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xb.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xr.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://un.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://av.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://vf.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://go.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://ec.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://yx.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://fk.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://tf.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vk.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://dc.panjiajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hn.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ia.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://ia.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://kf.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://eg.newstarts.cn


<!-- 参考信息 -->