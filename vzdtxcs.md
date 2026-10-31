代发 wailian999

[C02] 默认参数
来源：http://gt.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://rf.panjiajie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zs.9csxet.cn

JS:   function greet(name = "World") { return name; }
来源：http://ip.nszjky.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://id.wgjwhj.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://us.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ux.jianghongdianzi.cn

Ruby: def greet(name = "World") = name
来源：http://no.yuexingan06.cn

C#:   string Greet(string name = "World") => name;
来源：http://sz.hnjuh.cn

[C03] 可变参数
来源：http://ib.shxzukj.cn

Py:   def total(*args): return sum(args)
来源：http://cc.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tn.muxihuayi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://on.jianghongdianzi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ec.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dt.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dl.shxzskj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xy.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xd.wgjwhj.cn

[C04] 命名参数 / 关键字参数
来源：http://uq.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mb.bookmarksfly.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cw.szsharing.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kx.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gc.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://lq.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://nc.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://mc.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://ox.bjjhwx.cn

[C05] 返回多个值
来源：http://hj.nszjky.cn

Py:   return a, b
来源：http://cm.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://fn.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ly.bookmarksfly.cn

TS:   return { a, b };
来源：http://wb.yuexingan06.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wt.shtwfgs.cn

Go:   return a, b
来源：http://wv.jctech888.com.cn

Ruby: return a, b
来源：http://te.huixinmuqiang.cn

C#:   return (a, b);              // ValueTuple
来源：http://yl.521024.cn

[C06] 匿名函数 / lambda
来源：http://xl.newstarts.cn

Py:   square = lambda x: x * x
来源：http://tt.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://iu.bookmarksfly.cn

JS:   const square = x => x * x;
来源：http://lf.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://ih.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kk.wgjwhj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hy.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://qe.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ga.jianghongdianzi.cn

[C07] 把函数作为参数传入
来源：http://tw.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fr.huixiangedu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ya.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kf.gzmigu.cn

TS:   arr.map(String)
来源：http://oa.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xc.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zs.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://ht.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qu.panjiajie.cn

[C08] 闭包
来源：http://vp.shxzskj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ho.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tg.szsharing.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mz.yuexingan06.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://we.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yq.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ag.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jt.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vk.bjjhwx.cn

[C09] 递归
来源：http://me.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xw.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bu.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vc.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mc.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ih.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pl.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vv.521024.cn

[C10] 变量作用域
来源：http://yh.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xn.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fx.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://do.jianghongdianzi.cn

TS:   同 JS
来源：http://ei.newstarts.cn

Java: 方法内为块级作用域
来源：http://gc.wgjwhj.cn

Go:   花括号块级作用域
来源：http://rh.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nv.haigaiapp.cn

C#:   块级作用域
来源：http://vg.huanxung.cn

[C11] 模块导入与导出
来源：http://hn.521024.cn

Py:   from module import func
来源：http://uu.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qd.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://iz.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bw.bookmarksfly.cn

Java: import java.util.List;
来源：http://ys.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xc.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://zl.wgjwhj.cn

C#:   using System.Text;
来源：http://rp.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://oz.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://rh.huanxung.cn

PHP:  (function () { echo "run"; })();
来源：http://aq.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://ew.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://eh.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fv.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://qq.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://jb.yuntaijiaju.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://an.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://tq.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kp.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kp.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ay.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lo.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bx.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://cw.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zb.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fw.huanxung.cn

[C14] 泛型函数
来源：http://af.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rl.hnjuh.cn

PHP:  // 无泛型
来源：http://ku.huixinmuqiang.cn

JS:   // 无泛型
来源：http://pu.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lz.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hm.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ge.colortex.cn

Ruby: # 无泛型
来源：http://tk.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wv.newstarts.cn

[C15] 解构 / 展开参数
来源：http://tp.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fo.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://ls.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hw.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zj.shxzukj.cn

Java: // 无解构
来源：http://qu.nszjky.cn

Go:   // 无解构
来源：http://gr.nszjky.cn

Ruby: a, b = pair
来源：http://iz.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://ya.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://gr.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bz.muxihuayi.cn

PHP:  // 无重载
来源：http://iz.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dz.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://vv.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xi.muxihuayi.cn

Go:   // 无重载：用不同函数名
来源：http://nh.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://it.szxytkj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ft.9csxet.cn

================================================================================
来源：http://bv.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://ga.shxzukj.cn

================================================================================
来源：http://jj.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://kc.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://io.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bz.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oo.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rl.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hk.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://fb.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://yv.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sq.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://wv.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pk.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zp.nszjky.cn

JS:   arr.push(4);
来源：http://hv.wgjwhj.cn

TS:   arr.push(4);
来源：http://sw.haigaiapp.cn

Java: list.add(4);
来源：http://gt.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://ef.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://jh.9csxet.cn

C#:   list.Add(4);
来源：http://ww.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://sp.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://wk.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jz.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vx.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://we.shtwfgs.cn

Java: list.add(0, 0);
来源：http://ea.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rv.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rb.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://yz.chemitech.net.cn

[D04] 删除元素
来源：http://oy.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wt.gzmigu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tb.9csxet.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xa.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://ij.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cd.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uv.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ov.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wk.bjjhwx.cn

[D05] 访问与修改元素
来源：http://tr.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jb.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://do.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zq.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://fp.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://tn.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ys.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fj.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://me.haigaiapp.cn

[D06] 数组长度
来源：http://jm.521024.cn

Py:   len(arr)
来源：http://xr.nszjky.cn

PHP:  count($arr);
来源：http://gf.huixiangedu.cn

JS:   arr.length
来源：http://at.huixinmuqiang.cn

TS:   arr.length
来源：http://be.jctech888.com.cn

Java: list.size();
来源：http://db.panjiajie.cn

Go:   len(arr)
来源：http://hy.huanxung.cn

Ruby: arr.length; arr.size
来源：http://ch.jctech888.com.cn

C#:   list.Count;
来源：http://dl.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://ws.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fm.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://df.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://tj.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://fi.shxzskj.cn

Java: list.subList(1, 4);
来源：http://jb.jctech888.com.cn

Go:   arr[1:4]
来源：http://bz.panjiajie.cn

Ruby: arr[1, 3]
来源：http://vy.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://ji.bookmarksfly.cn

[D08] 合并两个数组
来源：http://ob.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://rz.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://ej.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hh.nicolike.cn

TS:   [...a, ...b];
来源：http://gx.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xp.521024.cn

Go:   append(a, b...)
来源：http://pf.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://eh.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://cq.szsharing.cn

[D09] 排序（升序）
来源：http://uy.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://vu.gzmigu.cn

PHP:  sort($arr);
来源：http://nx.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dr.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://co.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ds.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jq.gzmigu.cn

Ruby: arr.sort
来源：http://ha.shxzskj.cn

C#:   list.Sort();
来源：http://pw.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fb.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ln.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://au.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ms.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://co.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ji.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ec.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ko.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bs.yuexingan06.cn

[D11] 反转数组
来源：http://ps.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ow.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://fj.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qx.shxzukj.cn

TS:   [...arr].reverse();
来源：http://gp.lnxyls.cn

Java: Collections.reverse(list);
来源：http://iu.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://qf.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://dt.asd995.cn

C#:   list.Reverse();
来源：http://yo.bookmarksfly.cn

[D12] 查找元素下标
来源：http://bm.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://sb.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jq.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qa.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pc.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fn.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://tw.shtwfgs.cn

Ruby: arr.index(x)
来源：http://zj.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://cq.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://ry.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://km.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://us.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://dq.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://gm.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://om.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bs.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kp.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ew.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://mu.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ed.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mb.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://rl.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://rl.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nx.shxzukj.cn

Go:   // 手写循环
来源：http://dn.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ur.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lm.bookmarksfly.cn

[D15] 去重
来源：http://cb.bookmarksfly.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kr.lnxyls.cn

PHP:  array_unique($arr);
来源：http://vy.nicolike.cn

JS:   [...new Set(arr)]
来源：http://gl.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://wu.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jd.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wc.chemitech.net.cn

Ruby: arr.uniq
来源：http://nw.panjiajie.cn

C#:   list.Distinct().ToList()
来源：http://ue.521024.cn

[D16] 求和与平均值
来源：http://vd.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vc.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kh.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ha.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nm.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lt.bjjhwx.cn

Go:   // 手写循环累加
来源：http://pr.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ut.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://kg.hahajie.cn

[D17] 最大值与最小值
来源：http://ki.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://dh.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ng.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://db.9csxet.cn

TS:   Math.max(...arr);
来源：http://ge.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dz.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uu.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://uw.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://hx.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://ff.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rt.521024.cn

PHP:  array_merge(...$nested);
来源：http://ff.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vt.nszjky.cn

TS:   nested.flat();
来源：http://jx.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sf.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://kr.shxzskj.cn

Ruby: nested.flatten
来源：http://az.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ja.nicolike.cn


<!-- 参考信息 -->