代发 wailian999

Py:   if not data: return
来源：http://ko.haigaiapp.cn

PHP:  if (!$data) { return; }
来源：http://at.shxzukj.cn

JS:   if (!data) return;
来源：http://gh.bjjhwx.cn

TS:   if (!data) return;
来源：http://qm.bookmarksfly.cn

Java: if (data == null) return;
来源：http://ue.szxytkj.cn

Go:   if data == nil { return }
来源：http://gx.shtwfgs.cn

Ruby: return if data.nil?
来源：http://fr.nszjky.cn

C#:   if (data == null) return;
来源：http://zl.shxzskj.cn

================================================================================
来源：http://sn.bookmarksfly.cn

C. 函数与作用域
来源：http://bc.haigaiapp.cn

================================================================================
来源：http://uo.wgjwhj.cn

[C01] 定义函数
来源：http://xf.huixiangedu.cn

Py:   def add(a, b): return a + b
来源：http://gi.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gm.colortex.cn

JS:   function add(a, b) { return a + b; }
来源：http://jd.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://np.huanxung.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cp.huixinmuqiang.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nh.muxihuayi.cn

Ruby: def add(a, b); a + b; end
来源：http://bk.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zv.chemitech.net.cn

[C02] 默认参数
来源：http://rf.lnxyls.cn

Py:   def greet(name="World"): return name
来源：http://ef.colortex.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xx.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://ai.huixinmuqiang.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kb.nicolike.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qp.colortex.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bp.huanxung.cn

Ruby: def greet(name = "World") = name
来源：http://iv.jianghongdianzi.cn

C#:   string Greet(string name = "World") => name;
来源：http://kk.panjiajie.cn

[C03] 可变参数
来源：http://zq.asd995.cn

Py:   def total(*args): return sum(args)
来源：http://qx.haigaiapp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ea.hahajie.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ky.bookmarksfly.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pg.yuntaijiaju.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zb.szxytkj.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qm.521024.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kw.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fq.jianghongdianzi.cn

[C04] 命名参数 / 关键字参数
来源：http://bw.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nc.shxzskj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jj.wgjwhj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ty.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kp.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://co.asd995.cn

Go:   // 无：用配置结构体参数
来源：http://lp.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://sq.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://zh.haigaiapp.cn

[C05] 返回多个值
来源：http://vy.haigaiapp.cn

Py:   return a, b
来源：http://fp.hahajie.cn

PHP:  return [$a, $b];
来源：http://gm.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sc.lnxyls.cn

TS:   return { a, b };
来源：http://eq.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zj.huixiangedu.cn

Go:   return a, b
来源：http://gg.bjjhwx.cn

Ruby: return a, b
来源：http://if.shtwfgs.cn

C#:   return (a, b);              // ValueTuple
来源：http://ir.colortex.cn

[C06] 匿名函数 / lambda
来源：http://zw.yuexingan06.cn

Py:   square = lambda x: x * x
来源：http://jd.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gl.shxzukj.cn

JS:   const square = x => x * x;
来源：http://jc.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://uv.521024.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uo.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://md.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://ll.huixiangedu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ch.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://hh.hnjuh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ir.chemitech.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vj.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://px.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://ah.huixinmuqiang.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://no.hnjuh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dg.nszjky.cn

Ruby: arr.map(&:upcase)
来源：http://qz.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://du.szxytkj.cn

[C08] 闭包
来源：http://yi.bookmarksfly.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oy.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ks.wgjwhj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ku.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uo.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wb.muxihuayi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dq.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://za.muxihuayi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pl.nicolike.cn

[C09] 递归
来源：http://kh.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nz.hahajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fh.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qq.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://io.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yc.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pc.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nl.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lh.szsharing.cn

[C10] 变量作用域
来源：http://ol.shxzskj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://az.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fk.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ya.nszjky.cn

TS:   同 JS
来源：http://ro.lnxyls.cn

Java: 方法内为块级作用域
来源：http://lf.gzmigu.cn

Go:   花括号块级作用域
来源：http://op.yuexingan06.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ii.hahajie.cn

C#:   块级作用域
来源：http://yj.gzmigu.cn

[C11] 模块导入与导出
来源：http://hs.huixinmuqiang.cn

Py:   from module import func
来源：http://yz.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mk.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ay.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://uh.yuntaijiaju.cn

Java: import java.util.List;
来源：http://dh.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mi.shxzskj.cn

Ruby: require "json"; require_relative "./util"
来源：http://uk.nicolike.cn

C#:   using System.Text;
来源：http://ij.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://uh.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://pa.nszjky.cn

PHP:  (function () { echo "run"; })();
来源：http://ji.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://bh.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://tn.yuntaijiaju.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mn.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ug.haigaiapp.cn

Ruby: -> { puts "run" }.call
来源：http://ze.colortex.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mg.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://nj.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ik.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pi.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://au.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nh.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cj.huanxung.cn

Go:   func add(a, b int) int
来源：http://ix.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gc.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tz.yuexingan06.cn

[C14] 泛型函数
来源：http://zt.muxihuayi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fs.muxihuayi.cn

PHP:  // 无泛型
来源：http://ag.hnjuh.cn

JS:   // 无泛型
来源：http://rv.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yx.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vx.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zb.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://rg.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://py.hnjuh.cn

[C15] 解构 / 展开参数
来源：http://xy.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ev.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://up.shxzukj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gy.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zv.hahajie.cn

Java: // 无解构
来源：http://ms.newstarts.cn

Go:   // 无解构
来源：http://tx.colortex.cn

Ruby: a, b = pair
来源：http://re.nszjky.cn

C#:   var (a, b) = pair;
来源：http://gz.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://jv.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rt.colortex.cn

PHP:  // 无重载
来源：http://hq.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jf.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://sm.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cg.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://ck.jianghongdianzi.cn

Ruby: # 无重载：靠动态参数
来源：http://lj.wgjwhj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pi.jianghongdianzi.cn

================================================================================
来源：http://zt.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://bi.muxihuayi.cn

================================================================================
来源：http://ou.hahajie.cn

[D01] 创建数组 / 列表
来源：http://tl.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rq.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qt.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hk.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jz.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yn.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://uq.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://ah.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lf.colortex.cn

[D02] 追加元素到末尾
来源：http://mc.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ds.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xx.bjjhwx.cn

JS:   arr.push(4);
来源：http://ma.shtwfgs.cn

TS:   arr.push(4);
来源：http://cu.521024.cn

Java: list.add(4);
来源：http://jj.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://fv.szxytkj.cn

Ruby: arr << 4; arr.push(5)
来源：http://np.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://tn.hahajie.cn

[D03] 在指定位置插入元素
来源：http://zn.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://kn.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ph.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://um.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://gf.wgjwhj.cn

Java: list.add(0, 0);
来源：http://dl.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ru.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pi.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://my.szsharing.cn

[D04] 删除元素
来源：http://jr.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rj.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oc.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gz.521024.cn

TS:   arr.splice(0, 1);
来源：http://ow.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ly.szsharing.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qy.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hk.gzmigu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wc.huixiangedu.cn

[D05] 访问与修改元素
来源：http://wr.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fd.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ll.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://db.nszjky.cn

TS:   arr[0]; arr.at(-1);
来源：http://hx.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://ge.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://cd.jctech888.com.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gl.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dc.szsharing.cn

[D06] 数组长度
来源：http://ws.shxzukj.cn

Py:   len(arr)
来源：http://sp.huixiangedu.cn

PHP:  count($arr);
来源：http://hk.huixiangedu.cn

JS:   arr.length
来源：http://il.hahajie.cn

TS:   arr.length
来源：http://gm.shxzskj.cn

Java: list.size();
来源：http://rt.huanxung.cn

Go:   len(arr)
来源：http://wd.szsharing.cn

Ruby: arr.length; arr.size
来源：http://ai.szxytkj.cn

C#:   list.Count;
来源：http://ax.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://vp.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ke.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xx.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://zk.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://pf.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://ha.wgjwhj.cn

Go:   arr[1:4]
来源：http://va.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://hr.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://rp.9csxet.cn

[D08] 合并两个数组
来源：http://gi.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://xj.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://ac.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gn.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://qj.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wc.nicolike.cn

Go:   append(a, b...)
来源：http://bt.hnjuh.cn

Ruby: a + b;  a.concat(b)
来源：http://kp.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://oa.panjiajie.cn

[D09] 排序（升序）
来源：http://to.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://od.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://ut.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yv.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qv.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ub.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ux.shxzukj.cn

Ruby: arr.sort
来源：http://pz.yuntaijiaju.cn

C#:   list.Sort();
来源：http://fg.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ci.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qv.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wf.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vz.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ey.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oe.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://al.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hm.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gb.szxytkj.cn

[D11] 反转数组
来源：http://sy.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gp.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://np.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.colortex.cn

TS:   [...arr].reverse();
来源：http://bg.szsharing.cn

Java: Collections.reverse(list);
来源：http://vv.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://il.colortex.cn

Ruby: arr.reverse
来源：http://kx.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://te.asd995.cn

[D12] 查找元素下标
来源：http://hm.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://uz.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pp.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fs.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iv.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lr.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://jl.huanxung.cn

Ruby: arr.index(x)
来源：http://ev.9csxet.cn

C#:   list.IndexOf(x);
来源：http://fm.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://in.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jy.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ol.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://lh.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://yg.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jg.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oj.szxytkj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tj.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lj.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://qz.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ar.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sr.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://wk.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://tw.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bi.jianghongdianzi.cn

Go:   // 手写循环
来源：http://qt.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ed.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kf.lnxyls.cn

[D15] 去重
来源：http://xs.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bb.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://zv.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://hl.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://yu.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ne.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zt.bookmarksfly.cn

Ruby: arr.uniq
来源：http://dh.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://co.nicolike.cn

[D16] 求和与平均值
来源：http://ec.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lw.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://us.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pb.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vc.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qh.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://ed.szsharing.cn


<!-- 参考信息 -->