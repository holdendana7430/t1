代发 wailian999

[C02] 默认参数
来源：http://vu.chemitech.net.cn

Py:   def greet(name="World"): return name
来源：http://nu.newstarts.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zz.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://ur.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tz.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pm.yuexingan06.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zu.9csxet.cn

Ruby: def greet(name = "World") = name
来源：http://ww.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://bx.hnjuh.cn

[C03] 可变参数
来源：http://dd.nszjky.cn

Py:   def total(*args): return sum(args)
来源：http://sr.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hm.shxzskj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tr.9csxet.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pd.yuexingan06.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iq.521024.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://va.panjiajie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zx.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ty.haigaiapp.cn

[C04] 命名参数 / 关键字参数
来源：http://nx.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://os.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ql.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://je.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zo.hahajie.cn

Java: // 无：用 Builder 模式或 record
来源：http://lg.huixinmuqiang.cn

Go:   // 无：用配置结构体参数
来源：http://lf.huixinmuqiang.cn

Ruby: f(a: 1, b: 2)
来源：http://dv.huixinmuqiang.cn

C#:   f(a: 1, b: 2)
来源：http://xo.muxihuayi.cn

[C05] 返回多个值
来源：http://bd.asd995.cn

Py:   return a, b
来源：http://kj.bjjhwx.cn

PHP:  return [$a, $b];
来源：http://je.szsharing.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aa.huixinmuqiang.cn

TS:   return { a, b };
来源：http://jl.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tt.jctech888.com.cn

Go:   return a, b
来源：http://xr.shxzukj.cn

Ruby: return a, b
来源：http://oz.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://oq.nicolike.cn

[C06] 匿名函数 / lambda
来源：http://rx.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://st.hnjuh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ix.szxytkj.cn

JS:   const square = x => x * x;
来源：http://mf.hnjuh.cn

TS:   const square = (x: number): number => x * x;
来源：http://ck.colortex.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sz.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mj.521024.cn

Ruby: square = ->(x) { x * x }
来源：http://qk.muxihuayi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wy.gzmigu.cn

[C07] 把函数作为参数传入
来源：http://ek.huixiangedu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yt.bookmarksfly.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ch.9csxet.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kf.wgjwhj.cn

TS:   arr.map(String)
来源：http://hd.yuexingan06.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vt.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ou.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://qn.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jc.yuexingan06.cn

[C08] 闭包
来源：http://pg.9csxet.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dn.jianghongdianzi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rm.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hb.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jq.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ns.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jt.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zx.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pf.521024.cn

[C09] 递归
来源：http://np.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sw.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xo.lnxyls.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mf.panjiajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wp.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gz.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ab.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qx.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ar.chemitech.net.cn

[C10] 变量作用域
来源：http://pw.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cx.bjjhwx.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://se.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fd.shtwfgs.cn

TS:   同 JS
来源：http://dw.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://ij.gzmigu.cn

Go:   花括号块级作用域
来源：http://jp.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qu.szxytkj.cn

C#:   块级作用域
来源：http://rs.521024.cn

[C11] 模块导入与导出
来源：http://iw.shxzukj.cn

Py:   from module import func
来源：http://nh.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wf.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rd.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xc.chemitech.net.cn

Java: import java.util.List;
来源：http://uc.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pd.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://wv.panjiajie.cn

C#:   using System.Text;
来源：http://ii.bjjhwx.cn

[C12] 立即执行函数 IIFE
来源：http://wd.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://so.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://gw.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://da.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://di.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nf.yuexingan06.cn

Go:   func() { fmt.Println("run") }()
来源：http://lh.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://eo.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lz.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ls.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zs.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hv.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qy.lnxyls.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vc.wgjwhj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vo.gzmigu.cn

Go:   func add(a, b int) int
来源：http://wv.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ix.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jw.hnjuh.cn

[C14] 泛型函数
来源：http://nw.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rk.bookmarksfly.cn

PHP:  // 无泛型
来源：http://dp.colortex.cn

JS:   // 无泛型
来源：http://qk.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cb.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dg.nicolike.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://te.shxzskj.cn

Ruby: # 无泛型
来源：http://em.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ia.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://zb.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nf.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://ut.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pl.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sq.huanxung.cn

Java: // 无解构
来源：http://qo.shxzskj.cn

Go:   // 无解构
来源：http://tl.newstarts.cn

Ruby: a, b = pair
来源：http://ef.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://yk.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://jg.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xl.shxzukj.cn

PHP:  // 无重载
来源：http://fb.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ms.hahajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://de.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zi.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://su.szxytkj.cn

Ruby: # 无重载：靠动态参数
来源：http://hu.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://sp.jctech888.com.cn

================================================================================
来源：http://dl.nicolike.cn

D. 数组 / 列表 / 集合
来源：http://wy.huanxung.cn

================================================================================
来源：http://vn.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://nj.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ym.shxzskj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nu.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lw.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hi.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oh.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ep.chemitech.net.cn

Ruby: arr = [1, 2, 3]
来源：http://ix.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qd.huixinmuqiang.cn

[D02] 追加元素到末尾
来源：http://ft.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gb.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sj.chemitech.net.cn

JS:   arr.push(4);
来源：http://jh.lnxyls.cn

TS:   arr.push(4);
来源：http://ii.shtwfgs.cn

Java: list.add(4);
来源：http://wy.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://mv.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://bi.szxytkj.cn

C#:   list.Add(4);
来源：http://gb.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://wx.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://gr.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lp.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kv.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://sm.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://re.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ew.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lh.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://la.colortex.cn

[D04] 删除元素
来源：http://pq.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sd.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mm.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pd.muxihuayi.cn

TS:   arr.splice(0, 1);
来源：http://wv.haigaiapp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bc.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://be.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ib.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bb.asd995.cn

[D05] 访问与修改元素
来源：http://bh.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hs.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wj.muxihuayi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zi.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://yf.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://pw.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://bn.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cq.chemitech.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://al.yuntaijiaju.cn

[D06] 数组长度
来源：http://uc.szsharing.cn

Py:   len(arr)
来源：http://ik.yuexingan06.cn

PHP:  count($arr);
来源：http://cw.521024.cn

JS:   arr.length
来源：http://ke.panjiajie.cn

TS:   arr.length
来源：http://fi.nszjky.cn

Java: list.size();
来源：http://ax.szxytkj.cn

Go:   len(arr)
来源：http://an.colortex.cn

Ruby: arr.length; arr.size
来源：http://pi.yuexingan06.cn

C#:   list.Count;
来源：http://de.nicolike.cn

[D07] 切片 / 取子数组
来源：http://dj.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jz.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mz.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://xn.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://tw.nszjky.cn

Java: list.subList(1, 4);
来源：http://cy.muxihuayi.cn

Go:   arr[1:4]
来源：http://rw.nicolike.cn

Ruby: arr[1, 3]
来源：http://ha.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://dl.colortex.cn

[D08] 合并两个数组
来源：http://hs.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://qk.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://pu.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uv.hnjuh.cn

TS:   [...a, ...b];
来源：http://wz.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ww.nszjky.cn

Go:   append(a, b...)
来源：http://vs.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://pn.521024.cn

C#:   a.Concat(b).ToList()
来源：http://to.nszjky.cn

[D09] 排序（升序）
来源：http://ua.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://gn.asd995.cn

PHP:  sort($arr);
来源：http://nm.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vz.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tz.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sr.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cm.hnjuh.cn

Ruby: arr.sort
来源：http://ca.shxzskj.cn

C#:   list.Sort();
来源：http://bh.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qi.wgjwhj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rp.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://td.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bp.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bh.huixiangedu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kq.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fd.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pp.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aj.wgjwhj.cn

[D11] 反转数组
来源：http://dq.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hl.szsharing.cn

PHP:  array_reverse($arr);
来源：http://jq.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jm.9csxet.cn

TS:   [...arr].reverse();
来源：http://sn.huanxung.cn

Java: Collections.reverse(list);
来源：http://zc.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://fn.shxzskj.cn

Ruby: arr.reverse
来源：http://kj.huanxung.cn

C#:   list.Reverse();
来源：http://pk.hnjuh.cn

[D12] 查找元素下标
来源：http://pc.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://nj.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ng.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sr.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://no.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xc.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ca.panjiajie.cn

Ruby: arr.index(x)
来源：http://gu.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://lv.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://uc.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ln.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xy.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://vp.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://tl.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jq.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nb.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bb.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eh.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://fe.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hw.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ul.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://rj.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://ow.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hc.hnjuh.cn

Go:   // 手写循环
来源：http://kw.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uk.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cx.jctech888.com.cn

[D15] 去重
来源：http://ck.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wo.nicolike.cn

PHP:  array_unique($arr);
来源：http://dm.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://ve.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://ss.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ri.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ap.hahajie.cn

Ruby: arr.uniq
来源：http://fu.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://ub.szsharing.cn

[D16] 求和与平均值
来源：http://um.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vb.yuntaijiaju.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://re.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://er.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oa.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ro.asd995.cn

Go:   // 手写循环累加
来源：http://kr.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dh.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://lf.huanxung.cn

[D17] 最大值与最小值
来源：http://vv.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://jg.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://on.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vu.gzmigu.cn

TS:   Math.max(...arr);
来源：http://ae.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hc.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cu.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://rc.asd995.cn

C#:   list.Max();  list.Min()
来源：http://bb.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://vb.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gy.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://rb.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qu.yuexingan06.cn

TS:   nested.flat();
来源：http://ak.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zz.muxihuayi.cn

Go:   // 手写双层循环
来源：http://eg.bookmarksfly.cn

Ruby: nested.flatten
来源：http://ws.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kx.jianghongdianzi.cn


<!-- 参考信息 -->