代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://ii.yuntaijiaju.cn

Go:   func add(a, b int) int { return a + b }
来源：http://pe.lnxyls.cn

Ruby: def add(a, b); a + b; end
来源：http://yv.nszjky.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mb.hnjuh.cn

[C02] 默认参数
来源：http://mm.huanxung.cn

Py:   def greet(name="World"): return name
来源：http://dg.jctech888.com.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://du.nszjky.cn

JS:   function greet(name = "World") { return name; }
来源：http://zf.huanxung.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://od.huixinmuqiang.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nb.shtwfgs.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ng.yuexingan06.cn

Ruby: def greet(name = "World") = name
来源：http://qy.gzmigu.cn

C#:   string Greet(string name = "World") => name;
来源：http://wp.wgjwhj.cn

[C03] 可变参数
来源：http://tv.bookmarksfly.cn

Py:   def total(*args): return sum(args)
来源：http://wu.lnxyls.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iu.bjjhwx.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xq.muxihuayi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zc.colortex.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lv.chemitech.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ts.jianghongdianzi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://es.colortex.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rn.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://jv.szxytkj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dv.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zw.jctech888.com.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://if.szsharing.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fs.521024.cn

Java: // 无：用 Builder 模式或 record
来源：http://mq.wgjwhj.cn

Go:   // 无：用配置结构体参数
来源：http://at.asd995.cn

Ruby: f(a: 1, b: 2)
来源：http://zb.huixiangedu.cn

C#:   f(a: 1, b: 2)
来源：http://eo.huixinmuqiang.cn

[C05] 返回多个值
来源：http://qv.shtwfgs.cn

Py:   return a, b
来源：http://oe.huixinmuqiang.cn

PHP:  return [$a, $b];
来源：http://sr.chemitech.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://cq.nszjky.cn

TS:   return { a, b };
来源：http://vz.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bx.hnjuh.cn

Go:   return a, b
来源：http://qp.chemitech.net.cn

Ruby: return a, b
来源：http://pi.hnjuh.cn

C#:   return (a, b);              // ValueTuple
来源：http://cb.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://vz.newstarts.cn

Py:   square = lambda x: x * x
来源：http://zg.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ix.521024.cn

JS:   const square = x => x * x;
来源：http://br.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://tk.gzmigu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gf.shtwfgs.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dd.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://xk.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dm.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://mx.bjjhwx.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gf.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ps.szxytkj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nb.gzmigu.cn

TS:   arr.map(String)
来源：http://sp.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://le.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://me.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://nv.jianghongdianzi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://id.asd995.cn

[C08] 闭包
来源：http://ro.shtwfgs.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ny.yuexingan06.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lc.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jo.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yo.huixinmuqiang.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jq.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ly.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fy.huixinmuqiang.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://be.gzmigu.cn

[C09] 递归
来源：http://or.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zx.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lq.hnjuh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qs.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://em.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ls.lnxyls.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pc.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dj.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qx.bookmarksfly.cn

[C10] 变量作用域
来源：http://or.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://oy.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nn.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ht.panjiajie.cn

TS:   同 JS
来源：http://bu.newstarts.cn

Java: 方法内为块级作用域
来源：http://wp.nszjky.cn

Go:   花括号块级作用域
来源：http://gw.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vj.wgjwhj.cn

C#:   块级作用域
来源：http://hd.jctech888.com.cn

[C11] 模块导入与导出
来源：http://zd.colortex.cn

Py:   from module import func
来源：http://id.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aq.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hg.shxzskj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pf.nicolike.cn

Java: import java.util.List;
来源：http://uq.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dt.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://tv.chemitech.net.cn

C#:   using System.Text;
来源：http://iy.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://zk.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://eo.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://em.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://qz.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://mj.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qr.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://fq.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://ac.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ph.muxihuayi.cn

[C13] 类型声明 / 类型注解
来源：http://od.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cu.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rg.colortex.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nv.hnjuh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oi.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yk.shxzskj.cn

Go:   func add(a, b int) int
来源：http://al.yuexingan06.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hj.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uo.hahajie.cn

[C14] 泛型函数
来源：http://jj.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xo.shxzskj.cn

PHP:  // 无泛型
来源：http://tj.nicolike.cn

JS:   // 无泛型
来源：http://xy.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sl.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jy.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kg.muxihuayi.cn

Ruby: # 无泛型
来源：http://wa.jianghongdianzi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yx.nszjky.cn

[C15] 解构 / 展开参数
来源：http://lw.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aa.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://au.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ck.muxihuayi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pg.yuntaijiaju.cn

Java: // 无解构
来源：http://ua.panjiajie.cn

Go:   // 无解构
来源：http://jj.bjjhwx.cn

Ruby: a, b = pair
来源：http://pj.newstarts.cn

C#:   var (a, b) = pair;
来源：http://tf.szsharing.cn

[C16] 函数 / 方法重载
来源：http://ah.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wi.huixinmuqiang.cn

PHP:  // 无重载
来源：http://jw.shtwfgs.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://el.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://ux.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cm.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://td.521024.cn

Ruby: # 无重载：靠动态参数
来源：http://lb.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://df.haigaiapp.cn

================================================================================
来源：http://hu.521024.cn

D. 数组 / 列表 / 集合
来源：http://vu.shxzskj.cn

================================================================================
来源：http://iy.nszjky.cn

[D01] 创建数组 / 列表
来源：http://qc.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fh.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nf.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dw.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dg.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://db.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://zq.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://bc.shtwfgs.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ne.huixiangedu.cn

[D02] 追加元素到末尾
来源：http://gn.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://it.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bb.huanxung.cn

JS:   arr.push(4);
来源：http://ab.huixiangedu.cn

TS:   arr.push(4);
来源：http://kh.szsharing.cn

Java: list.add(4);
来源：http://wn.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://uy.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://fs.yuexingan06.cn

C#:   list.Add(4);
来源：http://ey.521024.cn

[D03] 在指定位置插入元素
来源：http://wk.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://ok.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://of.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bi.huanxung.cn

TS:   arr.splice(0, 0, 0);
来源：http://lq.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://hg.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qu.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kb.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://cj.asd995.cn

[D04] 删除元素
来源：http://te.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qa.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yg.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rt.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://np.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tf.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tf.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tu.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cv.shxzukj.cn

[D05] 访问与修改元素
来源：http://hf.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wi.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jb.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gs.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://fj.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://rh.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://uf.asd995.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gr.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ux.huixinmuqiang.cn

[D06] 数组长度
来源：http://pd.colortex.cn

Py:   len(arr)
来源：http://vr.panjiajie.cn

PHP:  count($arr);
来源：http://zu.nicolike.cn

JS:   arr.length
来源：http://ng.huixinmuqiang.cn

TS:   arr.length
来源：http://zv.shxzskj.cn

Java: list.size();
来源：http://mz.huanxung.cn

Go:   len(arr)
来源：http://di.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://zk.shxzukj.cn

C#:   list.Count;
来源：http://qf.huanxung.cn

[D07] 切片 / 取子数组
来源：http://zf.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oe.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://es.huixinmuqiang.cn

JS:   arr.slice(1, 4);
来源：http://eq.newstarts.cn

TS:   arr.slice(1, 4);
来源：http://iy.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://mh.huanxung.cn

Go:   arr[1:4]
来源：http://mw.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://ek.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://zw.nicolike.cn

[D08] 合并两个数组
来源：http://hs.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://cq.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://md.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cj.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ka.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dm.521024.cn

Go:   append(a, b...)
来源：http://wl.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://lz.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://hh.bookmarksfly.cn

[D09] 排序（升序）
来源：http://ln.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://ux.shxzukj.cn

PHP:  sort($arr);
来源：http://uf.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nd.huixinmuqiang.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tl.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ez.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bm.huanxung.cn

Ruby: arr.sort
来源：http://by.newstarts.cn

C#:   list.Sort();
来源：http://dq.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ye.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rm.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ca.newstarts.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hk.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lk.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lx.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://av.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://me.yuexingan06.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://om.huixiangedu.cn

[D11] 反转数组
来源：http://bj.panjiajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://et.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://yk.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qz.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://cn.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://qu.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://it.hnjuh.cn

Ruby: arr.reverse
来源：http://qo.gzmigu.cn

C#:   list.Reverse();
来源：http://nq.9csxet.cn

[D12] 查找元素下标
来源：http://rt.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://dt.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qe.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zh.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://et.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fz.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://vj.gzmigu.cn

Ruby: arr.index(x)
来源：http://cf.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://dz.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://sh.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qm.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://if.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://ub.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://of.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://as.szsharing.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xw.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cj.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wd.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://fj.shxzskj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cj.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pt.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://sm.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://zu.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sr.huanxung.cn

Go:   // 手写循环
来源：http://pj.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xm.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sf.huixinmuqiang.cn

[D15] 去重
来源：http://vg.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qs.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://pp.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://px.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://vi.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ce.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gy.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://wy.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://ju.wgjwhj.cn

[D16] 求和与平均值
来源：http://ok.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vs.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oc.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://df.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ac.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sz.hahajie.cn

Go:   // 手写循环累加
来源：http://rv.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zw.521024.cn

C#:   list.Sum();  list.Average()
来源：http://iy.gzmigu.cn

[D17] 最大值与最小值
来源：http://nq.colortex.cn

Py:   max(arr);  min(arr)
来源：http://er.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://tt.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tx.hahajie.cn

TS:   Math.max(...arr);
来源：http://op.shxzskj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cs.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pc.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://km.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://vl.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://dn.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kr.521024.cn

PHP:  array_merge(...$nested);
来源：http://se.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://du.nszjky.cn

TS:   nested.flat();
来源：http://qv.lnxyls.cn


<!-- 参考信息 -->