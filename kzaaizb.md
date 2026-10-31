代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://kq.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://kt.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nk.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://sa.nszjky.cn

C#:   string Greet(string name = "World") => name;
来源：http://fq.nicolike.cn

[C03] 可变参数
来源：http://xo.haigaiapp.cn

Py:   def total(*args): return sum(args)
来源：http://sv.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vg.9csxet.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://df.jctech888.com.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cv.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lo.huanxung.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ap.szsharing.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zh.bjjhwx.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ku.bookmarksfly.cn

[C04] 命名参数 / 关键字参数
来源：http://fj.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lv.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iv.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rc.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jk.panjiajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ya.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://jf.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://am.lnxyls.cn

C#:   f(a: 1, b: 2)
来源：http://gr.newstarts.cn

[C05] 返回多个值
来源：http://kn.huixinmuqiang.cn

Py:   return a, b
来源：http://eo.szxytkj.cn

PHP:  return [$a, $b];
来源：http://at.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fc.yuexingan06.cn

TS:   return { a, b };
来源：http://vp.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dg.asd995.cn

Go:   return a, b
来源：http://xg.shxzukj.cn

Ruby: return a, b
来源：http://gl.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://fa.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://cc.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://ph.521024.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zr.gzmigu.cn

JS:   const square = x => x * x;
来源：http://ti.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://zs.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kf.asd995.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yq.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://hi.jctech888.com.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jq.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://fz.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pw.colortex.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ux.bjjhwx.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://js.colortex.cn

TS:   arr.map(String)
来源：http://wo.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ck.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wf.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://tb.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oy.newstarts.cn

[C08] 闭包
来源：http://hm.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bc.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cj.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xl.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zn.bookmarksfly.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ql.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xh.szsharing.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lt.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jp.nszjky.cn

[C09] 递归
来源：http://cl.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pv.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ii.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://et.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kl.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tk.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://by.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ho.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pl.nszjky.cn

[C10] 变量作用域
来源：http://wk.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ty.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xk.yuntaijiaju.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ov.gzmigu.cn

TS:   同 JS
来源：http://di.hahajie.cn

Java: 方法内为块级作用域
来源：http://mc.colortex.cn

Go:   花括号块级作用域
来源：http://xj.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ib.shxzukj.cn

C#:   块级作用域
来源：http://sd.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://da.jianghongdianzi.cn

Py:   from module import func
来源：http://dr.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dh.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zo.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://di.hnjuh.cn

Java: import java.util.List;
来源：http://qf.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ey.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://dr.521024.cn

C#:   using System.Text;
来源：http://zq.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://hj.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://bp.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://hz.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://gy.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://oj.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bp.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://wb.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://dx.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://nn.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://ez.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ek.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xq.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ou.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://om.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qj.newstarts.cn

Go:   func add(a, b int) int
来源：http://rf.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nh.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vo.yuexingan06.cn

[C14] 泛型函数
来源：http://yn.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hd.shtwfgs.cn

PHP:  // 无泛型
来源：http://nj.shxzskj.cn

JS:   // 无泛型
来源：http://cf.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cx.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dv.9csxet.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://iy.shxzskj.cn

Ruby: # 无泛型
来源：http://dr.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hi.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://dd.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lw.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://xq.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hp.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yu.newstarts.cn

Java: // 无解构
来源：http://pe.szsharing.cn

Go:   // 无解构
来源：http://yy.yuexingan06.cn

Ruby: a, b = pair
来源：http://cg.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://yo.colortex.cn

[C16] 函数 / 方法重载
来源：http://hs.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kv.huixinmuqiang.cn

PHP:  // 无重载
来源：http://bh.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://br.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://nn.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://na.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://vg.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://wy.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ds.hahajie.cn

================================================================================
来源：http://iv.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://ei.muxihuayi.cn

================================================================================
来源：http://oe.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://lk.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dy.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ms.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bi.szxytkj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dj.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kl.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://oc.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://oa.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lq.shxzskj.cn

[D02] 追加元素到末尾
来源：http://mm.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sw.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uh.szxytkj.cn

JS:   arr.push(4);
来源：http://qg.szsharing.cn

TS:   arr.push(4);
来源：http://sn.newstarts.cn

Java: list.add(4);
来源：http://ig.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ri.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://rk.muxihuayi.cn

C#:   list.Add(4);
来源：http://wn.9csxet.cn

[D03] 在指定位置插入元素
来源：http://ze.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://on.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jj.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wl.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://ri.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://db.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://no.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sn.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://qu.yuntaijiaju.cn

[D04] 删除元素
来源：http://xe.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cc.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vn.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bn.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://im.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jr.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bg.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ac.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sx.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://es.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://re.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vw.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jo.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ij.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://mw.jianghongdianzi.cn

Go:   arr[0]; arr[0] = 9
来源：http://sb.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://no.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lo.huixiangedu.cn

[D06] 数组长度
来源：http://pd.yuexingan06.cn

Py:   len(arr)
来源：http://wm.hnjuh.cn

PHP:  count($arr);
来源：http://ob.muxihuayi.cn

JS:   arr.length
来源：http://ez.shtwfgs.cn

TS:   arr.length
来源：http://zs.9csxet.cn

Java: list.size();
来源：http://dp.jianghongdianzi.cn

Go:   len(arr)
来源：http://kn.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://fx.newstarts.cn

C#:   list.Count;
来源：http://fo.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://pu.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hy.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ye.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://zw.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://wt.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://sh.shxzskj.cn

Go:   arr[1:4]
来源：http://sg.colortex.cn

Ruby: arr[1, 3]
来源：http://fz.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://ds.newstarts.cn

[D08] 合并两个数组
来源：http://ts.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://nk.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://pe.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gg.bjjhwx.cn

TS:   [...a, ...b];
来源：http://qq.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nb.asd995.cn

Go:   append(a, b...)
来源：http://ab.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://zl.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://cy.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://js.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://wj.haigaiapp.cn

PHP:  sort($arr);
来源：http://pg.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fi.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sb.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xp.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yz.yuntaijiaju.cn

Ruby: arr.sort
来源：http://uu.yuntaijiaju.cn

C#:   list.Sort();
来源：http://pv.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nj.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dr.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ul.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kt.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wl.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ei.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fx.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gy.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hl.bookmarksfly.cn

[D11] 反转数组
来源：http://pc.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sv.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://ky.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ae.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://jf.521024.cn

Java: Collections.reverse(list);
来源：http://ur.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://pf.bookmarksfly.cn

Ruby: arr.reverse
来源：http://xf.bjjhwx.cn

C#:   list.Reverse();
来源：http://xz.szxytkj.cn

[D12] 查找元素下标
来源：http://do.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://hf.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sx.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ea.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ha.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jp.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://re.hahajie.cn

Ruby: arr.index(x)
来源：http://qc.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://qf.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://ft.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ik.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dk.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://nb.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://bi.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eh.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qb.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://la.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://du.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://ar.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://br.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kq.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://mc.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://dk.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yy.bookmarksfly.cn

Go:   // 手写循环
来源：http://ht.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ve.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hg.jctech888.com.cn

[D15] 去重
来源：http://xs.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ne.shtwfgs.cn

PHP:  array_unique($arr);
来源：http://zv.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://bm.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://ix.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tu.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://au.huixiangedu.cn

Ruby: arr.uniq
来源：http://ar.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://cn.huixiangedu.cn

[D16] 求和与平均值
来源：http://pd.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sh.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uy.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zu.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://va.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dr.huanxung.cn

Go:   // 手写循环累加
来源：http://ia.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qb.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://cb.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://tw.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://lo.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ox.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yt.szsharing.cn

TS:   Math.max(...arr);
来源：http://su.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://up.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xw.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://ca.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://az.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://dg.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://it.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://rg.9csxet.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mw.huixiangedu.cn

TS:   nested.flat();
来源：http://xl.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zw.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://qm.szsharing.cn

Ruby: nested.flatten
来源：http://xa.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zc.yuexingan06.cn

[D19] 按字段分组
来源：http://vi.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://za.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eu.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mp.nszjky.cn


<!-- 参考信息 -->