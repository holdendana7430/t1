代发 wailian999

================================================================================
来源：http://qm.nicolike.cn

C. 函数与作用域
来源：http://nz.yuntaijiaju.cn

================================================================================
来源：http://qm.huixinmuqiang.cn

[C01] 定义函数
来源：http://wj.shxzukj.cn

Py:   def add(a, b): return a + b
来源：http://cv.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uo.panjiajie.cn

JS:   function add(a, b) { return a + b; }
来源：http://zl.wgjwhj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zn.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eo.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rd.9csxet.cn

Ruby: def add(a, b); a + b; end
来源：http://vi.szxytkj.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jc.hnjuh.cn

[C02] 默认参数
来源：http://kx.shxzukj.cn

Py:   def greet(name="World"): return name
来源：http://qq.9csxet.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fm.asd995.cn

JS:   function greet(name = "World") { return name; }
来源：http://ua.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nf.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rd.jianghongdianzi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pl.hahajie.cn

Ruby: def greet(name = "World") = name
来源：http://vp.haigaiapp.cn

C#:   string Greet(string name = "World") => name;
来源：http://gq.muxihuayi.cn

[C03] 可变参数
来源：http://xd.colortex.cn

Py:   def total(*args): return sum(args)
来源：http://sc.shtwfgs.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://au.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bs.gzmigu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iz.gzmigu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xi.colortex.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kj.chemitech.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ua.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kw.huixiangedu.cn

[C04] 命名参数 / 关键字参数
来源：http://bw.asd995.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mf.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yu.panjiajie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xl.nicolike.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dc.szxytkj.cn

Java: // 无：用 Builder 模式或 record
来源：http://le.shxzskj.cn

Go:   // 无：用配置结构体参数
来源：http://oo.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://os.521024.cn

C#:   f(a: 1, b: 2)
来源：http://xi.gzmigu.cn

[C05] 返回多个值
来源：http://nl.huixiangedu.cn

Py:   return a, b
来源：http://nf.hahajie.cn

PHP:  return [$a, $b];
来源：http://ks.bookmarksfly.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oe.lnxyls.cn

TS:   return { a, b };
来源：http://rx.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rx.bjjhwx.cn

Go:   return a, b
来源：http://gh.9csxet.cn

Ruby: return a, b
来源：http://gj.yuntaijiaju.cn

C#:   return (a, b);              // ValueTuple
来源：http://ss.jctech888.com.cn

[C06] 匿名函数 / lambda
来源：http://qw.huanxung.cn

Py:   square = lambda x: x * x
来源：http://ob.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kv.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://lq.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://fa.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://on.nszjky.cn

Go:   sq := func(x int) int { return x * x }
来源：http://in.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://gw.szsharing.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cx.newstarts.cn

[C07] 把函数作为参数传入
来源：http://sb.hahajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ne.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zy.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oo.bookmarksfly.cn

TS:   arr.map(String)
来源：http://lt.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lt.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uc.panjiajie.cn

Ruby: arr.map(&:upcase)
来源：http://hj.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cv.521024.cn

[C08] 闭包
来源：http://db.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nc.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://em.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://aa.521024.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cg.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eu.haigaiapp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kw.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kd.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://um.nszjky.cn

[C09] 递归
来源：http://pj.gzmigu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ck.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rw.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://is.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bt.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nz.hahajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://od.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lk.shxzukj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ak.haigaiapp.cn

[C10] 变量作用域
来源：http://fo.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://my.9csxet.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jp.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fz.9csxet.cn

TS:   同 JS
来源：http://cn.9csxet.cn

Java: 方法内为块级作用域
来源：http://dk.newstarts.cn

Go:   花括号块级作用域
来源：http://ur.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://km.jianghongdianzi.cn

C#:   块级作用域
来源：http://qd.gzmigu.cn

[C11] 模块导入与导出
来源：http://wc.chemitech.net.cn

Py:   from module import func
来源：http://uh.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qh.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ll.asd995.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mu.shtwfgs.cn

Java: import java.util.List;
来源：http://hk.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fm.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://dj.9csxet.cn

C#:   using System.Text;
来源：http://sw.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://ak.colortex.cn

Py:   (lambda: print("run"))()
来源：http://vw.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://fq.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://uw.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://su.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fi.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://uh.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://rw.shxzukj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lv.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://ci.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wi.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ez.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xa.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hc.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nl.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://jq.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ta.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ma.shtwfgs.cn

[C14] 泛型函数
来源：http://cj.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ew.bookmarksfly.cn

PHP:  // 无泛型
来源：http://zr.wgjwhj.cn

JS:   // 无泛型
来源：http://vu.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zt.hahajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ng.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lh.shxzukj.cn

Ruby: # 无泛型
来源：http://dn.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yl.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://vk.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zj.yuexingan06.cn

PHP:  [$a, $b] = $pair;
来源：http://am.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nd.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yv.nszjky.cn

Java: // 无解构
来源：http://bw.yuntaijiaju.cn

Go:   // 无解构
来源：http://ar.yuexingan06.cn

Ruby: a, b = pair
来源：http://lv.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://tt.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ch.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ug.hahajie.cn

PHP:  // 无重载
来源：http://eg.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://en.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://pn.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ap.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://fd.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://mz.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://en.chemitech.net.cn

================================================================================
来源：http://cs.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://xj.9csxet.cn

================================================================================
来源：http://ty.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://yn.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://py.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lu.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ww.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ky.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fr.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://uj.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://zt.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pt.nszjky.cn

[D02] 追加元素到末尾
来源：http://yp.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://an.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oe.521024.cn

JS:   arr.push(4);
来源：http://in.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://tu.asd995.cn

Java: list.add(4);
来源：http://se.asd995.cn

Go:   arr = append(arr, 4)
来源：http://rl.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://vo.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://dl.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://bz.colortex.cn

Py:   arr.insert(0, 0)
来源：http://jl.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ad.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mi.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://vq.521024.cn

Java: list.add(0, 0);
来源：http://vf.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fs.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ub.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://ua.muxihuayi.cn

[D04] 删除元素
来源：http://iw.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lo.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pg.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ep.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://sg.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://da.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fe.wgjwhj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dy.huanxung.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hn.panjiajie.cn

[D05] 访问与修改元素
来源：http://kn.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cy.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gy.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vh.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://ug.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://qn.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://xu.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zj.huixinmuqiang.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yv.nicolike.cn

[D06] 数组长度
来源：http://pm.asd995.cn

Py:   len(arr)
来源：http://xe.huixinmuqiang.cn

PHP:  count($arr);
来源：http://ni.huanxung.cn

JS:   arr.length
来源：http://te.chemitech.net.cn

TS:   arr.length
来源：http://iu.shxzskj.cn

Java: list.size();
来源：http://hj.shxzskj.cn

Go:   len(arr)
来源：http://jk.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://nz.yuntaijiaju.cn

C#:   list.Count;
来源：http://fe.asd995.cn

[D07] 切片 / 取子数组
来源：http://mk.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xv.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fm.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://hs.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://et.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://su.9csxet.cn

Go:   arr[1:4]
来源：http://vh.szxytkj.cn

Ruby: arr[1, 3]
来源：http://jg.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://jv.wgjwhj.cn

[D08] 合并两个数组
来源：http://qu.jianghongdianzi.cn

Py:   a + b;  a.extend(b)
来源：http://qg.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://ke.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fu.shxzskj.cn

TS:   [...a, ...b];
来源：http://bp.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tx.yuexingan06.cn

Go:   append(a, b...)
来源：http://eb.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://on.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://xa.wgjwhj.cn

[D09] 排序（升序）
来源：http://lz.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://jm.521024.cn

PHP:  sort($arr);
来源：http://at.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ts.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qp.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cn.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yy.newstarts.cn

Ruby: arr.sort
来源：http://vd.9csxet.cn

C#:   list.Sort();
来源：http://kd.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nr.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uq.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ut.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gm.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zv.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qf.newstarts.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xb.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rw.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hc.521024.cn

[D11] 反转数组
来源：http://xu.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ct.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://zp.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yg.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://jk.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://nz.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://gt.nicolike.cn

Ruby: arr.reverse
来源：http://kf.hahajie.cn

C#:   list.Reverse();
来源：http://cd.hahajie.cn

[D12] 查找元素下标
来源：http://fr.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://op.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yf.hahajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kn.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dw.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xm.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://jr.colortex.cn

Ruby: arr.index(x)
来源：http://kq.newstarts.cn

C#:   list.IndexOf(x);
来源：http://ds.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://te.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ku.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uk.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://vt.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ut.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sy.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kh.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tq.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ek.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://xj.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ni.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rp.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://kp.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://nr.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uw.hnjuh.cn

Go:   // 手写循环
来源：http://nx.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wc.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pw.colortex.cn

[D15] 去重
来源：http://jq.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lv.szsharing.cn

PHP:  array_unique($arr);
来源：http://yv.huanxung.cn

JS:   [...new Set(arr)]
来源：http://wp.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://zb.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bn.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gm.521024.cn

Ruby: arr.uniq
来源：http://nj.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://ag.szsharing.cn

[D16] 求和与平均值
来源：http://hf.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yt.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ug.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uf.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xz.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sp.shtwfgs.cn

Go:   // 手写循环累加
来源：http://wp.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yc.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://mk.colortex.cn

[D17] 最大值与最小值
来源：http://vb.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://dw.asd995.cn

PHP:  max($arr);  min($arr);
来源：http://tb.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bh.colortex.cn

TS:   Math.max(...arr);
来源：http://lk.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wd.asd995.cn


<!-- 参考信息 -->