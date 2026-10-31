代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://mb.nicolike.cn

[C03] 可变参数
来源：http://sl.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://rj.chemitech.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rn.asd995.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gu.colortex.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ja.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://la.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bz.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://py.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://db.panjiajie.cn

[C04] 命名参数 / 关键字参数
来源：http://bo.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zy.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vu.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://um.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qo.yuexingan06.cn

Java: // 无：用 Builder 模式或 record
来源：http://fc.colortex.cn

Go:   // 无：用配置结构体参数
来源：http://eg.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://if.yuexingan06.cn

C#:   f(a: 1, b: 2)
来源：http://xw.hahajie.cn

[C05] 返回多个值
来源：http://xz.szxytkj.cn

Py:   return a, b
来源：http://lx.yuntaijiaju.cn

PHP:  return [$a, $b];
来源：http://wl.hahajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mb.muxihuayi.cn

TS:   return { a, b };
来源：http://mo.wgjwhj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hs.shxzukj.cn

Go:   return a, b
来源：http://uh.newstarts.cn

Ruby: return a, b
来源：http://ng.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://tk.gzmigu.cn

[C06] 匿名函数 / lambda
来源：http://yd.colortex.cn

Py:   square = lambda x: x * x
来源：http://bz.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bt.gzmigu.cn

JS:   const square = x => x * x;
来源：http://ag.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ih.bjjhwx.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ks.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ix.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://hh.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://et.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://ka.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ni.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zn.hnjuh.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://do.huanxung.cn

TS:   arr.map(String)
来源：http://jg.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gy.szxytkj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ov.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://zo.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jp.9csxet.cn

[C08] 闭包
来源：http://iy.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ha.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://be.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ch.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hn.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xj.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ql.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://on.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wj.gzmigu.cn

[C09] 递归
来源：http://yt.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://we.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://as.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tg.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gq.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://et.shxzskj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mf.gzmigu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ub.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gt.wgjwhj.cn

[C10] 变量作用域
来源：http://cy.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kz.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vj.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bt.muxihuayi.cn

TS:   同 JS
来源：http://wj.colortex.cn

Java: 方法内为块级作用域
来源：http://xk.wgjwhj.cn

Go:   花括号块级作用域
来源：http://wb.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ie.colortex.cn

C#:   块级作用域
来源：http://ql.huixiangedu.cn

[C11] 模块导入与导出
来源：http://xp.nicolike.cn

Py:   from module import func
来源：http://nv.lnxyls.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vq.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://er.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dz.jctech888.com.cn

Java: import java.util.List;
来源：http://ju.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vi.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://gf.hnjuh.cn

C#:   using System.Text;
来源：http://sp.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://ye.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://gw.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://va.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://ef.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://jg.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mp.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ao.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://uw.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://aq.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://yx.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jd.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wa.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pd.muxihuayi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gt.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vv.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://br.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bt.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://na.bookmarksfly.cn

[C14] 泛型函数
来源：http://fp.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://of.newstarts.cn

PHP:  // 无泛型
来源：http://ug.9csxet.cn

JS:   // 无泛型
来源：http://ow.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zy.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mu.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zs.newstarts.cn

Ruby: # 无泛型
来源：http://zn.muxihuayi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dx.hahajie.cn

[C15] 解构 / 展开参数
来源：http://bz.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dc.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://hz.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gn.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ua.jianghongdianzi.cn

Java: // 无解构
来源：http://fd.lnxyls.cn

Go:   // 无解构
来源：http://qb.newstarts.cn

Ruby: a, b = pair
来源：http://bt.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://nj.nicolike.cn

[C16] 函数 / 方法重载
来源：http://tp.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ma.huanxung.cn

PHP:  // 无重载
来源：http://ym.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://du.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://fp.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vw.yuexingan06.cn

Go:   // 无重载：用不同函数名
来源：http://lg.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://qa.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ji.yuexingan06.cn

================================================================================
来源：http://py.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://dt.newstarts.cn

================================================================================
来源：http://nw.asd995.cn

[D01] 创建数组 / 列表
来源：http://hm.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oc.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ao.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pk.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gk.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kp.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://fu.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://zu.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gh.asd995.cn

[D02] 追加元素到末尾
来源：http://pk.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ua.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wg.nicolike.cn

JS:   arr.push(4);
来源：http://yu.newstarts.cn

TS:   arr.push(4);
来源：http://yv.bookmarksfly.cn

Java: list.add(4);
来源：http://cs.521024.cn

Go:   arr = append(arr, 4)
来源：http://jt.wgjwhj.cn

Ruby: arr << 4; arr.push(5)
来源：http://qd.nszjky.cn

C#:   list.Add(4);
来源：http://fq.nszjky.cn

[D03] 在指定位置插入元素
来源：http://vn.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://ek.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fh.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://un.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://bs.yuexingan06.cn

Java: list.add(0, 0);
来源：http://qo.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://se.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bw.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://vb.jctech888.com.cn

[D04] 删除元素
来源：http://km.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kl.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wd.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://df.colortex.cn

TS:   arr.splice(0, 1);
来源：http://ui.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uv.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tl.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ef.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yv.nicolike.cn

[D05] 访问与修改元素
来源：http://hu.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kd.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fi.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oj.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://wv.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://gv.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://br.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jc.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hl.521024.cn

[D06] 数组长度
来源：http://ue.jianghongdianzi.cn

Py:   len(arr)
来源：http://kj.bjjhwx.cn

PHP:  count($arr);
来源：http://yf.szsharing.cn

JS:   arr.length
来源：http://in.yuntaijiaju.cn

TS:   arr.length
来源：http://xf.yuntaijiaju.cn

Java: list.size();
来源：http://lv.hahajie.cn

Go:   len(arr)
来源：http://lt.9csxet.cn

Ruby: arr.length; arr.size
来源：http://uw.jianghongdianzi.cn

C#:   list.Count;
来源：http://mu.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://pb.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ed.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gq.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://hx.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://bk.asd995.cn

Java: list.subList(1, 4);
来源：http://au.bjjhwx.cn

Go:   arr[1:4]
来源：http://dv.hnjuh.cn

Ruby: arr[1, 3]
来源：http://zi.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://mb.shxzukj.cn

[D08] 合并两个数组
来源：http://vy.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://df.asd995.cn

PHP:  array_merge($a, $b);
来源：http://rn.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hv.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://bp.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hk.shxzskj.cn

Go:   append(a, b...)
来源：http://fd.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://zt.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://et.nicolike.cn

[D09] 排序（升序）
来源：http://al.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://us.huanxung.cn

PHP:  sort($arr);
来源：http://ef.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tu.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://en.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rf.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wm.yuntaijiaju.cn

Ruby: arr.sort
来源：http://se.nicolike.cn

C#:   list.Sort();
来源：http://iw.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yz.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ay.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rf.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://io.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nf.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yy.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://to.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nd.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ej.shxzukj.cn

[D11] 反转数组
来源：http://vv.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://do.colortex.cn

PHP:  array_reverse($arr);
来源：http://lu.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lf.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://wr.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://kt.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://yq.muxihuayi.cn

Ruby: arr.reverse
来源：http://dt.chemitech.net.cn

C#:   list.Reverse();
来源：http://gv.panjiajie.cn

[D12] 查找元素下标
来源：http://vf.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://li.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ya.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vj.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://co.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aa.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://jb.szsharing.cn

Ruby: arr.index(x)
来源：http://oa.szsharing.cn

C#:   list.IndexOf(x);
来源：http://fy.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://vz.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bq.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://de.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://qo.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://zq.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jq.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bm.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jh.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hv.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://dj.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wo.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gr.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://sd.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://qu.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yh.wgjwhj.cn

Go:   // 手写循环
来源：http://oa.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tw.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ik.yuntaijiaju.cn

[D15] 去重
来源：http://zf.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aj.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://am.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://dp.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://mr.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ar.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xz.bookmarksfly.cn

Ruby: arr.uniq
来源：http://uw.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://wg.asd995.cn

[D16] 求和与平均值
来源：http://xa.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mh.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ee.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wr.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nv.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cb.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://vb.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vk.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://qj.shtwfgs.cn

[D17] 最大值与最小值
来源：http://hh.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://mj.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ll.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://no.colortex.cn

TS:   Math.max(...arr);
来源：http://uy.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gl.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gm.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://eu.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://sb.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://lo.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cs.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://am.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vp.huanxung.cn

TS:   nested.flat();
来源：http://wx.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mu.hahajie.cn

Go:   // 手写双层循环
来源：http://am.jctech888.com.cn

Ruby: nested.flatten
来源：http://ur.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ko.shxzskj.cn

[D19] 按字段分组
来源：http://hv.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zu.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://of.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vv.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tx.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pe.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://az.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://aw.nicolike.cn


<!-- 参考信息 -->