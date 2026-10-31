代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://gm.szsharing.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ca.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://ce.haigaiapp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zt.lnxyls.cn

[C02] 默认参数
来源：http://fp.asd995.cn

Py:   def greet(name="World"): return name
来源：http://ry.huixinmuqiang.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gi.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://br.newstarts.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://li.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ei.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jv.hnjuh.cn

Ruby: def greet(name = "World") = name
来源：http://iu.huixiangedu.cn

C#:   string Greet(string name = "World") => name;
来源：http://mm.newstarts.cn

[C03] 可变参数
来源：http://sn.nicolike.cn

Py:   def total(*args): return sum(args)
来源：http://qf.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ih.newstarts.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lt.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ne.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mw.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ir.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pg.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://go.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://ew.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hc.huixiangedu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://es.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eu.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://od.yuntaijiaju.cn

Java: // 无：用 Builder 模式或 record
来源：http://le.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://ia.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://hj.szxytkj.cn

C#:   f(a: 1, b: 2)
来源：http://nb.chemitech.net.cn

[C05] 返回多个值
来源：http://xy.haigaiapp.cn

Py:   return a, b
来源：http://om.colortex.cn

PHP:  return [$a, $b];
来源：http://jy.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ud.colortex.cn

TS:   return { a, b };
来源：http://ed.bjjhwx.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xb.jctech888.com.cn

Go:   return a, b
来源：http://zs.yuntaijiaju.cn

Ruby: return a, b
来源：http://nm.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://mg.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://uv.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://oa.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mx.521024.cn

JS:   const square = x => x * x;
来源：http://gz.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://kv.wgjwhj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wq.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nx.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://qo.newstarts.cn

C#:   Func<int, int> square = x => x * x;
来源：http://we.bookmarksfly.cn

[C07] 把函数作为参数传入
来源：http://ed.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vk.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://br.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wg.panjiajie.cn

TS:   arr.map(String)
来源：http://xj.panjiajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ob.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ks.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://bq.lnxyls.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gd.newstarts.cn

[C08] 闭包
来源：http://vr.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gi.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ti.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mu.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vb.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://up.bookmarksfly.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://di.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dw.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ob.bjjhwx.cn

[C09] 递归
来源：http://so.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bh.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ih.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wk.asd995.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sw.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zq.shxzukj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gz.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dw.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wp.huixiangedu.cn

[C10] 变量作用域
来源：http://yv.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gq.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ud.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ka.wgjwhj.cn

TS:   同 JS
来源：http://na.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ku.shxzskj.cn

Go:   花括号块级作用域
来源：http://jx.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jw.hahajie.cn

C#:   块级作用域
来源：http://rl.hnjuh.cn

[C11] 模块导入与导出
来源：http://ew.asd995.cn

Py:   from module import func
来源：http://ai.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kq.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mk.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jn.shxzskj.cn

Java: import java.util.List;
来源：http://th.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zf.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://ui.newstarts.cn

C#:   using System.Text;
来源：http://yw.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://da.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://ax.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://uh.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://ew.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://df.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rq.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://og.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://do.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qx.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://ck.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qk.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bk.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gh.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sz.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tv.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://il.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ja.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cc.yuntaijiaju.cn

[C14] 泛型函数
来源：http://wc.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vy.521024.cn

PHP:  // 无泛型
来源：http://pr.huixinmuqiang.cn

JS:   // 无泛型
来源：http://lk.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nn.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kk.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kg.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://vj.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pn.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://pb.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rt.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://jf.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xn.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rs.jctech888.com.cn

Java: // 无解构
来源：http://nf.panjiajie.cn

Go:   // 无解构
来源：http://rv.chemitech.net.cn

Ruby: a, b = pair
来源：http://jb.yuntaijiaju.cn

C#:   var (a, b) = pair;
来源：http://gx.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://nr.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://we.newstarts.cn

PHP:  // 无重载
来源：http://zd.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qy.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://uy.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://se.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://us.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://xe.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ci.huanxung.cn

================================================================================
来源：http://by.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://fv.muxihuayi.cn

================================================================================
来源：http://vq.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://cd.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pm.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oy.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jl.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nj.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aq.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://ty.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://sa.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ll.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://np.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uu.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nicolike.cn

JS:   arr.push(4);
来源：http://tt.newstarts.cn

TS:   arr.push(4);
来源：http://nn.newstarts.cn

Java: list.add(4);
来源：http://iu.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://ln.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://uu.yuexingan06.cn

C#:   list.Add(4);
来源：http://xu.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://qs.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://xt.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gb.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wh.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://uj.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://al.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ns.huixinmuqiang.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://on.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://zf.bookmarksfly.cn

[D04] 删除元素
来源：http://cy.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mb.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ht.chemitech.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zj.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://xq.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rx.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uz.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jc.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ym.chemitech.net.cn

[D05] 访问与修改元素
来源：http://dn.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hw.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ti.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tn.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://at.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://cp.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://io.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kh.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qg.huanxung.cn

[D06] 数组长度
来源：http://nr.chemitech.net.cn

Py:   len(arr)
来源：http://ip.shtwfgs.cn

PHP:  count($arr);
来源：http://dy.bookmarksfly.cn

JS:   arr.length
来源：http://yt.hahajie.cn

TS:   arr.length
来源：http://qt.chemitech.net.cn

Java: list.size();
来源：http://dy.asd995.cn

Go:   len(arr)
来源：http://ix.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://lz.asd995.cn

C#:   list.Count;
来源：http://pi.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://kk.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ad.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ok.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://zf.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://dx.huanxung.cn

Java: list.subList(1, 4);
来源：http://yk.chemitech.net.cn

Go:   arr[1:4]
来源：http://ml.newstarts.cn

Ruby: arr[1, 3]
来源：http://tt.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://ng.gzmigu.cn

[D08] 合并两个数组
来源：http://yf.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://qx.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://cu.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kh.yuexingan06.cn

TS:   [...a, ...b];
来源：http://oa.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yc.yuexingan06.cn

Go:   append(a, b...)
来源：http://ca.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://ij.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://ox.nszjky.cn

[D09] 排序（升序）
来源：http://io.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jw.shxzskj.cn

PHP:  sort($arr);
来源：http://qm.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kl.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fh.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oo.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cl.gzmigu.cn

Ruby: arr.sort
来源：http://ub.shxzukj.cn

C#:   list.Sort();
来源：http://ej.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bp.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yy.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://db.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ow.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lr.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ne.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zu.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aw.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yf.szxytkj.cn

[D11] 反转数组
来源：http://ey.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dd.hahajie.cn

PHP:  array_reverse($arr);
来源：http://is.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ih.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://qn.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://br.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://fv.huixiangedu.cn

Ruby: arr.reverse
来源：http://al.huanxung.cn

C#:   list.Reverse();
来源：http://wx.521024.cn

[D12] 查找元素下标
来源：http://fu.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://sp.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iz.nicolike.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fg.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rg.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lp.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://gk.hahajie.cn

Ruby: arr.index(x)
来源：http://lx.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://gw.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://tw.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ra.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ps.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://ia.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://es.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kg.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iu.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ia.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kj.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://fj.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vv.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fv.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://nf.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://hp.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bx.wgjwhj.cn

Go:   // 手写循环
来源：http://na.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lf.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pk.nszjky.cn

[D15] 去重
来源：http://tp.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zw.newstarts.cn

PHP:  array_unique($arr);
来源：http://xt.hahajie.cn

JS:   [...new Set(arr)]
来源：http://zj.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://dg.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qm.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ga.nicolike.cn

Ruby: arr.uniq
来源：http://ap.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://zq.shtwfgs.cn

[D16] 求和与平均值
来源：http://gk.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fn.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kf.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mt.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kl.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zc.shxzukj.cn

Go:   // 手写循环累加
来源：http://nw.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zo.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://pk.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://gz.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://oo.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://cc.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ml.shxzskj.cn

TS:   Math.max(...arr);
来源：http://oy.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://re.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fq.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://kx.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://fk.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://re.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sj.asd995.cn

PHP:  array_merge(...$nested);
来源：http://uz.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ym.bookmarksfly.cn

TS:   nested.flat();
来源：http://du.yuexingan06.cn


<!-- 参考信息 -->