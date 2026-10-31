代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vg.nszjky.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cs.panjiajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zv.gzmigu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pc.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sy.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ok.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://jz.yuntaijiaju.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ym.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fs.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qc.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bp.9csxet.cn

Java: // 无：用 Builder 模式或 record
来源：http://lh.szsharing.cn

Go:   // 无：用配置结构体参数
来源：http://ak.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://bo.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://zh.lnxyls.cn

[C05] 返回多个值
来源：http://bf.panjiajie.cn

Py:   return a, b
来源：http://xl.colortex.cn

PHP:  return [$a, $b];
来源：http://os.huanxung.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qv.lnxyls.cn

TS:   return { a, b };
来源：http://bb.newstarts.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jh.huanxung.cn

Go:   return a, b
来源：http://dg.lnxyls.cn

Ruby: return a, b
来源：http://kq.nicolike.cn

C#:   return (a, b);              // ValueTuple
来源：http://tb.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://uf.asd995.cn

Py:   square = lambda x: x * x
来源：http://yw.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nr.yuntaijiaju.cn

JS:   const square = x => x * x;
来源：http://kg.szxytkj.cn

TS:   const square = (x: number): number => x * x;
来源：http://ja.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cm.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oj.muxihuayi.cn

Ruby: square = ->(x) { x * x }
来源：http://jc.asd995.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wu.newstarts.cn

[C07] 把函数作为参数传入
来源：http://ql.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xo.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rz.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ea.panjiajie.cn

TS:   arr.map(String)
来源：http://jq.huanxung.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://or.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qw.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://au.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://sc.szsharing.cn

[C08] 闭包
来源：http://wg.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ki.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ww.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gp.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zf.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ll.wgjwhj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bb.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jn.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://st.gzmigu.cn

[C09] 递归
来源：http://tw.asd995.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hm.hnjuh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://me.haigaiapp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sa.gzmigu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uj.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hf.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dz.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oa.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eb.hnjuh.cn

[C10] 变量作用域
来源：http://mf.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tc.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rq.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fu.asd995.cn

TS:   同 JS
来源：http://cr.521024.cn

Java: 方法内为块级作用域
来源：http://ep.bjjhwx.cn

Go:   花括号块级作用域
来源：http://qn.huanxung.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xr.asd995.cn

C#:   块级作用域
来源：http://va.521024.cn

[C11] 模块导入与导出
来源：http://zi.jctech888.com.cn

Py:   from module import func
来源：http://mu.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ie.haigaiapp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pq.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vu.szxytkj.cn

Java: import java.util.List;
来源：http://qz.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cc.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://hd.szsharing.cn

C#:   using System.Text;
来源：http://vi.huixiangedu.cn

[C12] 立即执行函数 IIFE
来源：http://iw.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://xb.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://qx.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://nx.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://hw.lnxyls.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tt.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://yq.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://gp.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bi.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://gp.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pf.gzmigu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tu.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bq.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jn.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jz.nicolike.cn

Go:   func add(a, b int) int
来源：http://kj.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qj.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://yg.huanxung.cn

[C14] 泛型函数
来源：http://la.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ax.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://js.shxzskj.cn

JS:   // 无泛型
来源：http://ce.9csxet.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rm.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dt.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wm.bjjhwx.cn

Ruby: # 无泛型
来源：http://qd.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ah.bjjhwx.cn

[C15] 解构 / 展开参数
来源：http://sl.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xq.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://ue.chemitech.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pd.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ep.wgjwhj.cn

Java: // 无解构
来源：http://tv.bookmarksfly.cn

Go:   // 无解构
来源：http://hn.shxzskj.cn

Ruby: a, b = pair
来源：http://nf.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://qn.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://qs.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pg.shxzskj.cn

PHP:  // 无重载
来源：http://de.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://dx.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://cz.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ld.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://bq.panjiajie.cn

Ruby: # 无重载：靠动态参数
来源：http://cb.nicolike.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xm.haigaiapp.cn

================================================================================
来源：http://ha.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://jw.szsharing.cn

================================================================================
来源：http://il.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://nt.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ap.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tt.shxzukj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ws.newstarts.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gp.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uf.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://mu.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://aj.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kw.szsharing.cn

[D02] 追加元素到末尾
来源：http://tp.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xm.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fl.shtwfgs.cn

JS:   arr.push(4);
来源：http://su.shtwfgs.cn

TS:   arr.push(4);
来源：http://gx.gzmigu.cn

Java: list.add(4);
来源：http://xe.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://nu.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://eb.shxzukj.cn

C#:   list.Add(4);
来源：http://rg.szsharing.cn

[D03] 在指定位置插入元素
来源：http://xi.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://zn.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hx.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bm.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://yn.gzmigu.cn

Java: list.add(0, 0);
来源：http://cc.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://te.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ht.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://mp.yuntaijiaju.cn

[D04] 删除元素
来源：http://av.chemitech.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ch.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iy.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tv.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://bz.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bn.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://we.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sy.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vg.shtwfgs.cn

[D05] 访问与修改元素
来源：http://kj.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vt.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://he.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ud.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://jw.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://ll.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://fj.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ma.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vv.shtwfgs.cn

[D06] 数组长度
来源：http://cq.9csxet.cn

Py:   len(arr)
来源：http://yl.9csxet.cn

PHP:  count($arr);
来源：http://mn.shtwfgs.cn

JS:   arr.length
来源：http://nc.huixinmuqiang.cn

TS:   arr.length
来源：http://gz.gzmigu.cn

Java: list.size();
来源：http://vt.shtwfgs.cn

Go:   len(arr)
来源：http://ed.521024.cn

Ruby: arr.length; arr.size
来源：http://xc.yuexingan06.cn

C#:   list.Count;
来源：http://lw.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://so.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vv.szsharing.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ho.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://rv.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://fj.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://ft.szsharing.cn

Go:   arr[1:4]
来源：http://uw.lnxyls.cn

Ruby: arr[1, 3]
来源：http://ne.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://bs.szsharing.cn

[D08] 合并两个数组
来源：http://qc.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://br.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://lm.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oc.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://di.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://op.szsharing.cn

Go:   append(a, b...)
来源：http://cp.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://kn.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://km.yuexingan06.cn

[D09] 排序（升序）
来源：http://zi.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://uy.huixiangedu.cn

PHP:  sort($arr);
来源：http://qt.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pz.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bi.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jk.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qq.szsharing.cn

Ruby: arr.sort
来源：http://ym.bookmarksfly.cn

C#:   list.Sort();
来源：http://ak.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ac.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ad.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ej.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uv.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rr.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mi.panjiajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pe.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xw.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zt.szsharing.cn

[D11] 反转数组
来源：http://pz.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vj.huanxung.cn

PHP:  array_reverse($arr);
来源：http://ck.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rq.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://sp.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://zd.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://td.shtwfgs.cn

Ruby: arr.reverse
来源：http://oz.nszjky.cn

C#:   list.Reverse();
来源：http://zp.haigaiapp.cn

[D12] 查找元素下标
来源：http://lg.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://kc.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gb.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ei.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qo.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vp.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://be.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://bs.newstarts.cn

C#:   list.IndexOf(x);
来源：http://xv.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://do.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uo.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://av.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://yk.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://qt.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://be.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qf.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wp.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gz.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://ac.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jz.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ub.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://yu.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://hh.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ps.nicolike.cn

Go:   // 手写循环
来源：http://gh.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hi.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ia.9csxet.cn

[D15] 去重
来源：http://tk.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://in.huanxung.cn

PHP:  array_unique($arr);
来源：http://tt.asd995.cn

JS:   [...new Set(arr)]
来源：http://hz.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://sd.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rr.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://th.newstarts.cn

Ruby: arr.uniq
来源：http://ge.asd995.cn

C#:   list.Distinct().ToList()
来源：http://lm.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://qi.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ox.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hf.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zh.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ax.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oj.colortex.cn

Go:   // 手写循环累加
来源：http://wk.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xp.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://tw.asd995.cn

[D17] 最大值与最小值
来源：http://uh.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://ib.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://ar.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fl.panjiajie.cn

TS:   Math.max(...arr);
来源：http://gk.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qi.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hc.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://qn.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://uh.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://fm.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rg.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://ql.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gc.nszjky.cn

TS:   nested.flat();
来源：http://rs.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zx.bjjhwx.cn

Go:   // 手写双层循环
来源：http://lo.huixiangedu.cn

Ruby: nested.flatten
来源：http://wj.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yt.shxzskj.cn

[D19] 按字段分组
来源：http://wx.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wj.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ye.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ak.yuntaijiaju.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qd.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pf.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://bw.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zt.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ea.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://fm.panjiajie.cn

Py:   Counter(arr)
来源：http://pk.haigaiapp.cn

PHP:  array_count_values($arr);
来源：http://ub.shtwfgs.cn


<!-- 参考信息 -->