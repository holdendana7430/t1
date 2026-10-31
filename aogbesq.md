代发 wailian999

[C02] 默认参数
来源：http://lc.shxzskj.cn

Py:   def greet(name="World"): return name
来源：http://rb.shxzukj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://of.nicolike.cn

JS:   function greet(name = "World") { return name; }
来源：http://yu.shtwfgs.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wj.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xw.szxytkj.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sr.521024.cn

Ruby: def greet(name = "World") = name
来源：http://no.9csxet.cn

C#:   string Greet(string name = "World") => name;
来源：http://nw.panjiajie.cn

[C03] 可变参数
来源：http://ku.shxzskj.cn

Py:   def total(*args): return sum(args)
来源：http://oh.nicolike.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jo.haigaiapp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xm.szxytkj.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qn.shxzskj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://es.panjiajie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kg.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hv.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qz.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://ex.panjiajie.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fa.haigaiapp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ev.nicolike.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wu.huanxung.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fu.huixinmuqiang.cn

Java: // 无：用 Builder 模式或 record
来源：http://vq.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://px.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://zx.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://ym.asd995.cn

[C05] 返回多个值
来源：http://pn.lnxyls.cn

Py:   return a, b
来源：http://ue.haigaiapp.cn

PHP:  return [$a, $b];
来源：http://xb.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ii.jianghongdianzi.cn

TS:   return { a, b };
来源：http://im.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tf.szsharing.cn

Go:   return a, b
来源：http://bd.shxzukj.cn

Ruby: return a, b
来源：http://iv.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://gn.wgjwhj.cn

[C06] 匿名函数 / lambda
来源：http://vi.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://hx.lnxyls.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ll.nicolike.cn

JS:   const square = x => x * x;
来源：http://qx.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://tt.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xo.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fm.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://io.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qr.colortex.cn

[C07] 把函数作为参数传入
来源：http://ub.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kp.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ho.asd995.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lz.wgjwhj.cn

TS:   arr.map(String)
来源：http://vj.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pg.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fk.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://cx.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yx.shxzskj.cn

[C08] 闭包
来源：http://lx.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lg.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jq.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yb.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ni.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dq.yuexingan06.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sk.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pe.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://me.yuntaijiaju.cn

[C09] 递归
来源：http://sj.bjjhwx.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vu.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gg.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fm.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hb.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nz.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dh.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ia.szsharing.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uz.shtwfgs.cn

[C10] 变量作用域
来源：http://vw.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fx.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tg.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tt.hnjuh.cn

TS:   同 JS
来源：http://ko.9csxet.cn

Java: 方法内为块级作用域
来源：http://qf.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://nz.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kr.lnxyls.cn

C#:   块级作用域
来源：http://eg.hahajie.cn

[C11] 模块导入与导出
来源：http://ks.shxzukj.cn

Py:   from module import func
来源：http://fn.nicolike.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gk.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kx.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ip.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ux.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pa.521024.cn

Ruby: require "json"; require_relative "./util"
来源：http://nm.bjjhwx.cn

C#:   using System.Text;
来源：http://jk.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ry.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://mf.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://gc.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://da.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://nd.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://st.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://rw.panjiajie.cn

Ruby: -> { puts "run" }.call
来源：http://zz.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ss.521024.cn

[C13] 类型声明 / 类型注解
来源：http://xu.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lc.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jo.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hg.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gu.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ye.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://yb.bjjhwx.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yo.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cz.jctech888.com.cn

[C14] 泛型函数
来源：http://sa.yuntaijiaju.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ld.shxzskj.cn

PHP:  // 无泛型
来源：http://ue.shxzukj.cn

JS:   // 无泛型
来源：http://ag.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jc.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vh.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aq.haigaiapp.cn

Ruby: # 无泛型
来源：http://dw.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ws.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://wq.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dm.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://vc.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xb.shxzukj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wp.colortex.cn

Java: // 无解构
来源：http://mr.szsharing.cn

Go:   // 无解构
来源：http://up.nszjky.cn

Ruby: a, b = pair
来源：http://qk.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://gk.colortex.cn

[C16] 函数 / 方法重载
来源：http://cx.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ce.panjiajie.cn

PHP:  // 无重载
来源：http://ik.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eu.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://vo.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ta.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://mv.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://uc.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ck.szsharing.cn

================================================================================
来源：http://fn.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://ay.hahajie.cn

================================================================================
来源：http://yj.wgjwhj.cn

[D01] 创建数组 / 列表
来源：http://gn.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lf.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ii.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sf.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gv.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jc.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://nz.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://vr.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bd.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://ak.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sy.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ln.hahajie.cn

JS:   arr.push(4);
来源：http://go.nicolike.cn

TS:   arr.push(4);
来源：http://dy.wgjwhj.cn

Java: list.add(4);
来源：http://nd.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://tk.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://wl.hnjuh.cn

C#:   list.Add(4);
来源：http://fk.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://gl.bjjhwx.cn

Py:   arr.insert(0, 0)
来源：http://er.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ol.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pn.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://bg.lnxyls.cn

Java: list.add(0, 0);
来源：http://li.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ac.chemitech.net.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wq.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://ra.jianghongdianzi.cn

[D04] 删除元素
来源：http://wb.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xx.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wd.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hs.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://py.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xx.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://no.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://on.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://li.9csxet.cn

[D05] 访问与修改元素
来源：http://zj.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cr.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hm.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kr.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ks.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://rk.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://xe.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gn.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gw.jctech888.com.cn

[D06] 数组长度
来源：http://dw.huixinmuqiang.cn

Py:   len(arr)
来源：http://qf.shxzskj.cn

PHP:  count($arr);
来源：http://mc.nszjky.cn

JS:   arr.length
来源：http://fw.yuexingan06.cn

TS:   arr.length
来源：http://bi.szxytkj.cn

Java: list.size();
来源：http://cl.jianghongdianzi.cn

Go:   len(arr)
来源：http://mr.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://ym.nicolike.cn

C#:   list.Count;
来源：http://am.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://vu.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oi.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mi.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://eg.muxihuayi.cn

TS:   arr.slice(1, 4);
来源：http://rb.gzmigu.cn

Java: list.subList(1, 4);
来源：http://fv.wgjwhj.cn

Go:   arr[1:4]
来源：http://tk.hnjuh.cn

Ruby: arr[1, 3]
来源：http://kt.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://ak.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://bq.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://vp.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://uk.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sc.muxihuayi.cn

TS:   [...a, ...b];
来源：http://wr.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ec.szxytkj.cn

Go:   append(a, b...)
来源：http://da.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://fi.521024.cn

C#:   a.Concat(b).ToList()
来源：http://ow.colortex.cn

[D09] 排序（升序）
来源：http://uw.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://gh.szxytkj.cn

PHP:  sort($arr);
来源：http://sn.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kj.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ko.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://td.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uk.huixiangedu.cn

Ruby: arr.sort
来源：http://aq.hahajie.cn

C#:   list.Sort();
来源：http://et.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mc.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lw.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uq.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ry.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xd.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jz.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yy.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://il.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kx.chemitech.net.cn

[D11] 反转数组
来源：http://um.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yh.nszjky.cn

PHP:  array_reverse($arr);
来源：http://qs.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://by.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://di.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://ck.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://aa.wgjwhj.cn

Ruby: arr.reverse
来源：http://jh.wgjwhj.cn

C#:   list.Reverse();
来源：http://ck.shxzskj.cn

[D12] 查找元素下标
来源：http://dp.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://lq.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://br.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bh.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hg.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xp.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://id.gzmigu.cn

Ruby: arr.index(x)
来源：http://pb.newstarts.cn

C#:   list.IndexOf(x);
来源：http://lk.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://ih.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gp.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kg.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://hn.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://hy.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zr.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yz.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ir.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ih.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://ds.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eb.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cv.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://by.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://xn.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gb.yuexingan06.cn

Go:   // 手写循环
来源：http://gs.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sx.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jy.shxzskj.cn

[D15] 去重
来源：http://jm.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ks.nicolike.cn

PHP:  array_unique($arr);
来源：http://jo.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://uu.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://ep.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ld.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zd.szsharing.cn

Ruby: arr.uniq
来源：http://kk.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://cm.huanxung.cn

[D16] 求和与平均值
来源：http://jn.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ch.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jm.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ck.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bp.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://me.521024.cn

Go:   // 手写循环累加
来源：http://xw.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kb.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://kj.521024.cn

[D17] 最大值与最小值
来源：http://yj.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://gn.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://ax.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ez.nszjky.cn

TS:   Math.max(...arr);
来源：http://fm.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zh.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sc.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://lw.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://gu.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://rh.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nb.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://sf.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fe.huanxung.cn

TS:   nested.flat();
来源：http://ac.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fl.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://jx.shtwfgs.cn

Ruby: nested.flatten
来源：http://po.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kb.hahajie.cn


<!-- 参考信息 -->