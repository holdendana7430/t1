代发 wailian999

[C02] 默认参数
来源：http://tb.colortex.cn

Py:   def greet(name="World"): return name
来源：http://yz.szxytkj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xs.lnxyls.cn

JS:   function greet(name = "World") { return name; }
来源：http://ru.wgjwhj.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hf.panjiajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://mu.bjjhwx.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pt.haigaiapp.cn

Ruby: def greet(name = "World") = name
来源：http://ew.lnxyls.cn

C#:   string Greet(string name = "World") => name;
来源：http://op.jctech888.com.cn

[C03] 可变参数
来源：http://rm.hahajie.cn

Py:   def total(*args): return sum(args)
来源：http://jj.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jo.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ja.newstarts.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ks.huixinmuqiang.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ip.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hi.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bu.asd995.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zq.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://up.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pd.asd995.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xg.huanxung.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ct.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ll.shtwfgs.cn

Java: // 无：用 Builder 模式或 record
来源：http://jy.hnjuh.cn

Go:   // 无：用配置结构体参数
来源：http://mr.yuntaijiaju.cn

Ruby: f(a: 1, b: 2)
来源：http://mf.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://xb.huixinmuqiang.cn

[C05] 返回多个值
来源：http://cu.colortex.cn

Py:   return a, b
来源：http://qf.asd995.cn

PHP:  return [$a, $b];
来源：http://fm.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://le.hnjuh.cn

TS:   return { a, b };
来源：http://ep.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ho.jctech888.com.cn

Go:   return a, b
来源：http://mv.shxzukj.cn

Ruby: return a, b
来源：http://gl.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://tz.colortex.cn

[C06] 匿名函数 / lambda
来源：http://cy.muxihuayi.cn

Py:   square = lambda x: x * x
来源：http://qi.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jl.haigaiapp.cn

JS:   const square = x => x * x;
来源：http://yb.colortex.cn

TS:   const square = (x: number): number => x * x;
来源：http://np.shxzskj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kf.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fb.lnxyls.cn

Ruby: square = ->(x) { x * x }
来源：http://je.lnxyls.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tq.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://qr.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zh.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aq.wgjwhj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vp.nicolike.cn

TS:   arr.map(String)
来源：http://lt.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gk.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ds.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://oz.huanxung.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tq.nszjky.cn

[C08] 闭包
来源：http://la.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ck.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vn.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hd.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sx.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jw.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qp.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zj.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yj.yuntaijiaju.cn

[C09] 递归
来源：http://uh.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sm.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sz.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://aj.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rd.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bz.huixinmuqiang.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rk.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gb.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eq.newstarts.cn

[C10] 变量作用域
来源：http://at.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ys.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rz.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kq.shxzukj.cn

TS:   同 JS
来源：http://rh.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://cb.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://gm.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fe.huixinmuqiang.cn

C#:   块级作用域
来源：http://cn.bookmarksfly.cn

[C11] 模块导入与导出
来源：http://uf.jctech888.com.cn

Py:   from module import func
来源：http://ry.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ae.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bc.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ej.newstarts.cn

Java: import java.util.List;
来源：http://qj.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lz.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://xi.panjiajie.cn

C#:   using System.Text;
来源：http://yq.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://ml.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://nq.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://hd.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://eo.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://zc.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ud.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://it.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://si.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://hb.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lw.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wo.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yz.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ef.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mb.asd995.cn

Go:   func add(a, b int) int
来源：http://nq.shxzskj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wx.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yt.colortex.cn

[C14] 泛型函数
来源：http://du.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ii.nszjky.cn

PHP:  // 无泛型
来源：http://fh.nszjky.cn

JS:   // 无泛型
来源：http://en.lnxyls.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pf.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mj.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fu.9csxet.cn

Ruby: # 无泛型
来源：http://co.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://na.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://qf.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xb.hahajie.cn

PHP:  [$a, $b] = $pair;
来源：http://kh.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qb.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dw.huixinmuqiang.cn

Java: // 无解构
来源：http://kd.huanxung.cn

Go:   // 无解构
来源：http://tt.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://oe.521024.cn

C#:   var (a, b) = pair;
来源：http://zb.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://gh.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iq.gzmigu.cn

PHP:  // 无重载
来源：http://uh.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tp.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://mh.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://es.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://rg.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://oy.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lv.hnjuh.cn

================================================================================
来源：http://wp.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://ww.panjiajie.cn

================================================================================
来源：http://av.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://oq.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ak.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sj.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vc.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ab.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gz.haigaiapp.cn

Go:   arr := []int{1, 2, 3}
来源：http://es.szsharing.cn

Ruby: arr = [1, 2, 3]
来源：http://ac.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hb.colortex.cn

[D02] 追加元素到末尾
来源：http://iu.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mr.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sj.521024.cn

JS:   arr.push(4);
来源：http://tl.nszjky.cn

TS:   arr.push(4);
来源：http://wa.lnxyls.cn

Java: list.add(4);
来源：http://it.asd995.cn

Go:   arr = append(arr, 4)
来源：http://ko.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://pn.szsharing.cn

C#:   list.Add(4);
来源：http://iw.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://ak.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://oh.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://je.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cc.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://te.szsharing.cn

Java: list.add(0, 0);
来源：http://jf.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://eo.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ly.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://qp.yuntaijiaju.cn

[D04] 删除元素
来源：http://of.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qr.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tq.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://im.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://xk.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ry.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ua.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dt.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yz.muxihuayi.cn

[D05] 访问与修改元素
来源：http://kw.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hh.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://te.haigaiapp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tz.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://qw.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://ln.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://mj.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://un.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cc.9csxet.cn

[D06] 数组长度
来源：http://mk.hnjuh.cn

Py:   len(arr)
来源：http://er.nszjky.cn

PHP:  count($arr);
来源：http://ux.jctech888.com.cn

JS:   arr.length
来源：http://oc.jianghongdianzi.cn

TS:   arr.length
来源：http://cs.shtwfgs.cn

Java: list.size();
来源：http://zd.yuexingan06.cn

Go:   len(arr)
来源：http://sp.nszjky.cn

Ruby: arr.length; arr.size
来源：http://kk.hahajie.cn

C#:   list.Count;
来源：http://tp.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://nz.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kd.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jg.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://hj.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://fi.szxytkj.cn

Java: list.subList(1, 4);
来源：http://tk.huixiangedu.cn

Go:   arr[1:4]
来源：http://wd.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://vs.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://ex.hnjuh.cn

[D08] 合并两个数组
来源：http://pr.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://io.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://kz.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vv.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://eq.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://su.hnjuh.cn

Go:   append(a, b...)
来源：http://sj.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://ku.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://ae.nszjky.cn

[D09] 排序（升序）
来源：http://cw.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://xy.lnxyls.cn

PHP:  sort($arr);
来源：http://of.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gw.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xk.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bu.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://we.jctech888.com.cn

Ruby: arr.sort
来源：http://ru.yuexingan06.cn

C#:   list.Sort();
来源：http://tp.lnxyls.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nl.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qv.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xb.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ep.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dj.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lu.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nl.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://om.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fe.bjjhwx.cn

[D11] 反转数组
来源：http://oa.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://du.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://xb.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fv.shxzskj.cn

TS:   [...arr].reverse();
来源：http://ln.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://rn.521024.cn

Go:   slices.Reverse(arr)
来源：http://ww.yuexingan06.cn

Ruby: arr.reverse
来源：http://vn.wgjwhj.cn

C#:   list.Reverse();
来源：http://wn.szxytkj.cn

[D12] 查找元素下标
来源：http://uk.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://nb.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cs.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dk.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jj.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ff.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://lg.521024.cn

Ruby: arr.index(x)
来源：http://hp.asd995.cn

C#:   list.IndexOf(x);
来源：http://gs.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://xk.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ei.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vu.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://yz.panjiajie.cn

TS:   arr.filter(x => x > 3)
来源：http://nf.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oe.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ws.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kb.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fa.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://xc.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hn.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wa.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://ct.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://qu.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zv.shxzukj.cn

Go:   // 手写循环
来源：http://yr.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jt.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rk.asd995.cn

[D15] 去重
来源：http://um.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tq.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://fz.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://ih.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://kr.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tg.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qy.huixiangedu.cn

Ruby: arr.uniq
来源：http://md.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://xp.muxihuayi.cn

[D16] 求和与平均值
来源：http://xe.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vn.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jz.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vm.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ka.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kz.szxytkj.cn

Go:   // 手写循环累加
来源：http://dg.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lh.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://yv.nicolike.cn

[D17] 最大值与最小值
来源：http://rb.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://sp.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ho.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eo.nszjky.cn

TS:   Math.max(...arr);
来源：http://gg.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gc.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oa.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://uy.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://db.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://gn.muxihuayi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dg.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://cd.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lg.haigaiapp.cn

TS:   nested.flat();
来源：http://zx.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wf.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://we.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://sb.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jv.huanxung.cn


<!-- 参考信息 -->