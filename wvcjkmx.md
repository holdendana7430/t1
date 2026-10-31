代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://xr.hahajie.cn

[C03] 可变参数
来源：http://bt.szxytkj.cn

Py:   def total(*args): return sum(args)
来源：http://hm.jianghongdianzi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gg.jctech888.com.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fi.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://um.hnjuh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bq.shxzukj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ag.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ru.hahajie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ga.nszjky.cn

[C04] 命名参数 / 关键字参数
来源：http://xp.yuexingan06.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hc.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cj.lnxyls.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dh.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lp.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://bo.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://av.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://xg.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://zg.huixinmuqiang.cn

[C05] 返回多个值
来源：http://rf.panjiajie.cn

Py:   return a, b
来源：http://ig.szxytkj.cn

PHP:  return [$a, $b];
来源：http://lv.haigaiapp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://he.9csxet.cn

TS:   return { a, b };
来源：http://lq.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://le.yuexingan06.cn

Go:   return a, b
来源：http://sn.521024.cn

Ruby: return a, b
来源：http://nv.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://qg.haigaiapp.cn

[C06] 匿名函数 / lambda
来源：http://ez.9csxet.cn

Py:   square = lambda x: x * x
来源：http://fa.asd995.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ht.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://yx.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ez.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oq.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sl.huixinmuqiang.cn

Ruby: square = ->(x) { x * x }
来源：http://of.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gt.szsharing.cn

[C07] 把函数作为参数传入
来源：http://bx.asd995.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nc.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ap.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lm.muxihuayi.cn

TS:   arr.map(String)
来源：http://ap.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mn.panjiajie.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rq.huixinmuqiang.cn

Ruby: arr.map(&:upcase)
来源：http://fa.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://em.huanxung.cn

[C08] 闭包
来源：http://gy.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uf.bookmarksfly.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vv.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ov.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bx.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kr.shxzskj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ls.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ha.huixiangedu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rx.chemitech.net.cn

[C09] 递归
来源：http://qo.jianghongdianzi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qf.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sa.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lf.haigaiapp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yw.jctech888.com.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://co.nszjky.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://si.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fa.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uk.asd995.cn

[C10] 变量作用域
来源：http://od.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://je.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bg.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jr.shxzskj.cn

TS:   同 JS
来源：http://na.yuntaijiaju.cn

Java: 方法内为块级作用域
来源：http://ez.shxzukj.cn

Go:   花括号块级作用域
来源：http://ga.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://us.szsharing.cn

C#:   块级作用域
来源：http://fs.lnxyls.cn

[C11] 模块导入与导出
来源：http://yn.huixiangedu.cn

Py:   from module import func
来源：http://nn.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hv.muxihuayi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ut.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ge.hahajie.cn

Java: import java.util.List;
来源：http://dp.asd995.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fb.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://hv.nicolike.cn

C#:   using System.Text;
来源：http://vy.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://vt.nicolike.cn

Py:   (lambda: print("run"))()
来源：http://ul.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://yz.shxzukj.cn

JS:   (() => { console.log("run"); })();
来源：http://ei.jianghongdianzi.cn

TS:   (() => { console.log("run"); })();
来源：http://tq.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ia.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://fc.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://yv.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ia.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://uy.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://al.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ey.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ul.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uu.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ai.szsharing.cn

Go:   func add(a, b int) int
来源：http://eo.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://us.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nx.521024.cn

[C14] 泛型函数
来源：http://ba.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dg.shxzskj.cn

PHP:  // 无泛型
来源：http://js.panjiajie.cn

JS:   // 无泛型
来源：http://jp.haigaiapp.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fs.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ay.chemitech.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://br.chemitech.net.cn

Ruby: # 无泛型
来源：http://yl.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ob.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://sr.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gq.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://ik.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://in.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://of.shxzskj.cn

Java: // 无解构
来源：http://on.lnxyls.cn

Go:   // 无解构
来源：http://ju.9csxet.cn

Ruby: a, b = pair
来源：http://ni.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://dm.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://aa.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sd.wgjwhj.cn

PHP:  // 无重载
来源：http://pv.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ss.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://wx.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ti.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://kz.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://vo.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nw.jctech888.com.cn

================================================================================
来源：http://kx.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://ln.bookmarksfly.cn

================================================================================
来源：http://gg.asd995.cn

[D01] 创建数组 / 列表
来源：http://rc.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hr.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gt.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qu.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ex.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tf.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://tf.bjjhwx.cn

Ruby: arr = [1, 2, 3]
来源：http://eg.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gj.shxzukj.cn

[D02] 追加元素到末尾
来源：http://jo.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wo.nszjky.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://st.panjiajie.cn

JS:   arr.push(4);
来源：http://hj.huixiangedu.cn

TS:   arr.push(4);
来源：http://bf.shxzskj.cn

Java: list.add(4);
来源：http://lt.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://zo.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://yg.shxzskj.cn

C#:   list.Add(4);
来源：http://ua.huanxung.cn

[D03] 在指定位置插入元素
来源：http://bj.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://dh.szxytkj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jr.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://pt.szxytkj.cn

Java: list.add(0, 0);
来源：http://la.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tm.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aj.haigaiapp.cn

C#:   list.Insert(0, 0);
来源：http://uh.lnxyls.cn

[D04] 删除元素
来源：http://dt.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ua.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wp.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mr.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://kn.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xd.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://as.shxzukj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yc.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ys.wgjwhj.cn

[D05] 访问与修改元素
来源：http://gu.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mr.9csxet.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fo.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dm.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://hg.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://fc.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://vm.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pb.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fc.colortex.cn

[D06] 数组长度
来源：http://id.colortex.cn

Py:   len(arr)
来源：http://ot.nicolike.cn

PHP:  count($arr);
来源：http://zb.bjjhwx.cn

JS:   arr.length
来源：http://ta.shtwfgs.cn

TS:   arr.length
来源：http://io.lnxyls.cn

Java: list.size();
来源：http://lk.shxzskj.cn

Go:   len(arr)
来源：http://wb.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://sf.huanxung.cn

C#:   list.Count;
来源：http://iz.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://fc.shxzukj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bz.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ju.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://he.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://dx.hahajie.cn

Java: list.subList(1, 4);
来源：http://rb.panjiajie.cn

Go:   arr[1:4]
来源：http://rc.hahajie.cn

Ruby: arr[1, 3]
来源：http://fl.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://ga.panjiajie.cn

[D08] 合并两个数组
来源：http://fq.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://bj.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://bx.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ns.haigaiapp.cn

TS:   [...a, ...b];
来源：http://hz.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qw.gzmigu.cn

Go:   append(a, b...)
来源：http://ot.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://dz.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://cx.9csxet.cn

[D09] 排序（升序）
来源：http://tw.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://vn.huixiangedu.cn

PHP:  sort($arr);
来源：http://dq.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vt.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sf.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://so.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mh.jctech888.com.cn

Ruby: arr.sort
来源：http://ei.nszjky.cn

C#:   list.Sort();
来源：http://fp.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sz.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gy.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nz.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cs.hnjuh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zr.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sa.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yq.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sq.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nw.bjjhwx.cn

[D11] 反转数组
来源：http://dt.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uj.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://hi.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://im.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://hz.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://ca.huanxung.cn

Ruby: arr.reverse
来源：http://ou.huanxung.cn

C#:   list.Reverse();
来源：http://cp.nszjky.cn

[D12] 查找元素下标
来源：http://jx.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://ox.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bn.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yd.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ub.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qf.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://cf.nszjky.cn

Ruby: arr.index(x)
来源：http://yh.asd995.cn

C#:   list.IndexOf(x);
来源：http://vq.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://nt.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://da.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cw.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://zw.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://oc.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hn.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rp.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nl.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rp.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://km.nszjky.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ye.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jq.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://gl.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://sk.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gr.shtwfgs.cn

Go:   // 手写循环
来源：http://na.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cx.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qf.bookmarksfly.cn

[D15] 去重
来源：http://qn.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nk.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://af.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://wt.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://zo.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://va.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eb.newstarts.cn

Ruby: arr.uniq
来源：http://ft.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://np.huixiangedu.cn

[D16] 求和与平均值
来源：http://ms.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xp.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eu.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qh.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vq.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bz.shxzskj.cn

Go:   // 手写循环累加
来源：http://ya.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://in.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://vi.colortex.cn

[D17] 最大值与最小值
来源：http://rw.colortex.cn

Py:   max(arr);  min(arr)
来源：http://jy.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://wu.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://od.newstarts.cn

TS:   Math.max(...arr);
来源：http://jt.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://in.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cn.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://oh.521024.cn

C#:   list.Max();  list.Min()
来源：http://lj.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://up.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vz.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://hk.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dr.szsharing.cn

TS:   nested.flat();
来源：http://hs.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ak.haigaiapp.cn

Go:   // 手写双层循环
来源：http://wc.bjjhwx.cn

Ruby: nested.flatten
来源：http://tz.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ix.huanxung.cn

[D19] 按字段分组
来源：http://ib.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lu.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mn.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tc.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ap.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yw.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://bh.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://si.bookmarksfly.cn


<!-- 参考信息 -->