代发 wailian999

Java: if (data == null) return;
来源：http://my.huixiangedu.cn

Go:   if data == nil { return }
来源：http://hf.chemitech.net.cn

Ruby: return if data.nil?
来源：http://fh.chemitech.net.cn

C#:   if (data == null) return;
来源：http://ng.hahajie.cn

================================================================================
来源：http://wk.huanxung.cn

C. 函数与作用域
来源：http://ix.newstarts.cn

================================================================================
来源：http://bb.chemitech.net.cn

[C01] 定义函数
来源：http://di.shxzskj.cn

Py:   def add(a, b): return a + b
来源：http://rd.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kc.shtwfgs.cn

JS:   function add(a, b) { return a + b; }
来源：http://bq.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gx.muxihuayi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://kh.wgjwhj.cn

Go:   func add(a, b int) int { return a + b }
来源：http://mq.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://rr.bjjhwx.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://un.nszjky.cn

[C02] 默认参数
来源：http://um.szxytkj.cn

Py:   def greet(name="World"): return name
来源：http://eq.shxzskj.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fp.newstarts.cn

JS:   function greet(name = "World") { return name; }
来源：http://yk.521024.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eh.lnxyls.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://az.panjiajie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://be.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://ia.panjiajie.cn

C#:   string Greet(string name = "World") => name;
来源：http://tg.jctech888.com.cn

[C03] 可变参数
来源：http://mp.jctech888.com.cn

Py:   def total(*args): return sum(args)
来源：http://ag.shxzskj.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ug.shxzukj.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ap.haigaiapp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lr.nicolike.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zk.9csxet.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ld.gzmigu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jr.gzmigu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cm.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://vg.shtwfgs.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hl.jctech888.com.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hy.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pi.shtwfgs.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rp.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://lr.9csxet.cn

Go:   // 无：用配置结构体参数
来源：http://px.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://fd.hnjuh.cn

C#:   f(a: 1, b: 2)
来源：http://sw.muxihuayi.cn

[C05] 返回多个值
来源：http://qd.huixinmuqiang.cn

Py:   return a, b
来源：http://kh.panjiajie.cn

PHP:  return [$a, $b];
来源：http://zp.gzmigu.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jp.shxzukj.cn

TS:   return { a, b };
来源：http://oc.chemitech.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ib.lnxyls.cn

Go:   return a, b
来源：http://iw.lnxyls.cn

Ruby: return a, b
来源：http://ju.nszjky.cn

C#:   return (a, b);              // ValueTuple
来源：http://wr.shxzskj.cn

[C06] 匿名函数 / lambda
来源：http://kp.jianghongdianzi.cn

Py:   square = lambda x: x * x
来源：http://rn.colortex.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yw.hnjuh.cn

JS:   const square = x => x * x;
来源：http://ai.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://wx.szxytkj.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yf.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ly.chemitech.net.cn

Ruby: square = ->(x) { x * x }
来源：http://wp.szxytkj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zk.hahajie.cn

[C07] 把函数作为参数传入
来源：http://zb.haigaiapp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ab.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://by.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xj.hnjuh.cn

TS:   arr.map(String)
来源：http://rp.szsharing.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vl.asd995.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ps.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://ra.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://vx.muxihuayi.cn

[C08] 闭包
来源：http://fp.hnjuh.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qg.521024.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hs.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wm.shxzukj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://il.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kl.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hf.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ft.shtwfgs.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ch.szsharing.cn

[C09] 递归
来源：http://be.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://uo.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nq.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mm.bookmarksfly.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mw.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kq.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wb.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ov.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zh.szxytkj.cn

[C10] 变量作用域
来源：http://we.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yz.yuexingan06.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://md.wgjwhj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://iv.9csxet.cn

TS:   同 JS
来源：http://lh.chemitech.net.cn

Java: 方法内为块级作用域
来源：http://tq.muxihuayi.cn

Go:   花括号块级作用域
来源：http://dx.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nv.panjiajie.cn

C#:   块级作用域
来源：http://hq.colortex.cn

[C11] 模块导入与导出
来源：http://ti.szsharing.cn

Py:   from module import func
来源：http://bv.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nz.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tg.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jq.colortex.cn

Java: import java.util.List;
来源：http://nx.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://om.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://rh.shxzukj.cn

C#:   using System.Text;
来源：http://if.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://pn.yuexingan06.cn

Py:   (lambda: print("run"))()
来源：http://kg.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://fb.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://cl.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://uu.chemitech.net.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dn.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://is.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://ou.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vj.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://xa.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lv.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gl.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gw.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zy.shxzskj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yu.hnjuh.cn

Go:   func add(a, b int) int
来源：http://jg.nicolike.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dv.gzmigu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pk.chemitech.net.cn

[C14] 泛型函数
来源：http://ro.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nx.yuexingan06.cn

PHP:  // 无泛型
来源：http://du.asd995.cn

JS:   // 无泛型
来源：http://dy.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pf.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ie.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sd.huanxung.cn

Ruby: # 无泛型
来源：http://rj.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aq.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://hn.lnxyls.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://do.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://qw.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://km.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ne.yuntaijiaju.cn

Java: // 无解构
来源：http://zg.hnjuh.cn

Go:   // 无解构
来源：http://zx.asd995.cn

Ruby: a, b = pair
来源：http://hz.huixinmuqiang.cn

C#:   var (a, b) = pair;
来源：http://cf.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://za.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sv.huixiangedu.cn

PHP:  // 无重载
来源：http://lw.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gk.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://lg.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sl.shxzskj.cn

Go:   // 无重载：用不同函数名
来源：http://dr.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://yc.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cb.nszjky.cn

================================================================================
来源：http://wq.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://ws.szsharing.cn

================================================================================
来源：http://we.newstarts.cn

[D01] 创建数组 / 列表
来源：http://dd.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nt.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ca.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rl.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pv.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fn.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://le.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://sa.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cf.chemitech.net.cn

[D02] 追加元素到末尾
来源：http://ig.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fj.szxytkj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://an.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://ra.shxzukj.cn

TS:   arr.push(4);
来源：http://ku.chemitech.net.cn

Java: list.add(4);
来源：http://iv.huixiangedu.cn

Go:   arr = append(arr, 4)
来源：http://qh.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://zw.shxzukj.cn

C#:   list.Add(4);
来源：http://bv.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://jk.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://pt.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://is.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://us.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://rj.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://jn.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fi.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ow.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ok.jctech888.com.cn

[D04] 删除元素
来源：http://iu.szxytkj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kb.lnxyls.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sm.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ei.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://la.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rv.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zw.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zi.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xg.shtwfgs.cn

[D05] 访问与修改元素
来源：http://cx.hahajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iy.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ao.nszjky.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pi.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://ir.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://yf.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://vx.gzmigu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pm.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bb.gzmigu.cn

[D06] 数组长度
来源：http://hj.chemitech.net.cn

Py:   len(arr)
来源：http://oy.bjjhwx.cn

PHP:  count($arr);
来源：http://zu.newstarts.cn

JS:   arr.length
来源：http://xy.bookmarksfly.cn

TS:   arr.length
来源：http://tg.wgjwhj.cn

Java: list.size();
来源：http://di.9csxet.cn

Go:   len(arr)
来源：http://rw.huanxung.cn

Ruby: arr.length; arr.size
来源：http://zw.asd995.cn

C#:   list.Count;
来源：http://pq.asd995.cn

[D07] 切片 / 取子数组
来源：http://ex.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uc.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sa.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://rc.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://uj.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://zw.shtwfgs.cn

Go:   arr[1:4]
来源：http://ka.shxzskj.cn

Ruby: arr[1, 3]
来源：http://ma.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://ht.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://qk.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://nh.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://uo.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://by.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://ur.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vx.chemitech.net.cn

Go:   append(a, b...)
来源：http://ll.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://vv.521024.cn

C#:   a.Concat(b).ToList()
来源：http://jg.521024.cn

[D09] 排序（升序）
来源：http://dn.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://fr.521024.cn

PHP:  sort($arr);
来源：http://gj.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dl.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hn.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bu.jianghongdianzi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zt.colortex.cn

Ruby: arr.sort
来源：http://pv.muxihuayi.cn

C#:   list.Sort();
来源：http://ga.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ni.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jz.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://th.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sj.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yc.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wz.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pg.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nq.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cb.shxzukj.cn

[D11] 反转数组
来源：http://al.szxytkj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hj.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://jb.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tn.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://qi.szxytkj.cn

Java: Collections.reverse(list);
来源：http://nz.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://ge.bjjhwx.cn

Ruby: arr.reverse
来源：http://sp.nicolike.cn

C#:   list.Reverse();
来源：http://cx.haigaiapp.cn

[D12] 查找元素下标
来源：http://vu.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://ew.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sf.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xq.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sa.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zr.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://ro.bjjhwx.cn

Ruby: arr.index(x)
来源：http://qn.asd995.cn

C#:   list.IndexOf(x);
来源：http://hi.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://hz.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aa.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cb.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ci.colortex.cn

TS:   arr.filter(x => x > 3)
来源：http://ud.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rr.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://io.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://am.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://px.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://zo.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://th.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iq.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://aq.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://ip.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yk.huixinmuqiang.cn

Go:   // 手写循环
来源：http://lu.hahajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uf.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oi.shxzukj.cn

[D15] 去重
来源：http://gu.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gg.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://pg.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://eb.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://zx.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hb.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rr.asd995.cn

Ruby: arr.uniq
来源：http://ax.colortex.cn

C#:   list.Distinct().ToList()
来源：http://in.jctech888.com.cn

[D16] 求和与平均值
来源：http://oe.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wo.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pm.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jy.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jh.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lx.huanxung.cn

Go:   // 手写循环累加
来源：http://zt.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ak.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://nr.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://zg.jctech888.com.cn

Py:   max(arr);  min(arr)
来源：http://bo.panjiajie.cn


<!-- 参考信息 -->