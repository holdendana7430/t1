代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://gu.shxzukj.cn

[C03] 可变参数
来源：http://nr.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://rx.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pi.huanxung.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dj.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ki.newstarts.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sa.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ku.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ap.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bo.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://uz.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mt.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ru.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ki.jianghongdianzi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fw.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://km.panjiajie.cn

Go:   // 无：用配置结构体参数
来源：http://tc.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://uw.9csxet.cn

C#:   f(a: 1, b: 2)
来源：http://fx.huixiangedu.cn

[C05] 返回多个值
来源：http://yz.huanxung.cn

Py:   return a, b
来源：http://kw.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://dk.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cy.jctech888.com.cn

TS:   return { a, b };
来源：http://we.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rh.szsharing.cn

Go:   return a, b
来源：http://oh.huixiangedu.cn

Ruby: return a, b
来源：http://zh.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://ck.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://uq.hnjuh.cn

Py:   square = lambda x: x * x
来源：http://sh.szsharing.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fk.hahajie.cn

JS:   const square = x => x * x;
来源：http://dq.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://xe.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wd.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xc.szsharing.cn

Ruby: square = ->(x) { x * x }
来源：http://gr.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qa.szsharing.cn

[C07] 把函数作为参数传入
来源：http://ii.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yh.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cb.chemitech.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://en.colortex.cn

TS:   arr.map(String)
来源：http://kt.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hu.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zb.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://fa.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mz.colortex.cn

[C08] 闭包
来源：http://tm.nicolike.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oq.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ek.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gj.chemitech.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rh.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lb.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tf.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ks.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uk.shtwfgs.cn

[C09] 递归
来源：http://al.szxytkj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rf.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ts.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wi.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jr.jianghongdianzi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nl.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ci.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yr.lnxyls.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ny.jctech888.com.cn

[C10] 变量作用域
来源：http://lb.hnjuh.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jg.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://od.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vj.asd995.cn

TS:   同 JS
来源：http://kg.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://fh.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://jz.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ki.haigaiapp.cn

C#:   块级作用域
来源：http://vb.shxzukj.cn

[C11] 模块导入与导出
来源：http://iv.hahajie.cn

Py:   from module import func
来源：http://xw.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ak.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kq.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hx.huixiangedu.cn

Java: import java.util.List;
来源：http://uw.lnxyls.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mo.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://mi.szsharing.cn

C#:   using System.Text;
来源：http://aw.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://sf.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://jf.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://ia.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://ko.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://tn.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wz.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://sr.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://bf.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kg.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://mx.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qd.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ei.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lc.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oi.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dc.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://km.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ug.panjiajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ld.bookmarksfly.cn

[C14] 泛型函数
来源：http://sa.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zy.nicolike.cn

PHP:  // 无泛型
来源：http://hh.colortex.cn

JS:   // 无泛型
来源：http://pf.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xm.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ey.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zt.huanxung.cn

Ruby: # 无泛型
来源：http://jt.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vi.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://hu.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gb.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://sh.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://on.bjjhwx.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ny.muxihuayi.cn

Java: // 无解构
来源：http://qs.hnjuh.cn

Go:   // 无解构
来源：http://am.nszjky.cn

Ruby: a, b = pair
来源：http://bk.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://jz.huanxung.cn

[C16] 函数 / 方法重载
来源：http://lk.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yn.panjiajie.cn

PHP:  // 无重载
来源：http://sb.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qg.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://tj.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://an.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://ah.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://xz.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rh.shxzukj.cn

================================================================================
来源：http://cg.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://dh.jianghongdianzi.cn

================================================================================
来源：http://ig.huanxung.cn

[D01] 创建数组 / 列表
来源：http://kw.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lj.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fw.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ox.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dj.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pn.szsharing.cn

Go:   arr := []int{1, 2, 3}
来源：http://fe.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://we.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cb.hahajie.cn

[D02] 追加元素到末尾
来源：http://rv.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yy.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jy.huixiangedu.cn

JS:   arr.push(4);
来源：http://np.lnxyls.cn

TS:   arr.push(4);
来源：http://ei.lnxyls.cn

Java: list.add(4);
来源：http://ks.9csxet.cn

Go:   arr = append(arr, 4)
来源：http://tv.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://ot.9csxet.cn

C#:   list.Add(4);
来源：http://oa.yuntaijiaju.cn

[D03] 在指定位置插入元素
来源：http://ea.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://fy.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vd.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://za.shxzskj.cn

TS:   arr.splice(0, 0, 0);
来源：http://fz.shxzskj.cn

Java: list.add(0, 0);
来源：http://ti.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vd.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nn.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://iq.asd995.cn

[D04] 删除元素
来源：http://kh.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ze.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gv.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vp.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://my.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xp.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sl.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yi.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nh.huixiangedu.cn

[D05] 访问与修改元素
来源：http://hg.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dk.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ah.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xq.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://yg.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://dy.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://wu.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vo.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kq.shxzukj.cn

[D06] 数组长度
来源：http://pw.hnjuh.cn

Py:   len(arr)
来源：http://vk.shtwfgs.cn

PHP:  count($arr);
来源：http://kh.yuntaijiaju.cn

JS:   arr.length
来源：http://ex.huixiangedu.cn

TS:   arr.length
来源：http://lr.bookmarksfly.cn

Java: list.size();
来源：http://du.bjjhwx.cn

Go:   len(arr)
来源：http://sr.huanxung.cn

Ruby: arr.length; arr.size
来源：http://iw.hahajie.cn

C#:   list.Count;
来源：http://bo.newstarts.cn

[D07] 切片 / 取子数组
来源：http://lz.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nv.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sw.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://em.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://ji.szxytkj.cn

Java: list.subList(1, 4);
来源：http://io.521024.cn

Go:   arr[1:4]
来源：http://ss.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://sw.chemitech.net.cn

C#:   list.GetRange(1, 3);
来源：http://zc.yuexingan06.cn

[D08] 合并两个数组
来源：http://fi.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://dx.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://dx.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bv.gzmigu.cn

TS:   [...a, ...b];
来源：http://sj.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sj.newstarts.cn

Go:   append(a, b...)
来源：http://wj.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://gv.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://tv.nicolike.cn

[D09] 排序（升序）
来源：http://dx.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://np.shxzukj.cn

PHP:  sort($arr);
来源：http://uc.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iz.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ph.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://nv.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zr.szsharing.cn

Ruby: arr.sort
来源：http://bp.yuntaijiaju.cn

C#:   list.Sort();
来源：http://ic.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ms.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nd.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://si.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oi.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ol.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fo.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ql.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://so.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ot.jianghongdianzi.cn

[D11] 反转数组
来源：http://qq.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hw.asd995.cn

PHP:  array_reverse($arr);
来源：http://nd.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fm.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://pd.colortex.cn

Java: Collections.reverse(list);
来源：http://pj.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://pm.huanxung.cn

Ruby: arr.reverse
来源：http://dw.haigaiapp.cn

C#:   list.Reverse();
来源：http://ov.hahajie.cn

[D12] 查找元素下标
来源：http://pw.nicolike.cn

Py:   arr.index(x);  x in arr
来源：http://gi.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nk.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lw.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xh.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qh.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://kq.shxzskj.cn

Ruby: arr.index(x)
来源：http://ww.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://on.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://fw.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://no.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ek.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://qt.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://hf.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ko.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xo.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kg.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hy.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://jf.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mj.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ov.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://di.521024.cn

TS:   arr.map(x => x * 2)
来源：http://hq.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ip.szsharing.cn

Go:   // 手写循环
来源：http://oo.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cx.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sk.shtwfgs.cn

[D15] 去重
来源：http://qd.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yp.shxzukj.cn

PHP:  array_unique($arr);
来源：http://ol.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://oa.szsharing.cn

TS:   [...new Set(arr)]
来源：http://lj.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yl.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wq.bjjhwx.cn

Ruby: arr.uniq
来源：http://hz.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://td.9csxet.cn

[D16] 求和与平均值
来源：http://sz.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://la.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nj.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ln.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gz.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gj.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://cp.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gl.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://hp.huixiangedu.cn

[D17] 最大值与最小值
来源：http://qc.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://kv.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://rv.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rw.colortex.cn

TS:   Math.max(...arr);
来源：http://ep.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rc.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://am.bookmarksfly.cn

Ruby: arr.max;  arr.min
来源：http://ta.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://qi.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://og.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oo.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://zw.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ik.jctech888.com.cn

TS:   nested.flat();
来源：http://eo.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qv.asd995.cn

Go:   // 手写双层循环
来源：http://mi.9csxet.cn

Ruby: nested.flatten
来源：http://ad.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://as.asd995.cn

[D19] 按字段分组
来源：http://fy.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fp.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rc.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tw.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hb.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ss.colortex.cn

Go:   // 手写 map[string][]T
来源：http://xx.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yr.nicolike.cn


<!-- 参考信息 -->