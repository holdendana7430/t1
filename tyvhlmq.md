代发 wailian999

Java: if (data == null) return;
来源：http://sn.lnxyls.cn

Go:   if data == nil { return }
来源：http://pu.yuexingan06.cn

Ruby: return if data.nil?
来源：http://gp.shxzskj.cn

C#:   if (data == null) return;
来源：http://ld.nicolike.cn

================================================================================
来源：http://be.huanxung.cn

C. 函数与作用域
来源：http://cl.gzmigu.cn

================================================================================
来源：http://fa.panjiajie.cn

[C01] 定义函数
来源：http://uc.yuexingan06.cn

Py:   def add(a, b): return a + b
来源：http://zm.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fy.szxytkj.cn

JS:   function add(a, b) { return a + b; }
来源：http://wz.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ox.shxzukj.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dr.colortex.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yi.bookmarksfly.cn

Ruby: def add(a, b); a + b; end
来源：http://mj.lnxyls.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jf.gzmigu.cn

[C02] 默认参数
来源：http://ua.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://du.asd995.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://te.wgjwhj.cn

JS:   function greet(name = "World") { return name; }
来源：http://pd.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qs.chemitech.net.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hm.szsharing.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qd.nszjky.cn

Ruby: def greet(name = "World") = name
来源：http://ps.huanxung.cn

C#:   string Greet(string name = "World") => name;
来源：http://we.nszjky.cn

[C03] 可变参数
来源：http://xb.hnjuh.cn

Py:   def total(*args): return sum(args)
来源：http://vr.huixiangedu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vj.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sc.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://so.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yk.nszjky.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ba.huixiangedu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://eq.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mo.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://km.hahajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xx.521024.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nh.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ut.muxihuayi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fd.nszjky.cn

Java: // 无：用 Builder 模式或 record
来源：http://yj.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://oj.jianghongdianzi.cn

Ruby: f(a: 1, b: 2)
来源：http://fr.shtwfgs.cn

C#:   f(a: 1, b: 2)
来源：http://sp.szsharing.cn

[C05] 返回多个值
来源：http://tt.wgjwhj.cn

Py:   return a, b
来源：http://fo.gzmigu.cn

PHP:  return [$a, $b];
来源：http://kn.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vh.hnjuh.cn

TS:   return { a, b };
来源：http://tq.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gm.gzmigu.cn

Go:   return a, b
来源：http://ec.shtwfgs.cn

Ruby: return a, b
来源：http://uh.chemitech.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://ai.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://dl.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://md.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://il.hahajie.cn

JS:   const square = x => x * x;
来源：http://tf.jianghongdianzi.cn

TS:   const square = (x: number): number => x * x;
来源：http://gs.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://je.nicolike.cn

Go:   sq := func(x int) int { return x * x }
来源：http://js.asd995.cn

Ruby: square = ->(x) { x * x }
来源：http://cb.chemitech.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://et.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://ku.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ss.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mo.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://df.colortex.cn

TS:   arr.map(String)
来源：http://ko.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dl.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qv.muxihuayi.cn

Ruby: arr.map(&:upcase)
来源：http://sc.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vj.nszjky.cn

[C08] 闭包
来源：http://cw.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yt.huanxung.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gb.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mi.colortex.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hb.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gp.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bk.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ci.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gf.shxzukj.cn

[C09] 递归
来源：http://qk.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rc.bookmarksfly.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://to.521024.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ne.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xm.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ec.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://va.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://my.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yw.huixiangedu.cn

[C10] 变量作用域
来源：http://on.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://au.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lg.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rr.huixinmuqiang.cn

TS:   同 JS
来源：http://vl.jctech888.com.cn

Java: 方法内为块级作用域
来源：http://ao.muxihuayi.cn

Go:   花括号块级作用域
来源：http://nr.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://it.huixinmuqiang.cn

C#:   块级作用域
来源：http://rh.jianghongdianzi.cn

[C11] 模块导入与导出
来源：http://cp.haigaiapp.cn

Py:   from module import func
来源：http://fp.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ab.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gw.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rz.huixiangedu.cn

Java: import java.util.List;
来源：http://yy.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ta.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://nd.yuntaijiaju.cn

C#:   using System.Text;
来源：http://hm.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://wn.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://wh.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://nm.jianghongdianzi.cn

JS:   (() => { console.log("run"); })();
来源：http://af.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://yo.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dn.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://cb.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://eq.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gn.521024.cn

[C13] 类型声明 / 类型注解
来源：http://cv.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sr.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://su.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ss.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://da.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dm.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://li.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cb.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tc.hnjuh.cn

[C14] 泛型函数
来源：http://na.huixiangedu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fx.shtwfgs.cn

PHP:  // 无泛型
来源：http://zu.szsharing.cn

JS:   // 无泛型
来源：http://yz.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fj.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ut.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gd.colortex.cn

Ruby: # 无泛型
来源：http://px.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jq.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://li.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yq.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://hi.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nk.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ao.huixinmuqiang.cn

Java: // 无解构
来源：http://dk.newstarts.cn

Go:   // 无解构
来源：http://cg.chemitech.net.cn

Ruby: a, b = pair
来源：http://mo.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://as.newstarts.cn

[C16] 函数 / 方法重载
来源：http://tp.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wr.haigaiapp.cn

PHP:  // 无重载
来源：http://lx.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qi.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://al.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ii.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://qy.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://to.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cr.huanxung.cn

================================================================================
来源：http://rf.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://ce.szsharing.cn

================================================================================
来源：http://oz.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://dl.bjjhwx.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oj.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ph.szxytkj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ou.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cf.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ys.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ru.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://be.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mw.huanxung.cn

[D02] 追加元素到末尾
来源：http://ld.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lv.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ho.bjjhwx.cn

JS:   arr.push(4);
来源：http://mx.newstarts.cn

TS:   arr.push(4);
来源：http://qa.bjjhwx.cn

Java: list.add(4);
来源：http://ot.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://ko.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://uv.lnxyls.cn

C#:   list.Add(4);
来源：http://ha.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://aa.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://yl.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ns.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vp.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://xl.jctech888.com.cn

Java: list.add(0, 0);
来源：http://yt.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jv.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iu.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://el.szxytkj.cn

[D04] 删除元素
来源：http://ux.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vd.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://st.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ee.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://wt.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://br.panjiajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wv.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vs.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yt.szxytkj.cn

[D05] 访问与修改元素
来源：http://id.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zu.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ys.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hu.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://vp.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://nm.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://ep.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lu.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dt.jianghongdianzi.cn

[D06] 数组长度
来源：http://db.nszjky.cn

Py:   len(arr)
来源：http://po.lnxyls.cn

PHP:  count($arr);
来源：http://so.colortex.cn

JS:   arr.length
来源：http://es.chemitech.net.cn

TS:   arr.length
来源：http://jy.huanxung.cn

Java: list.size();
来源：http://fb.newstarts.cn

Go:   len(arr)
来源：http://ov.9csxet.cn

Ruby: arr.length; arr.size
来源：http://ca.panjiajie.cn

C#:   list.Count;
来源：http://ck.colortex.cn

[D07] 切片 / 取子数组
来源：http://tr.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kb.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ha.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://bk.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://xj.szxytkj.cn

Java: list.subList(1, 4);
来源：http://bw.chemitech.net.cn

Go:   arr[1:4]
来源：http://mf.szxytkj.cn

Ruby: arr[1, 3]
来源：http://cx.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://aj.shxzukj.cn

[D08] 合并两个数组
来源：http://qz.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://kb.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://et.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nd.panjiajie.cn

TS:   [...a, ...b];
来源：http://ho.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iz.gzmigu.cn

Go:   append(a, b...)
来源：http://hc.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://ra.asd995.cn

C#:   a.Concat(b).ToList()
来源：http://rq.nicolike.cn

[D09] 排序（升序）
来源：http://ca.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://sp.panjiajie.cn

PHP:  sort($arr);
来源：http://zt.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qf.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bo.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://er.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qk.yuexingan06.cn

Ruby: arr.sort
来源：http://km.bookmarksfly.cn

C#:   list.Sort();
来源：http://oo.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zf.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jf.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nz.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yl.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gn.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ck.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jf.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ha.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hl.jianghongdianzi.cn

[D11] 反转数组
来源：http://wi.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vy.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://hf.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vb.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://gg.shxzukj.cn

Java: Collections.reverse(list);
来源：http://eg.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://io.szsharing.cn

Ruby: arr.reverse
来源：http://jo.bookmarksfly.cn

C#:   list.Reverse();
来源：http://gf.jctech888.com.cn

[D12] 查找元素下标
来源：http://bb.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://dw.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://om.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xs.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xe.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cs.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://lw.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://ob.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://pl.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://tl.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tb.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uq.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://sg.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://rf.newstarts.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xq.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vu.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fm.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cw.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://yr.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sk.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://om.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://ro.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://wy.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cp.bjjhwx.cn

Go:   // 手写循环
来源：http://lx.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xo.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://di.shxzukj.cn

[D15] 去重
来源：http://lm.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dx.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://cv.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://mk.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://cm.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tw.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iu.nszjky.cn

Ruby: arr.uniq
来源：http://rb.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://fv.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://kg.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oi.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qn.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qc.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://do.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wv.colortex.cn

Go:   // 手写循环累加
来源：http://rs.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dh.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://ss.yuexingan06.cn

[D17] 最大值与最小值
来源：http://hk.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://ij.haigaiapp.cn


<!-- 参考信息 -->