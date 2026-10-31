代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gc.hnjuh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fe.asd995.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qw.asd995.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fp.shtwfgs.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ie.jianghongdianzi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nh.shxzukj.cn

[C04] 命名参数 / 关键字参数
来源：http://zo.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hu.newstarts.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ns.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tw.panjiajie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ox.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://te.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://os.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://wj.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://lp.lnxyls.cn

[C05] 返回多个值
来源：http://qw.hnjuh.cn

Py:   return a, b
来源：http://rg.colortex.cn

PHP:  return [$a, $b];
来源：http://nc.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hy.shxzukj.cn

TS:   return { a, b };
来源：http://hk.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ld.wgjwhj.cn

Go:   return a, b
来源：http://gm.szxytkj.cn

Ruby: return a, b
来源：http://op.9csxet.cn

C#:   return (a, b);              // ValueTuple
来源：http://wb.521024.cn

[C06] 匿名函数 / lambda
来源：http://oj.nicolike.cn

Py:   square = lambda x: x * x
来源：http://vl.huanxung.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pr.chemitech.net.cn

JS:   const square = x => x * x;
来源：http://fk.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://rr.szsharing.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oe.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wv.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://gt.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qg.huanxung.cn

[C07] 把函数作为参数传入
来源：http://ba.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gv.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jn.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rd.asd995.cn

TS:   arr.map(String)
来源：http://gs.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gq.shtwfgs.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ft.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://do.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://su.lnxyls.cn

[C08] 闭包
来源：http://on.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jz.szxytkj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cf.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vp.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://th.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gh.hahajie.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://on.haigaiapp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ls.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gv.nicolike.cn

[C09] 递归
来源：http://pk.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cn.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ac.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://su.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://km.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sc.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tp.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ze.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pt.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ll.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ou.shxzskj.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aw.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vn.asd995.cn

TS:   同 JS
来源：http://zw.huixinmuqiang.cn

Java: 方法内为块级作用域
来源：http://lc.haigaiapp.cn

Go:   花括号块级作用域
来源：http://nu.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uq.szxytkj.cn

C#:   块级作用域
来源：http://ep.jctech888.com.cn

[C11] 模块导入与导出
来源：http://bd.jctech888.com.cn

Py:   from module import func
来源：http://hj.szxytkj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wz.521024.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sm.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kl.wgjwhj.cn

Java: import java.util.List;
来源：http://bt.yuexingan06.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://au.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://uy.jctech888.com.cn

C#:   using System.Text;
来源：http://dz.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ba.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://jy.bjjhwx.cn

PHP:  (function () { echo "run"; })();
来源：http://ht.shtwfgs.cn

JS:   (() => { console.log("run"); })();
来源：http://xf.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://xv.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fn.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://rg.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://wk.jctech888.com.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lk.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://qa.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mq.szsharing.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tz.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ri.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nw.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gk.gzmigu.cn

Go:   func add(a, b int) int
来源：http://vs.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://la.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dn.gzmigu.cn

[C14] 泛型函数
来源：http://yk.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://al.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://lb.shxzskj.cn

JS:   // 无泛型
来源：http://ky.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fj.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gm.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mv.shxzskj.cn

Ruby: # 无泛型
来源：http://tx.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wq.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://zp.bjjhwx.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mp.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://ob.shtwfgs.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nq.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://va.muxihuayi.cn

Java: // 无解构
来源：http://hm.colortex.cn

Go:   // 无解构
来源：http://mb.panjiajie.cn

Ruby: a, b = pair
来源：http://ak.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://nj.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://yk.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gr.huanxung.cn

PHP:  // 无重载
来源：http://yq.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uo.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://dj.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ta.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://oq.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://sr.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ad.yuntaijiaju.cn

================================================================================
来源：http://hn.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://ep.bjjhwx.cn

================================================================================
来源：http://df.9csxet.cn

[D01] 创建数组 / 列表
来源：http://jn.haigaiapp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pm.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zb.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gx.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ia.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fn.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://ya.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://ec.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lw.szxytkj.cn

[D02] 追加元素到末尾
来源：http://vl.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jw.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nx.nszjky.cn

JS:   arr.push(4);
来源：http://bq.newstarts.cn

TS:   arr.push(4);
来源：http://ad.asd995.cn

Java: list.add(4);
来源：http://vz.asd995.cn

Go:   arr = append(arr, 4)
来源：http://ou.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://px.yuexingan06.cn

C#:   list.Add(4);
来源：http://cv.521024.cn

[D03] 在指定位置插入元素
来源：http://ye.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://zy.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kt.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bt.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://et.huixinmuqiang.cn

Java: list.add(0, 0);
来源：http://un.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bw.shxzskj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lu.colortex.cn

C#:   list.Insert(0, 0);
来源：http://jk.asd995.cn

[D04] 删除元素
来源：http://hj.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jy.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bd.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sr.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://kx.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ur.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jm.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wo.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://as.yuexingan06.cn

[D05] 访问与修改元素
来源：http://dh.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://im.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nx.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xi.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://kf.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://wm.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://yh.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vo.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ax.jianghongdianzi.cn

[D06] 数组长度
来源：http://qk.yuexingan06.cn

Py:   len(arr)
来源：http://np.wgjwhj.cn

PHP:  count($arr);
来源：http://fd.huixinmuqiang.cn

JS:   arr.length
来源：http://wf.colortex.cn

TS:   arr.length
来源：http://pa.huanxung.cn

Java: list.size();
来源：http://qp.szxytkj.cn

Go:   len(arr)
来源：http://sz.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://cj.shxzskj.cn

C#:   list.Count;
来源：http://vl.nicolike.cn

[D07] 切片 / 取子数组
来源：http://pn.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ym.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://im.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://jt.521024.cn

TS:   arr.slice(1, 4);
来源：http://le.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://mj.shxzukj.cn

Go:   arr[1:4]
来源：http://kw.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://xg.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://ex.huanxung.cn

[D08] 合并两个数组
来源：http://dx.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://nt.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://aa.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tr.newstarts.cn

TS:   [...a, ...b];
来源：http://mm.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lf.chemitech.net.cn

Go:   append(a, b...)
来源：http://ne.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://lr.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://ww.bookmarksfly.cn

[D09] 排序（升序）
来源：http://ea.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://jq.shtwfgs.cn

PHP:  sort($arr);
来源：http://fe.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lu.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bo.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gc.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sd.muxihuayi.cn

Ruby: arr.sort
来源：http://yk.huixiangedu.cn

C#:   list.Sort();
来源：http://eg.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nc.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ak.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hv.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ge.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ok.shxzukj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://it.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sf.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vi.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xb.lnxyls.cn

[D11] 反转数组
来源：http://iq.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zq.newstarts.cn

PHP:  array_reverse($arr);
来源：http://vc.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pa.nszjky.cn

TS:   [...arr].reverse();
来源：http://zn.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://xe.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://tf.szsharing.cn

Ruby: arr.reverse
来源：http://ki.colortex.cn

C#:   list.Reverse();
来源：http://tw.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://ql.521024.cn

Py:   arr.index(x);  x in arr
来源：http://zi.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cj.huanxung.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gc.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nn.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uu.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://gl.wgjwhj.cn

Ruby: arr.index(x)
来源：http://ey.newstarts.cn

C#:   list.IndexOf(x);
来源：http://uk.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://ji.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tf.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vx.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://vl.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://hc.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rq.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://et.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tt.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yh.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://qo.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://os.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ho.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ex.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://nh.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ro.nszjky.cn

Go:   // 手写循环
来源：http://un.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sy.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ej.szxytkj.cn

[D15] 去重
来源：http://ss.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://un.panjiajie.cn

PHP:  array_unique($arr);
来源：http://tm.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://qh.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://us.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lt.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ls.szxytkj.cn

Ruby: arr.uniq
来源：http://qv.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://kn.colortex.cn

[D16] 求和与平均值
来源：http://gf.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ls.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vl.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://du.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wo.panjiajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yo.gzmigu.cn

Go:   // 手写循环累加
来源：http://ci.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mq.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://wf.521024.cn

[D17] 最大值与最小值
来源：http://jj.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://wc.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://pf.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fw.shxzskj.cn

TS:   Math.max(...arr);
来源：http://ln.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qt.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yk.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://rz.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://st.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://do.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sh.asd995.cn

PHP:  array_merge(...$nested);
来源：http://sv.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qv.bookmarksfly.cn

TS:   nested.flat();
来源：http://hw.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hi.nszjky.cn

Go:   // 手写双层循环
来源：http://ds.jctech888.com.cn

Ruby: nested.flatten
来源：http://sv.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hq.huixinmuqiang.cn

[D19] 按字段分组
来源：http://fu.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bu.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dk.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qg.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jc.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cc.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://hc.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cc.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zm.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://ee.huixiangedu.cn

Py:   Counter(arr)
来源：http://gx.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://zq.hahajie.cn


<!-- 参考信息 -->