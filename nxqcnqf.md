代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://vi.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ax.jianghongdianzi.cn

Ruby: def add(a, b); a + b; end
来源：http://oy.colortex.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tz.panjiajie.cn

[C02] 默认参数
来源：http://hw.asd995.cn

Py:   def greet(name="World"): return name
来源：http://sl.yuntaijiaju.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yb.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://hp.colortex.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lu.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jo.jctech888.com.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mf.shxzukj.cn

Ruby: def greet(name = "World") = name
来源：http://pb.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://bc.nicolike.cn

[C03] 可变参数
来源：http://st.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://fj.szxytkj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cc.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sd.lnxyls.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yj.szxytkj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xg.newstarts.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xw.szxytkj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nq.hnjuh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xz.asd995.cn

[C04] 命名参数 / 关键字参数
来源：http://te.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uh.hnjuh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fa.huixiangedu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ky.yuntaijiaju.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://we.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://nv.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://jf.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://ht.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://zf.asd995.cn

[C05] 返回多个值
来源：http://ff.bjjhwx.cn

Py:   return a, b
来源：http://jd.panjiajie.cn

PHP:  return [$a, $b];
来源：http://be.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pp.muxihuayi.cn

TS:   return { a, b };
来源：http://tk.hnjuh.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cg.panjiajie.cn

Go:   return a, b
来源：http://gg.yuntaijiaju.cn

Ruby: return a, b
来源：http://ym.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://dq.colortex.cn

[C06] 匿名函数 / lambda
来源：http://xr.colortex.cn

Py:   square = lambda x: x * x
来源：http://fz.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kv.asd995.cn

JS:   const square = x => x * x;
来源：http://ep.newstarts.cn

TS:   const square = (x: number): number => x * x;
来源：http://dr.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rk.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sd.haigaiapp.cn

Ruby: square = ->(x) { x * x }
来源：http://yy.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yp.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://wq.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yd.haigaiapp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://by.hahajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://as.nicolike.cn

TS:   arr.map(String)
来源：http://md.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sh.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yr.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://rk.newstarts.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qk.huixiangedu.cn

[C08] 闭包
来源：http://mj.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ku.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nk.muxihuayi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lx.szxytkj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tp.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ih.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rh.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sp.haigaiapp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://is.521024.cn

[C09] 递归
来源：http://vz.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ig.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rp.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kx.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qo.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iu.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rq.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ol.521024.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iy.yuntaijiaju.cn

[C10] 变量作用域
来源：http://yz.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oy.szxytkj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ov.bjjhwx.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yb.yuntaijiaju.cn

TS:   同 JS
来源：http://th.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://mn.newstarts.cn

Go:   花括号块级作用域
来源：http://ka.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ev.nszjky.cn

C#:   块级作用域
来源：http://qu.9csxet.cn

[C11] 模块导入与导出
来源：http://tm.muxihuayi.cn

Py:   from module import func
来源：http://jt.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mp.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sr.huixiangedu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://is.gzmigu.cn

Java: import java.util.List;
来源：http://pt.haigaiapp.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hi.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://yy.haigaiapp.cn

C#:   using System.Text;
来源：http://mw.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://rz.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://aj.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://zc.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://ve.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://tt.jianghongdianzi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jz.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://mq.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://qm.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ln.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://kt.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fx.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yv.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eh.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iu.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://as.panjiajie.cn

Go:   func add(a, b int) int
来源：http://tq.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hr.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sw.szsharing.cn

[C14] 泛型函数
来源：http://fc.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tt.asd995.cn

PHP:  // 无泛型
来源：http://ix.jianghongdianzi.cn

JS:   // 无泛型
来源：http://hs.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qa.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mn.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yb.asd995.cn

Ruby: # 无泛型
来源：http://cn.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ho.shxzukj.cn

[C15] 解构 / 展开参数
来源：http://ig.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nc.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://mj.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iu.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nh.shxzskj.cn

Java: // 无解构
来源：http://lt.chemitech.net.cn

Go:   // 无解构
来源：http://je.gzmigu.cn

Ruby: a, b = pair
来源：http://aa.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://vp.9csxet.cn

[C16] 函数 / 方法重载
来源：http://gh.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qu.huixiangedu.cn

PHP:  // 无重载
来源：http://ol.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lz.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://mz.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yd.521024.cn

Go:   // 无重载：用不同函数名
来源：http://xb.yuexingan06.cn

Ruby: # 无重载：靠动态参数
来源：http://ym.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://we.jctech888.com.cn

================================================================================
来源：http://ip.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://kg.jctech888.com.cn

================================================================================
来源：http://us.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://ls.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ov.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aw.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hn.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wk.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sv.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://cs.huixinmuqiang.cn

Ruby: arr = [1, 2, 3]
来源：http://zo.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vw.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://au.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://li.wgjwhj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nv.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ct.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://pd.shxzukj.cn

Java: list.add(4);
来源：http://hh.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://dq.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://lt.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://vs.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://wl.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://fc.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bf.9csxet.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yd.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://zl.hahajie.cn

Java: list.add(0, 0);
来源：http://ky.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://um.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://os.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://bs.9csxet.cn

[D04] 删除元素
来源：http://hj.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lm.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zo.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://er.colortex.cn

TS:   arr.splice(0, 1);
来源：http://os.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ac.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://td.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dz.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nt.szxytkj.cn

[D05] 访问与修改元素
来源：http://tg.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nk.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iw.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nq.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://sq.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://me.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://em.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zm.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wq.szxytkj.cn

[D06] 数组长度
来源：http://ug.yuntaijiaju.cn

Py:   len(arr)
来源：http://hn.bjjhwx.cn

PHP:  count($arr);
来源：http://ya.shxzskj.cn

JS:   arr.length
来源：http://op.lnxyls.cn

TS:   arr.length
来源：http://qd.yuntaijiaju.cn

Java: list.size();
来源：http://db.huixinmuqiang.cn

Go:   len(arr)
来源：http://be.szsharing.cn

Ruby: arr.length; arr.size
来源：http://wa.szxytkj.cn

C#:   list.Count;
来源：http://ha.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://iw.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ot.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qu.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://oa.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://uh.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://rj.gzmigu.cn

Go:   arr[1:4]
来源：http://qe.hnjuh.cn

Ruby: arr[1, 3]
来源：http://et.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ms.newstarts.cn

[D08] 合并两个数组
来源：http://qi.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://az.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://uu.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tb.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://fa.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://du.szsharing.cn

Go:   append(a, b...)
来源：http://qr.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://ft.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://jc.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://aj.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://ft.521024.cn

PHP:  sort($arr);
来源：http://tq.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ck.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ua.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iq.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gp.colortex.cn

Ruby: arr.sort
来源：http://ew.shxzukj.cn

C#:   list.Sort();
来源：http://kt.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ls.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dc.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tp.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://om.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ag.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wc.chemitech.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://in.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://by.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mw.newstarts.cn

[D11] 反转数组
来源：http://th.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hn.haigaiapp.cn

PHP:  array_reverse($arr);
来源：http://el.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nj.newstarts.cn

TS:   [...arr].reverse();
来源：http://yk.nszjky.cn

Java: Collections.reverse(list);
来源：http://fh.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://if.haigaiapp.cn

Ruby: arr.reverse
来源：http://ji.huixiangedu.cn

C#:   list.Reverse();
来源：http://ee.huixiangedu.cn

[D12] 查找元素下标
来源：http://gt.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://nw.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vq.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nf.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://py.nszjky.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lk.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://vw.shxzukj.cn

Ruby: arr.index(x)
来源：http://ly.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://mx.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://mt.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qy.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sn.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://mm.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://uc.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sx.bookmarksfly.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iv.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hr.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pz.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://ym.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vf.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bb.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://yk.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://no.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://if.szxytkj.cn

Go:   // 手写循环
来源：http://di.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vg.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ym.chemitech.net.cn

[D15] 去重
来源：http://tr.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://op.nicolike.cn

PHP:  array_unique($arr);
来源：http://ah.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://lr.9csxet.cn

TS:   [...new Set(arr)]
来源：http://se.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tw.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://mt.shxzukj.cn

Ruby: arr.uniq
来源：http://mj.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://sl.muxihuayi.cn

[D16] 求和与平均值
来源：http://es.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wl.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://te.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wv.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dn.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bn.9csxet.cn

Go:   // 手写循环累加
来源：http://nz.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://on.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://ju.wgjwhj.cn

[D17] 最大值与最小值
来源：http://xr.asd995.cn

Py:   max(arr);  min(arr)
来源：http://ti.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://dy.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zu.nszjky.cn

TS:   Math.max(...arr);
来源：http://mk.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uv.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oa.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://ey.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://gm.colortex.cn

[D18] 扁平化嵌套数组
来源：http://oh.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ra.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://kz.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ns.lnxyls.cn

TS:   nested.flat();
来源：http://zn.shtwfgs.cn


<!-- 参考信息 -->