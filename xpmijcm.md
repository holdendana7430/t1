代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://fs.szsharing.cn

[C03] 可变参数
来源：http://rw.jianghongdianzi.cn

Py:   def total(*args): return sum(args)
来源：http://ay.bookmarksfly.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jf.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pe.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lh.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tj.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://go.huixinmuqiang.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yw.jctech888.com.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ku.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://mp.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ao.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mg.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nd.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pi.bookmarksfly.cn

Java: // 无：用 Builder 模式或 record
来源：http://cs.gzmigu.cn

Go:   // 无：用配置结构体参数
来源：http://gx.szxytkj.cn

Ruby: f(a: 1, b: 2)
来源：http://yf.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://pt.haigaiapp.cn

[C05] 返回多个值
来源：http://hg.haigaiapp.cn

Py:   return a, b
来源：http://yj.asd995.cn

PHP:  return [$a, $b];
来源：http://gf.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ir.gzmigu.cn

TS:   return { a, b };
来源：http://bv.hahajie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zy.colortex.cn

Go:   return a, b
来源：http://wp.gzmigu.cn

Ruby: return a, b
来源：http://ui.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://gc.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://sh.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://hv.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://uu.yuexingan06.cn

JS:   const square = x => x * x;
来源：http://pu.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://ay.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sh.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xn.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://kn.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gm.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://eg.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ky.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ti.shxzukj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jg.shxzukj.cn

TS:   arr.map(String)
来源：http://oa.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kh.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rt.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://jy.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uf.hahajie.cn

[C08] 闭包
来源：http://rw.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yk.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oh.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oc.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fq.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ql.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wt.shxzukj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xl.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yn.nicolike.cn

[C09] 递归
来源：http://el.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mf.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cf.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lu.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ta.yuntaijiaju.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pi.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ec.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xa.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ma.chemitech.net.cn

[C10] 变量作用域
来源：http://be.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zk.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tw.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hc.huanxung.cn

TS:   同 JS
来源：http://kh.gzmigu.cn

Java: 方法内为块级作用域
来源：http://wn.shxzukj.cn

Go:   花括号块级作用域
来源：http://tv.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xh.shxzukj.cn

C#:   块级作用域
来源：http://rd.wgjwhj.cn

[C11] 模块导入与导出
来源：http://ef.bookmarksfly.cn

Py:   from module import func
来源：http://ho.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xf.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ve.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wh.szxytkj.cn

Java: import java.util.List;
来源：http://nq.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zs.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://uf.wgjwhj.cn

C#:   using System.Text;
来源：http://tx.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://fm.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://rd.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://vl.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://cl.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://uw.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sd.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yw.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ic.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jk.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://fe.yuntaijiaju.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yv.chemitech.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vg.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nn.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://am.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eg.nszjky.cn

Go:   func add(a, b int) int
来源：http://kj.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lj.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gp.9csxet.cn

[C14] 泛型函数
来源：http://wo.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sz.lnxyls.cn

PHP:  // 无泛型
来源：http://um.szsharing.cn

JS:   // 无泛型
来源：http://za.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dw.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://al.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wx.gzmigu.cn

Ruby: # 无泛型
来源：http://jc.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wu.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://fs.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vb.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://lm.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://db.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mh.jctech888.com.cn

Java: // 无解构
来源：http://aj.panjiajie.cn

Go:   // 无解构
来源：http://zq.colortex.cn

Ruby: a, b = pair
来源：http://dq.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://ha.9csxet.cn

[C16] 函数 / 方法重载
来源：http://yq.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sf.asd995.cn

PHP:  // 无重载
来源：http://la.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wb.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://pt.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ig.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://of.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://kk.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qp.szxytkj.cn

================================================================================
来源：http://lm.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://ro.szsharing.cn

================================================================================
来源：http://ud.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ji.panjiajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nr.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ut.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xp.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bk.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://av.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://bz.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://bf.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://za.panjiajie.cn

[D02] 追加元素到末尾
来源：http://xc.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ft.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qi.hnjuh.cn

JS:   arr.push(4);
来源：http://ft.lnxyls.cn

TS:   arr.push(4);
来源：http://sw.yuexingan06.cn

Java: list.add(4);
来源：http://zx.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://tj.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://be.9csxet.cn

C#:   list.Add(4);
来源：http://zc.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://tg.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://fa.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cc.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ox.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://nc.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://jq.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ii.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hl.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://kb.szsharing.cn

[D04] 删除元素
来源：http://sa.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://db.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ce.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jp.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://qc.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gh.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wn.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lm.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nk.gzmigu.cn

[D05] 访问与修改元素
来源：http://nz.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qw.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hy.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://am.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ua.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://sd.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://mx.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ak.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rc.wgjwhj.cn

[D06] 数组长度
来源：http://wr.colortex.cn

Py:   len(arr)
来源：http://bo.huixinmuqiang.cn

PHP:  count($arr);
来源：http://xp.newstarts.cn

JS:   arr.length
来源：http://wo.panjiajie.cn

TS:   arr.length
来源：http://rt.shxzskj.cn

Java: list.size();
来源：http://lh.muxihuayi.cn

Go:   len(arr)
来源：http://ic.yuntaijiaju.cn

Ruby: arr.length; arr.size
来源：http://ib.521024.cn

C#:   list.Count;
来源：http://mo.szsharing.cn

[D07] 切片 / 取子数组
来源：http://vo.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://go.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qj.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://dr.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://ra.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://dj.huanxung.cn

Go:   arr[1:4]
来源：http://pn.9csxet.cn

Ruby: arr[1, 3]
来源：http://ue.521024.cn

C#:   list.GetRange(1, 3);
来源：http://tp.huixinmuqiang.cn

[D08] 合并两个数组
来源：http://if.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://zn.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://pp.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jb.wgjwhj.cn

TS:   [...a, ...b];
来源：http://dx.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wi.chemitech.net.cn

Go:   append(a, b...)
来源：http://gh.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://nt.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://jb.yuexingan06.cn

[D09] 排序（升序）
来源：http://lx.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://zr.muxihuayi.cn

PHP:  sort($arr);
来源：http://rr.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rz.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mg.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cy.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://td.muxihuayi.cn

Ruby: arr.sort
来源：http://fp.colortex.cn

C#:   list.Sort();
来源：http://ck.hnjuh.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yd.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ni.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fb.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qr.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fq.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cy.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zu.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dc.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pr.shxzukj.cn

[D11] 反转数组
来源：http://sx.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lq.colortex.cn

PHP:  array_reverse($arr);
来源：http://dr.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gz.asd995.cn

TS:   [...arr].reverse();
来源：http://hh.huanxung.cn

Java: Collections.reverse(list);
来源：http://ax.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://er.panjiajie.cn

Ruby: arr.reverse
来源：http://tv.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://pn.newstarts.cn

[D12] 查找元素下标
来源：http://om.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://js.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ye.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aj.chemitech.net.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zj.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xd.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://kd.wgjwhj.cn

Ruby: arr.index(x)
来源：http://od.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://zw.panjiajie.cn

[D13] 过滤（保留满足条件的）
来源：http://sa.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://an.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ku.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://zo.szsharing.cn

TS:   arr.filter(x => x > 3)
来源：http://kp.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rv.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ma.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zp.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sr.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://gp.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pu.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qa.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://su.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://gu.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fa.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ow.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dh.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nx.panjiajie.cn

[D15] 去重
来源：http://nt.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ei.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://nb.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://un.521024.cn

TS:   [...new Set(arr)]
来源：http://wh.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ga.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qp.lnxyls.cn

Ruby: arr.uniq
来源：http://jg.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://bv.asd995.cn

[D16] 求和与平均值
来源：http://be.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jb.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ui.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rs.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wy.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gl.9csxet.cn

Go:   // 手写循环累加
来源：http://xm.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nj.huixinmuqiang.cn

C#:   list.Sum();  list.Average()
来源：http://nm.asd995.cn

[D17] 最大值与最小值
来源：http://up.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://ip.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://ms.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wb.newstarts.cn

TS:   Math.max(...arr);
来源：http://ec.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nq.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gf.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://hc.521024.cn

C#:   list.Max();  list.Min()
来源：http://tf.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://sk.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sq.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://yv.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ks.jianghongdianzi.cn

TS:   nested.flat();
来源：http://sg.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xf.huixiangedu.cn

Go:   // 手写双层循环
来源：http://dy.muxihuayi.cn

Ruby: nested.flatten
来源：http://wm.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vs.muxihuayi.cn

[D19] 按字段分组
来源：http://an.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zx.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bf.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://he.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fo.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eh.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://zp.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zq.huixinmuqiang.cn


<!-- 参考信息 -->