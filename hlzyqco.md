代发 wailian999

Py:   def add(a, b): return a + b
来源：http://wq.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zw.lnxyls.cn

JS:   function add(a, b) { return a + b; }
来源：http://oi.colortex.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ok.shxzskj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://la.hnjuh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pt.nicolike.cn

Ruby: def add(a, b); a + b; end
来源：http://ir.chemitech.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gt.huixinmuqiang.cn

[C02] 默认参数
来源：http://db.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://vm.bjjhwx.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qn.muxihuayi.cn

JS:   function greet(name = "World") { return name; }
来源：http://au.jctech888.com.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wz.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hd.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ld.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://we.szsharing.cn

C#:   string Greet(string name = "World") => name;
来源：http://gh.nicolike.cn

[C03] 可变参数
来源：http://vl.bjjhwx.cn

Py:   def total(*args): return sum(args)
来源：http://ir.hahajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ht.huixiangedu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://as.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cp.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ux.jianghongdianzi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yr.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tf.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nm.shtwfgs.cn

[C04] 命名参数 / 关键字参数
来源：http://ol.gzmigu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zg.szsharing.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dz.gzmigu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kv.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wq.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://xy.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://td.nicolike.cn

Ruby: f(a: 1, b: 2)
来源：http://xo.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://kf.shtwfgs.cn

[C05] 返回多个值
来源：http://gl.jianghongdianzi.cn

Py:   return a, b
来源：http://ow.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://ez.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://je.muxihuayi.cn

TS:   return { a, b };
来源：http://ma.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qj.colortex.cn

Go:   return a, b
来源：http://ke.colortex.cn

Ruby: return a, b
来源：http://cg.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://uu.huanxung.cn

[C06] 匿名函数 / lambda
来源：http://un.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://dd.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://au.gzmigu.cn

JS:   const square = x => x * x;
来源：http://st.shxzskj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ec.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tw.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zc.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://db.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yk.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://jn.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zm.bjjhwx.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ir.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://is.panjiajie.cn

TS:   arr.map(String)
来源：http://zs.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wk.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bk.nicolike.cn

Ruby: arr.map(&:upcase)
来源：http://pz.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xe.asd995.cn

[C08] 闭包
来源：http://fj.huixinmuqiang.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cz.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nw.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fa.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ny.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ni.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://la.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://za.asd995.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pz.shtwfgs.cn

[C09] 递归
来源：http://bi.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vy.jctech888.com.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ml.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dx.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ps.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wg.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gm.lnxyls.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qk.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ir.bjjhwx.cn

[C10] 变量作用域
来源：http://ig.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yy.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jy.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oi.asd995.cn

TS:   同 JS
来源：http://jk.jianghongdianzi.cn

Java: 方法内为块级作用域
来源：http://vw.hnjuh.cn

Go:   花括号块级作用域
来源：http://jt.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dt.panjiajie.cn

C#:   块级作用域
来源：http://us.szxytkj.cn

[C11] 模块导入与导出
来源：http://mo.wgjwhj.cn

Py:   from module import func
来源：http://xt.hnjuh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jq.huanxung.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qu.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gk.jianghongdianzi.cn

Java: import java.util.List;
来源：http://vg.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://op.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://ft.huanxung.cn

C#:   using System.Text;
来源：http://ny.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ub.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://wa.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://mb.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ne.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://ts.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lt.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://aj.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://bb.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xd.colortex.cn

[C13] 类型声明 / 类型注解
来源：http://ig.asd995.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kk.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hn.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vz.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bf.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yr.nszjky.cn

Go:   func add(a, b int) int
来源：http://lv.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lz.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vp.jctech888.com.cn

[C14] 泛型函数
来源：http://mb.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qb.chemitech.net.cn

PHP:  // 无泛型
来源：http://cy.huixiangedu.cn

JS:   // 无泛型
来源：http://hk.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vz.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dc.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gs.colortex.cn

Ruby: # 无泛型
来源：http://yx.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vc.wgjwhj.cn

[C15] 解构 / 展开参数
来源：http://tw.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cd.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://uc.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cb.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tj.shxzukj.cn

Java: // 无解构
来源：http://cr.huanxung.cn

Go:   // 无解构
来源：http://xx.9csxet.cn

Ruby: a, b = pair
来源：http://qf.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://mm.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://nx.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nn.hnjuh.cn

PHP:  // 无重载
来源：http://yg.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://no.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://bq.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lc.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://cl.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://og.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ke.szsharing.cn

================================================================================
来源：http://dt.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://yb.jctech888.com.cn

================================================================================
来源：http://mk.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://cy.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xx.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sc.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qo.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ge.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mb.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://cz.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://me.muxihuayi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ve.hnjuh.cn

[D02] 追加元素到末尾
来源：http://nt.9csxet.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rd.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vr.nicolike.cn

JS:   arr.push(4);
来源：http://kg.shxzukj.cn

TS:   arr.push(4);
来源：http://bf.bjjhwx.cn

Java: list.add(4);
来源：http://dm.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://dd.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://ke.muxihuayi.cn

C#:   list.Add(4);
来源：http://fv.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://js.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://ml.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fk.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kk.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://yz.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://dq.521024.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rh.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cn.521024.cn

C#:   list.Insert(0, 0);
来源：http://vs.shxzskj.cn

[D04] 删除元素
来源：http://hw.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pf.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ge.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ap.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://fm.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://md.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ps.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ye.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fk.haigaiapp.cn

[D05] 访问与修改元素
来源：http://ko.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yp.newstarts.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ja.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zg.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://iz.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://lk.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://qs.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gu.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oh.muxihuayi.cn

[D06] 数组长度
来源：http://vd.huixinmuqiang.cn

Py:   len(arr)
来源：http://ca.szxytkj.cn

PHP:  count($arr);
来源：http://jw.shxzukj.cn

JS:   arr.length
来源：http://qj.asd995.cn

TS:   arr.length
来源：http://fg.hnjuh.cn

Java: list.size();
来源：http://nc.hnjuh.cn

Go:   len(arr)
来源：http://pb.9csxet.cn

Ruby: arr.length; arr.size
来源：http://ug.wgjwhj.cn

C#:   list.Count;
来源：http://ru.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://xa.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://io.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rh.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://nx.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://kr.colortex.cn

Java: list.subList(1, 4);
来源：http://nm.chemitech.net.cn

Go:   arr[1:4]
来源：http://lu.chemitech.net.cn

Ruby: arr[1, 3]
来源：http://yh.lnxyls.cn

C#:   list.GetRange(1, 3);
来源：http://fy.haigaiapp.cn

[D08] 合并两个数组
来源：http://ut.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://ik.huanxung.cn

PHP:  array_merge($a, $b);
来源：http://wp.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sq.nicolike.cn

TS:   [...a, ...b];
来源：http://fy.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pm.hnjuh.cn

Go:   append(a, b...)
来源：http://sf.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://rh.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://xu.bjjhwx.cn

[D09] 排序（升序）
来源：http://yi.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://fe.521024.cn

PHP:  sort($arr);
来源：http://ww.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cq.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ka.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kc.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://do.asd995.cn

Ruby: arr.sort
来源：http://xl.szsharing.cn

C#:   list.Sort();
来源：http://pn.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uk.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yx.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qk.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ya.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fe.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ie.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ap.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fj.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zt.panjiajie.cn

[D11] 反转数组
来源：http://yg.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bx.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://uz.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kr.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://wh.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://gy.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://qc.szxytkj.cn

Ruby: arr.reverse
来源：http://ek.gzmigu.cn

C#:   list.Reverse();
来源：http://oa.gzmigu.cn

[D12] 查找元素下标
来源：http://ix.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://if.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sn.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://to.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gg.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dk.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://ka.shtwfgs.cn

Ruby: arr.index(x)
来源：http://rz.colortex.cn

C#:   list.IndexOf(x);
来源：http://rh.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://yd.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mk.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ur.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://db.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://bq.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yj.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uv.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jz.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nm.chemitech.net.cn

[D14] 映射转换（每个元素变形）
来源：http://fl.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kq.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jv.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ax.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://xu.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ug.shxzukj.cn

Go:   // 手写循环
来源：http://pb.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qc.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wd.newstarts.cn

[D15] 去重
来源：http://ct.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cw.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://pu.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://hw.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://oq.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ih.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dn.colortex.cn

Ruby: arr.uniq
来源：http://fx.colortex.cn

C#:   list.Distinct().ToList()
来源：http://ya.shxzskj.cn

[D16] 求和与平均值
来源：http://lr.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://er.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lu.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sm.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iw.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dm.asd995.cn

Go:   // 手写循环累加
来源：http://cn.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mr.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://us.muxihuayi.cn

[D17] 最大值与最小值
来源：http://hs.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://km.521024.cn

PHP:  max($arr);  min($arr);
来源：http://bq.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qr.9csxet.cn

TS:   Math.max(...arr);
来源：http://jd.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cg.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pm.521024.cn

Ruby: arr.max;  arr.min
来源：http://fb.colortex.cn

C#:   list.Max();  list.Min()
来源：http://ok.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://sn.yuexingan06.cn


<!-- 参考信息 -->