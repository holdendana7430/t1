代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://bv.muxihuayi.cn

[C03] 可变参数
来源：http://ey.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://lf.huanxung.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wl.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://az.szsharing.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yn.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mj.jctech888.com.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ne.9csxet.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fa.shxzukj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uj.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://je.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pq.bjjhwx.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hq.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yl.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bo.hnjuh.cn

Java: // 无：用 Builder 模式或 record
来源：http://hc.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://ug.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://um.colortex.cn

C#:   f(a: 1, b: 2)
来源：http://qq.shxzukj.cn

[C05] 返回多个值
来源：http://ph.jctech888.com.cn

Py:   return a, b
来源：http://zs.huixiangedu.cn

PHP:  return [$a, $b];
来源：http://qf.newstarts.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lv.szxytkj.cn

TS:   return { a, b };
来源：http://of.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uv.yuntaijiaju.cn

Go:   return a, b
来源：http://mt.yuntaijiaju.cn

Ruby: return a, b
来源：http://dv.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://tb.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://nv.colortex.cn

Py:   square = lambda x: x * x
来源：http://gn.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rq.gzmigu.cn

JS:   const square = x => x * x;
来源：http://nw.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://in.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://me.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://og.panjiajie.cn

Ruby: square = ->(x) { x * x }
来源：http://yf.nicolike.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tx.shtwfgs.cn

[C07] 把函数作为参数传入
来源：http://fr.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ca.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://od.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nh.panjiajie.cn

TS:   arr.map(String)
来源：http://wm.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sh.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gc.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://ik.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vv.bookmarksfly.cn

[C08] 闭包
来源：http://ah.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qf.chemitech.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://un.newstarts.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://na.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://em.jianghongdianzi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kb.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mq.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://de.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cv.9csxet.cn

[C09] 递归
来源：http://sd.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jy.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ao.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gg.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hl.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ij.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rk.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bl.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qd.shxzskj.cn

[C10] 变量作用域
来源：http://zp.bookmarksfly.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ma.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rg.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ka.wgjwhj.cn

TS:   同 JS
来源：http://mv.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://uq.chemitech.net.cn

Go:   花括号块级作用域
来源：http://kq.yuntaijiaju.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ch.bookmarksfly.cn

C#:   块级作用域
来源：http://cn.9csxet.cn

[C11] 模块导入与导出
来源：http://an.9csxet.cn

Py:   from module import func
来源：http://qq.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bs.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ff.szsharing.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rk.nszjky.cn

Java: import java.util.List;
来源：http://yb.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tx.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://mw.newstarts.cn

C#:   using System.Text;
来源：http://sb.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://ys.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://oz.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://kd.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://hy.szxytkj.cn

TS:   (() => { console.log("run"); })();
来源：http://tq.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://by.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://kv.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://xu.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ug.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://wp.wgjwhj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ho.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gm.jianghongdianzi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sb.nszjky.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hy.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xb.szsharing.cn

Go:   func add(a, b int) int
来源：http://un.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wu.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bi.colortex.cn

[C14] 泛型函数
来源：http://qo.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yc.jctech888.com.cn

PHP:  // 无泛型
来源：http://is.yuntaijiaju.cn

JS:   // 无泛型
来源：http://ni.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uq.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dl.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cr.chemitech.net.cn

Ruby: # 无泛型
来源：http://gr.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://le.szsharing.cn

[C15] 解构 / 展开参数
来源：http://bk.jianghongdianzi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://my.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://pr.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bl.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ik.jctech888.com.cn

Java: // 无解构
来源：http://ny.muxihuayi.cn

Go:   // 无解构
来源：http://jb.shtwfgs.cn

Ruby: a, b = pair
来源：http://gh.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://au.nszjky.cn

[C16] 函数 / 方法重载
来源：http://uz.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ky.szsharing.cn

PHP:  // 无重载
来源：http://hy.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kv.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://dl.szsharing.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://se.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://yl.9csxet.cn

Ruby: # 无重载：靠动态参数
来源：http://qy.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nc.colortex.cn

================================================================================
来源：http://wm.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://pi.haigaiapp.cn

================================================================================
来源：http://ze.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://ys.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qu.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zs.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rl.muxihuayi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pq.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gv.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://xd.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://yw.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ce.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://fh.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xr.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fb.gzmigu.cn

JS:   arr.push(4);
来源：http://nf.asd995.cn

TS:   arr.push(4);
来源：http://ze.nicolike.cn

Java: list.add(4);
来源：http://un.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://it.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://ea.bookmarksfly.cn

C#:   list.Add(4);
来源：http://vy.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://bw.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://wy.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cq.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iq.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://vl.panjiajie.cn

Java: list.add(0, 0);
来源：http://ug.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rj.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eq.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://xj.bjjhwx.cn

[D04] 删除元素
来源：http://xb.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bo.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lj.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ve.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://zt.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vx.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://na.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dj.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pr.jctech888.com.cn

[D05] 访问与修改元素
来源：http://vw.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zl.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xb.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zf.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://py.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://zw.wgjwhj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ih.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ie.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oh.panjiajie.cn

[D06] 数组长度
来源：http://wv.haigaiapp.cn

Py:   len(arr)
来源：http://qv.panjiajie.cn

PHP:  count($arr);
来源：http://nm.haigaiapp.cn

JS:   arr.length
来源：http://ls.nszjky.cn

TS:   arr.length
来源：http://xh.bookmarksfly.cn

Java: list.size();
来源：http://su.huixiangedu.cn

Go:   len(arr)
来源：http://lf.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://qc.9csxet.cn

C#:   list.Count;
来源：http://jp.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://wg.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zg.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dh.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://ai.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://jg.hnjuh.cn

Java: list.subList(1, 4);
来源：http://wc.bookmarksfly.cn

Go:   arr[1:4]
来源：http://lq.shxzskj.cn

Ruby: arr[1, 3]
来源：http://ww.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://rl.huixiangedu.cn

[D08] 合并两个数组
来源：http://pl.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://be.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://nt.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dw.shxzskj.cn

TS:   [...a, ...b];
来源：http://ju.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pu.lnxyls.cn

Go:   append(a, b...)
来源：http://rh.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://ws.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://uo.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://lp.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://wz.huanxung.cn

PHP:  sort($arr);
来源：http://rf.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rz.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://su.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ah.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ku.newstarts.cn

Ruby: arr.sort
来源：http://et.shxzukj.cn

C#:   list.Sort();
来源：http://ix.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mq.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jb.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ly.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bu.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yk.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nh.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ew.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://em.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iw.yuexingan06.cn

[D11] 反转数组
来源：http://tb.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wz.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://li.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mk.newstarts.cn

TS:   [...arr].reverse();
来源：http://aj.shxzskj.cn

Java: Collections.reverse(list);
来源：http://tm.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://qe.hnjuh.cn

Ruby: arr.reverse
来源：http://qv.szxytkj.cn

C#:   list.Reverse();
来源：http://hn.muxihuayi.cn

[D12] 查找元素下标
来源：http://rm.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://bi.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zq.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qy.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pu.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tt.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://fz.nszjky.cn

Ruby: arr.index(x)
来源：http://rp.lnxyls.cn

C#:   list.IndexOf(x);
来源：http://fi.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://lk.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xk.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://de.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://yl.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://ig.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qa.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qd.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sn.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sy.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://dl.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ib.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ca.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://fm.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://ip.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zt.muxihuayi.cn

Go:   // 手写循环
来源：http://xm.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ow.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pg.nszjky.cn

[D15] 去重
来源：http://aq.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vn.shxzskj.cn

PHP:  array_unique($arr);
来源：http://jf.hahajie.cn

JS:   [...new Set(arr)]
来源：http://zn.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://pv.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uf.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xl.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://hf.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://up.nicolike.cn

[D16] 求和与平均值
来源：http://wu.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jh.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vp.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hs.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://th.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ib.huixiangedu.cn

Go:   // 手写循环累加
来源：http://vd.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wj.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://nt.hnjuh.cn

[D17] 最大值与最小值
来源：http://af.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://cl.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://yy.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bc.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://yl.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tx.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gr.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://mq.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://yg.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://vf.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mq.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://uv.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zj.newstarts.cn

TS:   nested.flat();
来源：http://tr.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cs.chemitech.net.cn

Go:   // 手写双层循环
来源：http://nn.shxzukj.cn

Ruby: nested.flatten
来源：http://iw.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xu.jctech888.com.cn

[D19] 按字段分组
来源：http://na.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ba.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ze.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://my.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zk.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ao.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://wd.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lx.hnjuh.cn


<!-- 参考信息 -->