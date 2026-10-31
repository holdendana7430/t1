代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xh.asd995.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://td.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jt.shtwfgs.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xi.muxihuayi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pv.shxzskj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://da.nicolike.cn

[C04] 命名参数 / 关键字参数
来源：http://uj.muxihuayi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bc.shtwfgs.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dk.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ow.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ko.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://pj.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://wu.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://mf.shxzskj.cn

C#:   f(a: 1, b: 2)
来源：http://bc.hnjuh.cn

[C05] 返回多个值
来源：http://xe.hnjuh.cn

Py:   return a, b
来源：http://va.gzmigu.cn

PHP:  return [$a, $b];
来源：http://dw.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wn.panjiajie.cn

TS:   return { a, b };
来源：http://ei.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ho.huanxung.cn

Go:   return a, b
来源：http://cc.muxihuayi.cn

Ruby: return a, b
来源：http://dp.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://gz.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://tl.szsharing.cn

Py:   square = lambda x: x * x
来源：http://ar.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ji.colortex.cn

JS:   const square = x => x * x;
来源：http://mf.yuexingan06.cn

TS:   const square = (x: number): number => x * x;
来源：http://po.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fl.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://eu.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://hg.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://pv.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://cx.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lz.jctech888.com.cn

PHP:  array_map("strtoupper", $arr);
来源：http://un.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pt.szsharing.cn

TS:   arr.map(String)
来源：http://os.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iy.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://di.chemitech.net.cn

Ruby: arr.map(&:upcase)
来源：http://gk.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ut.yuntaijiaju.cn

[C08] 闭包
来源：http://xu.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ph.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tt.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sr.szsharing.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kg.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qp.521024.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qh.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dp.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mb.shxzukj.cn

[C09] 递归
来源：http://ra.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fy.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://li.shxzskj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gj.lnxyls.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://do.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xd.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://un.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://no.haigaiapp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kq.szxytkj.cn

[C10] 变量作用域
来源：http://uv.haigaiapp.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yy.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wb.jianghongdianzi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gv.newstarts.cn

TS:   同 JS
来源：http://fv.colortex.cn

Java: 方法内为块级作用域
来源：http://eb.gzmigu.cn

Go:   花括号块级作用域
来源：http://jr.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rb.jctech888.com.cn

C#:   块级作用域
来源：http://ah.szsharing.cn

[C11] 模块导入与导出
来源：http://ez.gzmigu.cn

Py:   from module import func
来源：http://cx.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ag.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://yp.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hc.yuexingan06.cn

Java: import java.util.List;
来源：http://it.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://in.jianghongdianzi.cn

Ruby: require "json"; require_relative "./util"
来源：http://ub.shtwfgs.cn

C#:   using System.Text;
来源：http://ru.hahajie.cn

[C12] 立即执行函数 IIFE
来源：http://iy.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://bh.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://gh.wgjwhj.cn

JS:   (() => { console.log("run"); })();
来源：http://dt.shtwfgs.cn

TS:   (() => { console.log("run"); })();
来源：http://vj.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lq.shtwfgs.cn

Go:   func() { fmt.Println("run") }()
来源：http://fg.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://lb.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wk.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://va.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mv.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://oi.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cr.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zb.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zy.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://dp.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bg.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hs.asd995.cn

[C14] 泛型函数
来源：http://ih.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zp.szxytkj.cn

PHP:  // 无泛型
来源：http://ki.asd995.cn

JS:   // 无泛型
来源：http://lf.shxzukj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bc.gzmigu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://to.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qo.jctech888.com.cn

Ruby: # 无泛型
来源：http://zh.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kt.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://su.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://um.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://cy.colortex.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xx.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pa.lnxyls.cn

Java: // 无解构
来源：http://td.shtwfgs.cn

Go:   // 无解构
来源：http://gr.gzmigu.cn

Ruby: a, b = pair
来源：http://re.szsharing.cn

C#:   var (a, b) = pair;
来源：http://zc.newstarts.cn

[C16] 函数 / 方法重载
来源：http://yb.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qc.521024.cn

PHP:  // 无重载
来源：http://ps.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mr.huixiangedu.cn

TS:   // 用联合类型或重载签名声明
来源：http://va.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jt.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://cj.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://ls.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xe.huixinmuqiang.cn

================================================================================
来源：http://qd.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://cb.yuntaijiaju.cn

================================================================================
来源：http://up.huixinmuqiang.cn

[D01] 创建数组 / 列表
来源：http://eq.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pt.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eo.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://st.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dh.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fu.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://cg.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://nr.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ja.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://ud.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ta.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ej.bookmarksfly.cn

JS:   arr.push(4);
来源：http://jr.gzmigu.cn

TS:   arr.push(4);
来源：http://th.521024.cn

Java: list.add(4);
来源：http://vl.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://ie.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://ah.bjjhwx.cn

C#:   list.Add(4);
来源：http://yv.hahajie.cn

[D03] 在指定位置插入元素
来源：http://yi.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://dm.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bu.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ws.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://xv.hahajie.cn

Java: list.add(0, 0);
来源：http://ik.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://va.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kc.hnjuh.cn

C#:   list.Insert(0, 0);
来源：http://ok.szxytkj.cn

[D04] 删除元素
来源：http://zy.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sk.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yp.yuexingan06.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ro.521024.cn

TS:   arr.splice(0, 1);
来源：http://mc.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hh.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cx.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cw.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mo.bjjhwx.cn

[D05] 访问与修改元素
来源：http://bj.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kv.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yg.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ye.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://aa.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://mh.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://ci.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ag.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vc.wgjwhj.cn

[D06] 数组长度
来源：http://pt.muxihuayi.cn

Py:   len(arr)
来源：http://is.shxzukj.cn

PHP:  count($arr);
来源：http://xr.szsharing.cn

JS:   arr.length
来源：http://kf.hnjuh.cn

TS:   arr.length
来源：http://js.wgjwhj.cn

Java: list.size();
来源：http://xj.yuntaijiaju.cn

Go:   len(arr)
来源：http://rf.newstarts.cn

Ruby: arr.length; arr.size
来源：http://lb.szsharing.cn

C#:   list.Count;
来源：http://sv.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://ue.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://go.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gk.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://ga.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://yl.nszjky.cn

Java: list.subList(1, 4);
来源：http://oc.asd995.cn

Go:   arr[1:4]
来源：http://vc.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://ou.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://ra.huixiangedu.cn

[D08] 合并两个数组
来源：http://ww.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://bn.asd995.cn

PHP:  array_merge($a, $b);
来源：http://lm.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yc.bookmarksfly.cn

TS:   [...a, ...b];
来源：http://lq.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ir.asd995.cn

Go:   append(a, b...)
来源：http://ta.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://gz.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://rl.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://jd.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://lv.bookmarksfly.cn

PHP:  sort($arr);
来源：http://dx.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kv.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tw.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gu.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yw.panjiajie.cn

Ruby: arr.sort
来源：http://lp.hnjuh.cn

C#:   list.Sort();
来源：http://xi.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cu.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fq.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qs.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ev.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bz.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lq.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ia.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gc.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ov.hnjuh.cn

[D11] 反转数组
来源：http://xm.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oz.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://on.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xj.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://et.9csxet.cn

Java: Collections.reverse(list);
来源：http://bt.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://gi.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://ir.shxzukj.cn

C#:   list.Reverse();
来源：http://bg.shtwfgs.cn

[D12] 查找元素下标
来源：http://rd.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://ye.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ck.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gx.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sw.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tw.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://pp.colortex.cn

Ruby: arr.index(x)
来源：http://os.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://sw.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://kg.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zg.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vv.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://rm.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://yk.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://em.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pa.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pa.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yz.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://gz.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sy.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gs.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://js.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://oj.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sx.huanxung.cn

Go:   // 手写循环
来源：http://nk.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yt.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fn.huixinmuqiang.cn

[D15] 去重
来源：http://oq.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tu.gzmigu.cn

PHP:  array_unique($arr);
来源：http://fm.colortex.cn

JS:   [...new Set(arr)]
来源：http://zf.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://hi.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://do.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bw.panjiajie.cn

Ruby: arr.uniq
来源：http://ve.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://uh.shtwfgs.cn

[D16] 求和与平均值
来源：http://py.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vd.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zm.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kk.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vl.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://db.muxihuayi.cn

Go:   // 手写循环累加
来源：http://sw.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nh.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://nv.szxytkj.cn

[D17] 最大值与最小值
来源：http://zh.asd995.cn

Py:   max(arr);  min(arr)
来源：http://fx.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://zz.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qq.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://sx.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ux.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gh.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://zm.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://dq.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://og.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sg.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://ru.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.panjiajie.cn

TS:   nested.flat();
来源：http://vc.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mz.asd995.cn

Go:   // 手写双层循环
来源：http://yb.jctech888.com.cn

Ruby: nested.flatten
来源：http://gk.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fp.panjiajie.cn

[D19] 按字段分组
来源：http://dd.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vg.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lg.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zx.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ml.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zq.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://zy.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nn.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://se.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://zc.wgjwhj.cn

Py:   Counter(arr)
来源：http://tu.asd995.cn

PHP:  array_count_values($arr);
来源：http://ik.jctech888.com.cn


<!-- 参考信息 -->