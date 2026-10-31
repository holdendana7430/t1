代发 wailian999

[C02] 默认参数
来源：http://an.colortex.cn

Py:   def greet(name="World"): return name
来源：http://ov.shtwfgs.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dm.huixinmuqiang.cn

JS:   function greet(name = "World") { return name; }
来源：http://ig.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bj.haigaiapp.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lx.hnjuh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yw.asd995.cn

Ruby: def greet(name = "World") = name
来源：http://br.hahajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://qh.huanxung.cn

[C03] 可变参数
来源：http://fg.chemitech.net.cn

Py:   def total(*args): return sum(args)
来源：http://gp.colortex.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bn.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pd.shtwfgs.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vg.wgjwhj.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://li.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wm.bjjhwx.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kn.szxytkj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://on.lnxyls.cn

[C04] 命名参数 / 关键字参数
来源：http://an.jctech888.com.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rm.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vn.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xd.asd995.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kj.colortex.cn

Java: // 无：用 Builder 模式或 record
来源：http://lg.bookmarksfly.cn

Go:   // 无：用配置结构体参数
来源：http://xs.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://ob.bookmarksfly.cn

C#:   f(a: 1, b: 2)
来源：http://hz.haigaiapp.cn

[C05] 返回多个值
来源：http://qm.shtwfgs.cn

Py:   return a, b
来源：http://ky.shtwfgs.cn

PHP:  return [$a, $b];
来源：http://oy.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fx.yuntaijiaju.cn

TS:   return { a, b };
来源：http://nt.nicolike.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://id.asd995.cn

Go:   return a, b
来源：http://py.shxzskj.cn

Ruby: return a, b
来源：http://ni.yuexingan06.cn

C#:   return (a, b);              // ValueTuple
来源：http://pp.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://cw.szxytkj.cn

Py:   square = lambda x: x * x
来源：http://zx.yuntaijiaju.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yw.9csxet.cn

JS:   const square = x => x * x;
来源：http://nx.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://eh.asd995.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ul.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yy.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://qb.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jj.huixinmuqiang.cn

[C07] 把函数作为参数传入
来源：http://kl.chemitech.net.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lp.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vq.yuexingan06.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vu.huanxung.cn

TS:   arr.map(String)
来源：http://ya.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xy.lnxyls.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ip.9csxet.cn

Ruby: arr.map(&:upcase)
来源：http://ri.yuntaijiaju.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jt.hahajie.cn

[C08] 闭包
来源：http://xq.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://po.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mm.nicolike.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wu.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kk.panjiajie.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kq.panjiajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rd.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ug.newstarts.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ff.newstarts.cn

[C09] 递归
来源：http://ir.wgjwhj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ax.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ho.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lo.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yv.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lg.nicolike.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ts.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gb.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sr.yuexingan06.cn

[C10] 变量作用域
来源：http://fo.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cx.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jc.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sa.chemitech.net.cn

TS:   同 JS
来源：http://lz.gzmigu.cn

Java: 方法内为块级作用域
来源：http://zk.jianghongdianzi.cn

Go:   花括号块级作用域
来源：http://me.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yc.asd995.cn

C#:   块级作用域
来源：http://rs.bjjhwx.cn

[C11] 模块导入与导出
来源：http://mb.yuntaijiaju.cn

Py:   from module import func
来源：http://hf.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wx.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zf.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bv.bookmarksfly.cn

Java: import java.util.List;
来源：http://sd.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://so.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://gj.szxytkj.cn

C#:   using System.Text;
来源：http://bf.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://qg.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://mf.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://fr.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://ke.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://sh.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ou.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://cf.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://pd.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rk.yuexingan06.cn

[C13] 类型声明 / 类型注解
来源：http://hw.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hm.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tv.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iz.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://go.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jw.jianghongdianzi.cn

Go:   func add(a, b int) int
来源：http://zy.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vj.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ny.bookmarksfly.cn

[C14] 泛型函数
来源：http://rd.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kl.wgjwhj.cn

PHP:  // 无泛型
来源：http://am.shtwfgs.cn

JS:   // 无泛型
来源：http://zw.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://au.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fc.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xj.shtwfgs.cn

Ruby: # 无泛型
来源：http://po.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rj.nszjky.cn

[C15] 解构 / 展开参数
来源：http://tx.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vv.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://bo.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jo.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hd.yuexingan06.cn

Java: // 无解构
来源：http://yn.yuntaijiaju.cn

Go:   // 无解构
来源：http://pt.newstarts.cn

Ruby: a, b = pair
来源：http://jh.hahajie.cn

C#:   var (a, b) = pair;
来源：http://de.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ao.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kx.shtwfgs.cn

PHP:  // 无重载
来源：http://mv.asd995.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jf.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://ox.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hp.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://co.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://xa.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wd.521024.cn

================================================================================
来源：http://ud.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://jp.newstarts.cn

================================================================================
来源：http://ex.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://td.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://no.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yj.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://da.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wi.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sy.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://vt.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://sc.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://af.bookmarksfly.cn

[D02] 追加元素到末尾
来源：http://ft.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dk.hnjuh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dy.nszjky.cn

JS:   arr.push(4);
来源：http://qr.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://lf.yuntaijiaju.cn

Java: list.add(4);
来源：http://zd.haigaiapp.cn

Go:   arr = append(arr, 4)
来源：http://vb.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://uc.panjiajie.cn

C#:   list.Add(4);
来源：http://vi.haigaiapp.cn

[D03] 在指定位置插入元素
来源：http://fh.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://tl.muxihuayi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vn.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://es.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://ca.huanxung.cn

Java: list.add(0, 0);
来源：http://bu.jctech888.com.cn

Go:   arr = append([]int{0}, arr...)
来源：http://if.nicolike.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://be.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://ti.szsharing.cn

[D04] 删除元素
来源：http://wy.huixiangedu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dw.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gj.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sw.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://hw.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cu.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rn.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kp.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wu.huanxung.cn

[D05] 访问与修改元素
来源：http://pd.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rh.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aj.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://li.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://rw.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://oq.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://zy.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wl.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fz.asd995.cn

[D06] 数组长度
来源：http://gh.haigaiapp.cn

Py:   len(arr)
来源：http://ri.hahajie.cn

PHP:  count($arr);
来源：http://vf.shtwfgs.cn

JS:   arr.length
来源：http://ub.jianghongdianzi.cn

TS:   arr.length
来源：http://gi.yuntaijiaju.cn

Java: list.size();
来源：http://un.9csxet.cn

Go:   len(arr)
来源：http://yh.521024.cn

Ruby: arr.length; arr.size
来源：http://ud.yuntaijiaju.cn

C#:   list.Count;
来源：http://op.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://qv.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tu.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pa.colortex.cn

JS:   arr.slice(1, 4);
来源：http://zn.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://hi.hnjuh.cn

Java: list.subList(1, 4);
来源：http://zs.szxytkj.cn

Go:   arr[1:4]
来源：http://mz.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://fk.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://sk.panjiajie.cn

[D08] 合并两个数组
来源：http://xu.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://dr.muxihuayi.cn

PHP:  array_merge($a, $b);
来源：http://vo.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vb.newstarts.cn

TS:   [...a, ...b];
来源：http://gs.yuntaijiaju.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hs.hnjuh.cn

Go:   append(a, b...)
来源：http://fs.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://qv.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://st.asd995.cn

[D09] 排序（升序）
来源：http://pr.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://iv.jctech888.com.cn

PHP:  sort($arr);
来源：http://ee.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hu.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gp.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xg.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qe.shxzskj.cn

Ruby: arr.sort
来源：http://fg.jianghongdianzi.cn

C#:   list.Sort();
来源：http://ke.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sj.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xa.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bw.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://py.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tg.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vg.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wg.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://um.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nq.huixiangedu.cn

[D11] 反转数组
来源：http://zu.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cf.szsharing.cn

PHP:  array_reverse($arr);
来源：http://rq.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jk.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://st.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://ru.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://kz.muxihuayi.cn

Ruby: arr.reverse
来源：http://ml.shxzukj.cn

C#:   list.Reverse();
来源：http://mo.huanxung.cn

[D12] 查找元素下标
来源：http://gu.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://gd.jctech888.com.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bj.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://as.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nf.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oc.colortex.cn

Go:   slices.Index(arr, x)
来源：http://ed.jctech888.com.cn

Ruby: arr.index(x)
来源：http://wl.hahajie.cn

C#:   list.IndexOf(x);
来源：http://ak.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://tx.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ne.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rh.shtwfgs.cn

JS:   arr.filter(x => x > 3)
来源：http://gq.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://ca.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nn.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nl.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hq.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ej.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://ht.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ny.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sx.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://tp.shxzukj.cn

TS:   arr.map(x => x * 2)
来源：http://bb.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ed.colortex.cn

Go:   // 手写循环
来源：http://oe.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rh.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ar.lnxyls.cn

[D15] 去重
来源：http://eb.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://be.panjiajie.cn

PHP:  array_unique($arr);
来源：http://uh.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://bt.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://tl.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yk.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fp.lnxyls.cn

Ruby: arr.uniq
来源：http://db.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://aj.haigaiapp.cn

[D16] 求和与平均值
来源：http://ne.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sk.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pa.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pb.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dx.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://of.shtwfgs.cn

Go:   // 手写循环累加
来源：http://wf.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://df.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://je.asd995.cn

[D17] 最大值与最小值
来源：http://ai.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://de.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://pb.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vv.asd995.cn

TS:   Math.max(...arr);
来源：http://ca.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://je.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wi.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://mm.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://vx.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://ul.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vi.colortex.cn

PHP:  array_merge(...$nested);
来源：http://na.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tj.jianghongdianzi.cn

TS:   nested.flat();
来源：http://zu.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ow.shxzskj.cn

Go:   // 手写双层循环
来源：http://qq.bjjhwx.cn

Ruby: nested.flatten
来源：http://gi.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nw.bjjhwx.cn


<!-- 参考信息 -->