代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wy.9csxet.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oq.huixinmuqiang.cn

Ruby: def add(a, b); a + b; end
来源：http://hy.shtwfgs.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wn.jianghongdianzi.cn

[C02] 默认参数
来源：http://fw.hahajie.cn

Py:   def greet(name="World"): return name
来源：http://uj.haigaiapp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bs.shxzskj.cn

JS:   function greet(name = "World") { return name; }
来源：http://qc.nicolike.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wq.hahajie.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oo.huanxung.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fy.shxzskj.cn

Ruby: def greet(name = "World") = name
来源：http://az.bookmarksfly.cn

C#:   string Greet(string name = "World") => name;
来源：http://mx.bookmarksfly.cn

[C03] 可变参数
来源：http://ru.9csxet.cn

Py:   def total(*args): return sum(args)
来源：http://tu.panjiajie.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://au.yuntaijiaju.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ea.nicolike.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rr.hahajie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://js.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ra.wgjwhj.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pc.haigaiapp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://db.521024.cn

[C04] 命名参数 / 关键字参数
来源：http://tf.huanxung.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bm.huixinmuqiang.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wf.huixinmuqiang.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://le.shxzskj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xv.huanxung.cn

Java: // 无：用 Builder 模式或 record
来源：http://in.muxihuayi.cn

Go:   // 无：用配置结构体参数
来源：http://id.shxzskj.cn

Ruby: f(a: 1, b: 2)
来源：http://uz.yuntaijiaju.cn

C#:   f(a: 1, b: 2)
来源：http://jo.huanxung.cn

[C05] 返回多个值
来源：http://zr.chemitech.net.cn

Py:   return a, b
来源：http://qs.shxzukj.cn

PHP:  return [$a, $b];
来源：http://wo.huixinmuqiang.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pu.hahajie.cn

TS:   return { a, b };
来源：http://uo.gzmigu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fi.bjjhwx.cn

Go:   return a, b
来源：http://px.gzmigu.cn

Ruby: return a, b
来源：http://my.jianghongdianzi.cn

C#:   return (a, b);              // ValueTuple
来源：http://yv.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://tb.huanxung.cn

Py:   square = lambda x: x * x
来源：http://ts.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yf.shxzskj.cn

JS:   const square = x => x * x;
来源：http://iy.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://tp.huixinmuqiang.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mq.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rm.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://fj.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ha.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://kx.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ec.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zg.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vf.huixiangedu.cn

TS:   arr.map(String)
来源：http://gl.hahajie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cn.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sf.shtwfgs.cn

Ruby: arr.map(&:upcase)
来源：http://lh.bookmarksfly.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vk.huixinmuqiang.cn

[C08] 闭包
来源：http://gc.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ce.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ib.521024.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gk.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vr.muxihuayi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iy.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qb.huixinmuqiang.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oy.bookmarksfly.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fc.521024.cn

[C09] 递归
来源：http://vy.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xp.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kc.bookmarksfly.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://co.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xk.newstarts.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vt.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ue.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jq.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pd.huixinmuqiang.cn

[C10] 变量作用域
来源：http://td.szsharing.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wm.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kc.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://db.nszjky.cn

TS:   同 JS
来源：http://km.nicolike.cn

Java: 方法内为块级作用域
来源：http://lh.hahajie.cn

Go:   花括号块级作用域
来源：http://yj.shxzukj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oh.jctech888.com.cn

C#:   块级作用域
来源：http://pe.wgjwhj.cn

[C11] 模块导入与导出
来源：http://tc.haigaiapp.cn

Py:   from module import func
来源：http://bj.asd995.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yk.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://kr.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dg.521024.cn

Java: import java.util.List;
来源：http://my.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://an.hahajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://dh.wgjwhj.cn

C#:   using System.Text;
来源：http://st.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://uf.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ht.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://ev.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://bg.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://xb.huixiangedu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rd.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://lf.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://fr.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ae.bookmarksfly.cn

[C13] 类型声明 / 类型注解
来源：http://np.huixiangedu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vy.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xi.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dj.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bi.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uz.hnjuh.cn

Go:   func add(a, b int) int
来源：http://ni.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://du.nicolike.cn

C#:   int Add(int a, int b) => a + b;
来源：http://iu.muxihuayi.cn

[C14] 泛型函数
来源：http://bx.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hi.yuexingan06.cn

PHP:  // 无泛型
来源：http://oe.chemitech.net.cn

JS:   // 无泛型
来源：http://xd.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pk.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pp.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://my.gzmigu.cn

Ruby: # 无泛型
来源：http://cc.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://io.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://lt.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vq.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://ux.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ow.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mr.muxihuayi.cn

Java: // 无解构
来源：http://sx.szxytkj.cn

Go:   // 无解构
来源：http://wo.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://qc.hahajie.cn

C#:   var (a, b) = pair;
来源：http://ye.nicolike.cn

[C16] 函数 / 方法重载
来源：http://bh.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://de.szsharing.cn

PHP:  // 无重载
来源：http://zz.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cg.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://ck.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gf.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://vt.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://hd.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uj.haigaiapp.cn

================================================================================
来源：http://dw.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://vs.jctech888.com.cn

================================================================================
来源：http://td.haigaiapp.cn

[D01] 创建数组 / 列表
来源：http://yi.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hi.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xx.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rc.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mp.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zf.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://mf.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://ox.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xx.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://pe.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kg.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ki.jctech888.com.cn

JS:   arr.push(4);
来源：http://yq.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://mm.yuntaijiaju.cn

Java: list.add(4);
来源：http://kh.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://zg.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://tt.muxihuayi.cn

C#:   list.Add(4);
来源：http://iy.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ek.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://jg.shxzukj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://va.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mk.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://zr.nicolike.cn

Java: list.add(0, 0);
来源：http://xu.wgjwhj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gz.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://we.521024.cn

C#:   list.Insert(0, 0);
来源：http://oj.hahajie.cn

[D04] 删除元素
来源：http://fu.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fc.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nn.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ck.521024.cn

TS:   arr.splice(0, 1);
来源：http://ov.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ry.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gs.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://la.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ac.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://wy.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lb.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nq.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ld.jianghongdianzi.cn

TS:   arr[0]; arr.at(-1);
来源：http://mz.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://wl.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://wn.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jf.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dq.yuntaijiaju.cn

[D06] 数组长度
来源：http://lu.panjiajie.cn

Py:   len(arr)
来源：http://gk.hnjuh.cn

PHP:  count($arr);
来源：http://uw.huanxung.cn

JS:   arr.length
来源：http://oh.lnxyls.cn

TS:   arr.length
来源：http://fm.haigaiapp.cn

Java: list.size();
来源：http://il.huanxung.cn

Go:   len(arr)
来源：http://kt.szsharing.cn

Ruby: arr.length; arr.size
来源：http://av.wgjwhj.cn

C#:   list.Count;
来源：http://fx.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://mp.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wa.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zc.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://mc.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://kv.shxzukj.cn

Java: list.subList(1, 4);
来源：http://kp.9csxet.cn

Go:   arr[1:4]
来源：http://ut.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://zk.colortex.cn

C#:   list.GetRange(1, 3);
来源：http://wq.521024.cn

[D08] 合并两个数组
来源：http://iy.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://kq.colortex.cn

PHP:  array_merge($a, $b);
来源：http://td.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bu.nszjky.cn

TS:   [...a, ...b];
来源：http://su.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ry.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://ht.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://ie.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://nq.hahajie.cn

[D09] 排序（升序）
来源：http://rs.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://as.gzmigu.cn

PHP:  sort($arr);
来源：http://zr.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kp.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://na.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://og.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pm.colortex.cn

Ruby: arr.sort
来源：http://vp.huixinmuqiang.cn

C#:   list.Sort();
来源：http://kw.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cq.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jx.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://us.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bf.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fp.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rt.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://up.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ba.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jd.jianghongdianzi.cn

[D11] 反转数组
来源：http://py.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ro.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://mc.hnjuh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ct.hnjuh.cn

TS:   [...arr].reverse();
来源：http://iq.colortex.cn

Java: Collections.reverse(list);
来源：http://wi.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://qz.jianghongdianzi.cn

Ruby: arr.reverse
来源：http://ce.chemitech.net.cn

C#:   list.Reverse();
来源：http://mo.szxytkj.cn

[D12] 查找元素下标
来源：http://eh.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://ey.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iz.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://el.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://at.shxzukj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cs.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://sk.nicolike.cn

Ruby: arr.index(x)
来源：http://ku.nszjky.cn

C#:   list.IndexOf(x);
来源：http://tk.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ul.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oz.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zm.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://ja.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://jy.yuexingan06.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tu.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wx.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vl.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lh.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://xh.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://we.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://su.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://kp.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://tu.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://it.wgjwhj.cn

Go:   // 手写循环
来源：http://fa.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hu.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rw.lnxyls.cn

[D15] 去重
来源：http://ys.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uz.panjiajie.cn

PHP:  array_unique($arr);
来源：http://ft.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://ed.huixinmuqiang.cn

TS:   [...new Set(arr)]
来源：http://xe.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sg.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ph.haigaiapp.cn

Ruby: arr.uniq
来源：http://ft.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://mx.chemitech.net.cn

[D16] 求和与平均值
来源：http://po.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qr.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yo.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xi.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wi.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tc.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://pn.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xx.521024.cn

C#:   list.Sum();  list.Average()
来源：http://vz.colortex.cn

[D17] 最大值与最小值
来源：http://ij.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://lp.nicolike.cn

PHP:  max($arr);  min($arr);
来源：http://yn.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hp.hahajie.cn

TS:   Math.max(...arr);
来源：http://gv.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jh.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sp.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://ei.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://dw.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://ek.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dv.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://gr.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ip.bjjhwx.cn

TS:   nested.flat();
来源：http://sb.haigaiapp.cn


<!-- 参考信息 -->