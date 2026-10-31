代发 wailian999

Py:   def add(a, b): return a + b
来源：http://le.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zp.huixinmuqiang.cn

JS:   function add(a, b) { return a + b; }
来源：http://xj.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ya.huixinmuqiang.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hb.panjiajie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://he.chemitech.net.cn

Ruby: def add(a, b); a + b; end
来源：http://qj.bookmarksfly.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xw.huixiangedu.cn

[C02] 默认参数
来源：http://vn.yuntaijiaju.cn

Py:   def greet(name="World"): return name
来源：http://cy.521024.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ch.bjjhwx.cn

JS:   function greet(name = "World") { return name; }
来源：http://yf.muxihuayi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ds.shtwfgs.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://em.nicolike.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mz.panjiajie.cn

Ruby: def greet(name = "World") = name
来源：http://tg.muxihuayi.cn

C#:   string Greet(string name = "World") => name;
来源：http://jq.huixinmuqiang.cn

[C03] 可变参数
来源：http://mh.gzmigu.cn

Py:   def total(*args): return sum(args)
来源：http://ni.gzmigu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wt.gzmigu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mh.huixiangedu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xe.muxihuayi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fm.haigaiapp.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ej.asd995.cn

Ruby: def total(*nums); nums.sum; end
来源：http://zr.huixinmuqiang.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zi.huanxung.cn

[C04] 命名参数 / 关键字参数
来源：http://xt.shxzukj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pw.colortex.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bz.szxytkj.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fr.521024.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qg.szsharing.cn

Java: // 无：用 Builder 模式或 record
来源：http://hv.nicolike.cn

Go:   // 无：用配置结构体参数
来源：http://lz.colortex.cn

Ruby: f(a: 1, b: 2)
来源：http://yj.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://oh.panjiajie.cn

[C05] 返回多个值
来源：http://rj.hahajie.cn

Py:   return a, b
来源：http://oj.gzmigu.cn

PHP:  return [$a, $b];
来源：http://bb.nszjky.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sr.nszjky.cn

TS:   return { a, b };
来源：http://mz.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wq.bookmarksfly.cn

Go:   return a, b
来源：http://lg.yuntaijiaju.cn

Ruby: return a, b
来源：http://ny.szsharing.cn

C#:   return (a, b);              // ValueTuple
来源：http://jv.jianghongdianzi.cn

[C06] 匿名函数 / lambda
来源：http://iz.chemitech.net.cn

Py:   square = lambda x: x * x
来源：http://cy.shxzukj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dg.jctech888.com.cn

JS:   const square = x => x * x;
来源：http://vy.haigaiapp.cn

TS:   const square = (x: number): number => x * x;
来源：http://py.huixiangedu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jx.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pq.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://ha.9csxet.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bz.nicolike.cn

[C07] 把函数作为参数传入
来源：http://cs.yuntaijiaju.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lv.panjiajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://oj.huanxung.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wk.shxzukj.cn

TS:   arr.map(String)
来源：http://kh.chemitech.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ap.shxzskj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kx.wgjwhj.cn

Ruby: arr.map(&:upcase)
来源：http://ly.shxzukj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pg.shxzskj.cn

[C08] 闭包
来源：http://hy.huanxung.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lw.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nm.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vn.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wb.bjjhwx.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ub.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ao.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ku.yuntaijiaju.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iu.huixinmuqiang.cn

[C09] 递归
来源：http://hc.colortex.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://so.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sl.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://po.yuntaijiaju.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kb.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://os.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oq.bookmarksfly.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://us.huixinmuqiang.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ag.yuexingan06.cn

[C10] 变量作用域
来源：http://dg.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rd.jctech888.com.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yc.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://il.huixinmuqiang.cn

TS:   同 JS
来源：http://mz.shtwfgs.cn

Java: 方法内为块级作用域
来源：http://bk.huixiangedu.cn

Go:   花括号块级作用域
来源：http://wl.asd995.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ak.jianghongdianzi.cn

C#:   块级作用域
来源：http://ii.muxihuayi.cn

[C11] 模块导入与导出
来源：http://gg.szxytkj.cn

Py:   from module import func
来源：http://nc.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wt.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wr.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ut.huixiangedu.cn

Java: import java.util.List;
来源：http://jo.yuntaijiaju.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://of.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://fk.bookmarksfly.cn

C#:   using System.Text;
来源：http://qo.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://vk.newstarts.cn

Py:   (lambda: print("run"))()
来源：http://oq.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://sh.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://ap.yuexingan06.cn

TS:   (() => { console.log("run"); })();
来源：http://uf.panjiajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ts.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://sv.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://hi.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fh.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://zl.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pp.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xd.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vn.yuntaijiaju.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nd.jctech888.com.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ar.nicolike.cn

Go:   func add(a, b int) int
来源：http://zy.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tk.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ff.lnxyls.cn

[C14] 泛型函数
来源：http://jb.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hc.panjiajie.cn

PHP:  // 无泛型
来源：http://on.chemitech.net.cn

JS:   // 无泛型
来源：http://ai.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eh.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://df.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dc.nszjky.cn

Ruby: # 无泛型
来源：http://xg.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fi.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://sc.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://et.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://pg.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://il.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dd.lnxyls.cn

Java: // 无解构
来源：http://uh.huixiangedu.cn

Go:   // 无解构
来源：http://lm.9csxet.cn

Ruby: a, b = pair
来源：http://ij.haigaiapp.cn

C#:   var (a, b) = pair;
来源：http://au.huixinmuqiang.cn

[C16] 函数 / 方法重载
来源：http://kf.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hp.bookmarksfly.cn

PHP:  // 无重载
来源：http://ia.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kt.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://jd.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tv.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://ye.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://jw.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rw.lnxyls.cn

================================================================================
来源：http://ed.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://db.huixiangedu.cn

================================================================================
来源：http://dq.asd995.cn

[D01] 创建数组 / 列表
来源：http://qo.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bw.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xs.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lg.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bj.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ax.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://oz.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://kx.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yi.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://db.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bw.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pl.9csxet.cn

JS:   arr.push(4);
来源：http://fv.hahajie.cn

TS:   arr.push(4);
来源：http://xg.huixinmuqiang.cn

Java: list.add(4);
来源：http://bu.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://it.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://fn.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://qh.shxzukj.cn

[D03] 在指定位置插入元素
来源：http://cy.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://qs.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wg.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pn.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://gg.chemitech.net.cn

Java: list.add(0, 0);
来源：http://ql.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://je.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ri.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ui.nszjky.cn

[D04] 删除元素
来源：http://ol.muxihuayi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qd.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qq.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lt.gzmigu.cn

TS:   arr.splice(0, 1);
来源：http://xl.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vo.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zq.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rm.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lx.9csxet.cn

[D05] 访问与修改元素
来源：http://az.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bd.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hd.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pg.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://rn.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://wq.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://uo.szxytkj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ul.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fn.jctech888.com.cn

[D06] 数组长度
来源：http://hc.shxzskj.cn

Py:   len(arr)
来源：http://gm.shxzukj.cn

PHP:  count($arr);
来源：http://sh.521024.cn

JS:   arr.length
来源：http://lt.nszjky.cn

TS:   arr.length
来源：http://ib.shxzskj.cn

Java: list.size();
来源：http://tu.lnxyls.cn

Go:   len(arr)
来源：http://mq.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://oq.huixinmuqiang.cn

C#:   list.Count;
来源：http://fp.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://dt.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dn.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jx.yuntaijiaju.cn

JS:   arr.slice(1, 4);
来源：http://kd.colortex.cn

TS:   arr.slice(1, 4);
来源：http://pt.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://le.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://yc.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://mc.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://yd.panjiajie.cn

[D08] 合并两个数组
来源：http://nq.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://qy.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://rz.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://et.hnjuh.cn

TS:   [...a, ...b];
来源：http://az.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kf.szxytkj.cn

Go:   append(a, b...)
来源：http://fa.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://ka.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://gr.gzmigu.cn

[D09] 排序（升序）
来源：http://nr.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vh.chemitech.net.cn

PHP:  sort($arr);
来源：http://uk.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uh.yuntaijiaju.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nr.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iu.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ll.panjiajie.cn

Ruby: arr.sort
来源：http://yw.shxzukj.cn

C#:   list.Sort();
来源：http://ww.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jo.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ni.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lp.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://di.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bx.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://es.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fr.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vh.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xg.wgjwhj.cn

[D11] 反转数组
来源：http://oo.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zt.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://zb.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vr.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://zm.asd995.cn

Java: Collections.reverse(list);
来源：http://at.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://mz.chemitech.net.cn

Ruby: arr.reverse
来源：http://bs.huanxung.cn

C#:   list.Reverse();
来源：http://ub.bookmarksfly.cn

[D12] 查找元素下标
来源：http://lr.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://it.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vm.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fv.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vz.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vp.asd995.cn

Go:   slices.Index(arr, x)
来源：http://aj.yuexingan06.cn

Ruby: arr.index(x)
来源：http://ah.huanxung.cn

C#:   list.IndexOf(x);
来源：http://hn.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://mt.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bz.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ux.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://ne.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://xi.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sv.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jn.nszjky.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xx.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xs.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://fi.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://el.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zp.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://sw.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://cp.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hu.haigaiapp.cn

Go:   // 手写循环
来源：http://qt.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mh.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qo.szxytkj.cn

[D15] 去重
来源：http://sp.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dz.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://ff.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://ej.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://ku.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kq.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pm.jctech888.com.cn

Ruby: arr.uniq
来源：http://hh.colortex.cn

C#:   list.Distinct().ToList()
来源：http://yz.shxzukj.cn

[D16] 求和与平均值
来源：http://mo.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gf.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kw.chemitech.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pa.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ot.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sk.asd995.cn

Go:   // 手写循环累加
来源：http://hu.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qt.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://he.bjjhwx.cn

[D17] 最大值与最小值
来源：http://yh.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://xq.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://pv.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hahajie.cn

TS:   Math.max(...arr);
来源：http://fx.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kr.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kz.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://dh.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://qx.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://lb.huixinmuqiang.cn


<!-- 参考信息 -->