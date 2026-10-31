代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kf.huanxung.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pw.nszjky.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xx.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xq.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fx.yuntaijiaju.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ha.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://tf.shxzskj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://td.hahajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oo.bjjhwx.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nr.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nu.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://df.shtwfgs.cn

Go:   // 无：用配置结构体参数
来源：http://qh.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://et.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://fx.haigaiapp.cn

[C05] 返回多个值
来源：http://el.lnxyls.cn

Py:   return a, b
来源：http://wy.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://rv.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bi.szsharing.cn

TS:   return { a, b };
来源：http://wr.521024.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pm.521024.cn

Go:   return a, b
来源：http://fc.9csxet.cn

Ruby: return a, b
来源：http://xm.shxzskj.cn

C#:   return (a, b);              // ValueTuple
来源：http://wx.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://hh.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://nn.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oq.colortex.cn

JS:   const square = x => x * x;
来源：http://zw.nicolike.cn

TS:   const square = (x: number): number => x * x;
来源：http://os.panjiajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ry.panjiajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nv.yuntaijiaju.cn

Ruby: square = ->(x) { x * x }
来源：http://kd.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tk.shxzskj.cn

[C07] 把函数作为参数传入
来源：http://wf.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://km.muxihuayi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sz.panjiajie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://to.panjiajie.cn

TS:   arr.map(String)
来源：http://zk.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kf.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qf.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://xv.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://do.colortex.cn

[C08] 闭包
来源：http://pv.nszjky.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hj.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hc.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lj.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mq.shtwfgs.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fd.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fw.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ni.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uz.huanxung.cn

[C09] 递归
来源：http://kt.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://li.9csxet.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ql.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hm.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pb.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hd.haigaiapp.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bu.muxihuayi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ay.hnjuh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ie.nicolike.cn

[C10] 变量作用域
来源：http://od.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jm.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zj.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kn.shtwfgs.cn

TS:   同 JS
来源：http://ar.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://og.bjjhwx.cn

Go:   花括号块级作用域
来源：http://bv.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fv.chemitech.net.cn

C#:   块级作用域
来源：http://xi.muxihuayi.cn

[C11] 模块导入与导出
来源：http://ia.shxzukj.cn

Py:   from module import func
来源：http://qn.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fz.nicolike.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://am.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ls.muxihuayi.cn

Java: import java.util.List;
来源：http://ul.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sb.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://dn.huixinmuqiang.cn

C#:   using System.Text;
来源：http://dm.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://am.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://sb.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://dq.newstarts.cn

JS:   (() => { console.log("run"); })();
来源：http://uh.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://nz.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yf.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://gg.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://wz.jianghongdianzi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jl.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://jo.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ux.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vf.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gt.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ms.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gy.colortex.cn

Go:   func add(a, b int) int
来源：http://eu.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wj.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dq.asd995.cn

[C14] 泛型函数
来源：http://vt.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jl.szsharing.cn

PHP:  // 无泛型
来源：http://va.shtwfgs.cn

JS:   // 无泛型
来源：http://wc.nicolike.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ab.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yg.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vs.hnjuh.cn

Ruby: # 无泛型
来源：http://wk.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uj.huanxung.cn

[C15] 解构 / 展开参数
来源：http://xh.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dk.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://dn.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cr.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cj.hahajie.cn

Java: // 无解构
来源：http://us.wgjwhj.cn

Go:   // 无解构
来源：http://nh.huixiangedu.cn

Ruby: a, b = pair
来源：http://dq.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://uk.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://vr.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cj.huixinmuqiang.cn

PHP:  // 无重载
来源：http://mk.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oq.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://of.jctech888.com.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rq.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://st.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://bp.colortex.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qt.jianghongdianzi.cn

================================================================================
来源：http://rj.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://qr.colortex.cn

================================================================================
来源：http://ur.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://in.colortex.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gh.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hy.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dh.9csxet.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ch.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cs.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://xt.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://mw.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ru.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://uo.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ri.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hi.bookmarksfly.cn

JS:   arr.push(4);
来源：http://ml.yuexingan06.cn

TS:   arr.push(4);
来源：http://qo.gzmigu.cn

Java: list.add(4);
来源：http://rs.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://ee.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://px.jctech888.com.cn

C#:   list.Add(4);
来源：http://ep.newstarts.cn

[D03] 在指定位置插入元素
来源：http://kb.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://dl.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ba.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gq.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://pg.huanxung.cn

Java: list.add(0, 0);
来源：http://pf.haigaiapp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://et.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rc.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://bw.bjjhwx.cn

[D04] 删除元素
来源：http://le.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qu.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bt.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gj.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://cy.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yp.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qm.nszjky.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fg.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lv.jctech888.com.cn

[D05] 访问与修改元素
来源：http://hf.haigaiapp.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wq.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pc.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yo.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://on.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://zg.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ej.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yr.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ye.huixinmuqiang.cn

[D06] 数组长度
来源：http://xr.shxzskj.cn

Py:   len(arr)
来源：http://ah.gzmigu.cn

PHP:  count($arr);
来源：http://is.shxzskj.cn

JS:   arr.length
来源：http://mq.lnxyls.cn

TS:   arr.length
来源：http://sj.hnjuh.cn

Java: list.size();
来源：http://af.asd995.cn

Go:   len(arr)
来源：http://qm.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://sa.wgjwhj.cn

C#:   list.Count;
来源：http://al.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://ve.shxzskj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wz.yuexingan06.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kr.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://cf.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://rw.shxzukj.cn

Java: list.subList(1, 4);
来源：http://zj.lnxyls.cn

Go:   arr[1:4]
来源：http://fu.huanxung.cn

Ruby: arr[1, 3]
来源：http://qp.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://kr.bjjhwx.cn

[D08] 合并两个数组
来源：http://hf.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://na.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://kp.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vn.asd995.cn

TS:   [...a, ...b];
来源：http://an.huanxung.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mk.chemitech.net.cn

Go:   append(a, b...)
来源：http://wr.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://ht.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://cm.shtwfgs.cn

[D09] 排序（升序）
来源：http://fa.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://py.chemitech.net.cn

PHP:  sort($arr);
来源：http://uh.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lv.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ro.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yg.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uj.shxzukj.cn

Ruby: arr.sort
来源：http://fm.shxzukj.cn

C#:   list.Sort();
来源：http://px.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ox.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kq.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oc.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lg.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ij.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fk.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oh.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lz.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wk.chemitech.net.cn

[D11] 反转数组
来源：http://rl.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zt.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://lv.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ow.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://mz.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://vi.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://jq.gzmigu.cn

Ruby: arr.reverse
来源：http://xf.wgjwhj.cn

C#:   list.Reverse();
来源：http://ln.panjiajie.cn

[D12] 查找元素下标
来源：http://il.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://rk.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ha.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vi.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ov.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jp.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://gu.shtwfgs.cn

Ruby: arr.index(x)
来源：http://pm.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://uo.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://wd.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://up.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://iu.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://tr.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://kk.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bz.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rh.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kk.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eo.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://il.bjjhwx.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kk.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xy.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://pl.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://iq.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ds.nszjky.cn

Go:   // 手写循环
来源：http://yk.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lf.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ee.asd995.cn

[D15] 去重
来源：http://wl.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dw.9csxet.cn

PHP:  array_unique($arr);
来源：http://di.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://nu.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://qu.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cx.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xx.huanxung.cn

Ruby: arr.uniq
来源：http://xs.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://xa.colortex.cn

[D16] 求和与平均值
来源：http://aw.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zm.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xv.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gt.huixiangedu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iy.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://os.yuexingan06.cn

Go:   // 手写循环累加
来源：http://ko.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://re.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://lp.chemitech.net.cn

[D17] 最大值与最小值
来源：http://eu.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ia.huixinmuqiang.cn

PHP:  max($arr);  min($arr);
来源：http://nf.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xq.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://hk.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ak.colortex.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pg.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://vd.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://of.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://kf.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kq.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://ad.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bj.nicolike.cn

TS:   nested.flat();
来源：http://tb.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yg.lnxyls.cn

Go:   // 手写双层循环
来源：http://hv.jctech888.com.cn

Ruby: nested.flatten
来源：http://xh.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://de.521024.cn

[D19] 按字段分组
来源：http://dw.newstarts.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jy.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://da.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rc.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pg.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ag.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://cm.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://my.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vt.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://js.gzmigu.cn

Py:   Counter(arr)
来源：http://aq.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://hg.9csxet.cn


<!-- 参考信息 -->