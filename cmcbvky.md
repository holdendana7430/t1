代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://cv.hnjuh.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qu.lnxyls.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tm.bjjhwx.cn

Ruby: def greet(name = "World") = name
来源：http://ak.bjjhwx.cn

C#:   string Greet(string name = "World") => name;
来源：http://pl.szxytkj.cn

[C03] 可变参数
来源：http://bm.lnxyls.cn

Py:   def total(*args): return sum(args)
来源：http://fc.yuntaijiaju.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ma.nicolike.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pi.panjiajie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jh.9csxet.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vv.hnjuh.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ij.newstarts.cn

Ruby: def total(*nums); nums.sum; end
来源：http://za.szsharing.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uh.szxytkj.cn

[C04] 命名参数 / 关键字参数
来源：http://so.hnjuh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://us.shxzukj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://le.9csxet.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fs.szxytkj.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mb.haigaiapp.cn

Java: // 无：用 Builder 模式或 record
来源：http://ah.newstarts.cn

Go:   // 无：用配置结构体参数
来源：http://fz.shtwfgs.cn

Ruby: f(a: 1, b: 2)
来源：http://yu.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://bf.9csxet.cn

[C05] 返回多个值
来源：http://kk.asd995.cn

Py:   return a, b
来源：http://bw.9csxet.cn

PHP:  return [$a, $b];
来源：http://dm.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ng.panjiajie.cn

TS:   return { a, b };
来源：http://al.9csxet.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://df.9csxet.cn

Go:   return a, b
来源：http://ey.bjjhwx.cn

Ruby: return a, b
来源：http://cc.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://cv.colortex.cn

[C06] 匿名函数 / lambda
来源：http://zc.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://au.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sr.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://rl.muxihuayi.cn

TS:   const square = (x: number): number => x * x;
来源：http://kb.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ud.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cc.colortex.cn

Ruby: square = ->(x) { x * x }
来源：http://pc.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nl.521024.cn

[C07] 把函数作为参数传入
来源：http://ju.jctech888.com.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://av.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ao.huixiangedu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://od.gzmigu.cn

TS:   arr.map(String)
来源：http://hf.shxzukj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iw.haigaiapp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://af.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://uv.colortex.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cq.haigaiapp.cn

[C08] 闭包
来源：http://kg.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fo.huixiangedu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zc.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oh.newstarts.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vc.shxzukj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ij.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://su.szxytkj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ll.szxytkj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tt.shtwfgs.cn

[C09] 递归
来源：http://um.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fv.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ep.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ol.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vn.colortex.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://et.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qb.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qx.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xd.muxihuayi.cn

[C10] 变量作用域
来源：http://vf.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rm.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://is.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xl.jianghongdianzi.cn

TS:   同 JS
来源：http://mu.szsharing.cn

Java: 方法内为块级作用域
来源：http://zf.muxihuayi.cn

Go:   花括号块级作用域
来源：http://sg.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bx.colortex.cn

C#:   块级作用域
来源：http://we.hahajie.cn

[C11] 模块导入与导出
来源：http://os.521024.cn

Py:   from module import func
来源：http://ls.muxihuayi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://dv.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vi.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oi.nszjky.cn

Java: import java.util.List;
来源：http://zt.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oi.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://cc.colortex.cn

C#:   using System.Text;
来源：http://bh.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://rm.huixinmuqiang.cn

Py:   (lambda: print("run"))()
来源：http://rz.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://bs.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://ph.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://eo.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pl.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://fj.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://uc.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gn.gzmigu.cn

[C13] 类型声明 / 类型注解
来源：http://iu.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wr.lnxyls.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://in.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://es.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rw.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mt.muxihuayi.cn

Go:   func add(a, b int) int
来源：http://pd.chemitech.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kn.hnjuh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zi.bjjhwx.cn

[C14] 泛型函数
来源：http://yx.szxytkj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qv.521024.cn

PHP:  // 无泛型
来源：http://kq.panjiajie.cn

JS:   // 无泛型
来源：http://hn.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zg.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ui.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ur.yuexingan06.cn

Ruby: # 无泛型
来源：http://ii.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ae.newstarts.cn

[C15] 解构 / 展开参数
来源：http://tm.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sq.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://lx.9csxet.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wl.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qs.yuexingan06.cn

Java: // 无解构
来源：http://td.haigaiapp.cn

Go:   // 无解构
来源：http://cu.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://ki.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://au.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://yi.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ga.huixinmuqiang.cn

PHP:  // 无重载
来源：http://sk.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://me.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://gn.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hh.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://jb.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://mi.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cl.hahajie.cn

================================================================================
来源：http://vt.szsharing.cn

D. 数组 / 列表 / 集合
来源：http://ze.nszjky.cn

================================================================================
来源：http://yq.asd995.cn

[D01] 创建数组 / 列表
来源：http://ah.yuntaijiaju.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wq.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vz.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bx.shxzskj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kq.newstarts.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ht.newstarts.cn

Go:   arr := []int{1, 2, 3}
来源：http://mb.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://yy.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qg.szsharing.cn

[D02] 追加元素到末尾
来源：http://rj.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iz.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hj.newstarts.cn

JS:   arr.push(4);
来源：http://yg.lnxyls.cn

TS:   arr.push(4);
来源：http://rn.szsharing.cn

Java: list.add(4);
来源：http://nm.szxytkj.cn

Go:   arr = append(arr, 4)
来源：http://cn.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://pr.shtwfgs.cn

C#:   list.Add(4);
来源：http://om.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://bk.colortex.cn

Py:   arr.insert(0, 0)
来源：http://bv.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kp.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ak.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://pb.bjjhwx.cn

Java: list.add(0, 0);
来源：http://eb.muxihuayi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gk.huixiangedu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sf.wgjwhj.cn

C#:   list.Insert(0, 0);
来源：http://ey.jianghongdianzi.cn

[D04] 删除元素
来源：http://wg.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fz.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ru.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xx.521024.cn

TS:   arr.splice(0, 1);
来源：http://fo.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ll.jianghongdianzi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qz.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wt.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://az.9csxet.cn

[D05] 访问与修改元素
来源：http://px.jianghongdianzi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hb.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sd.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xo.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://cb.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://un.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://wg.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qn.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ti.haigaiapp.cn

[D06] 数组长度
来源：http://qe.szsharing.cn

Py:   len(arr)
来源：http://xj.9csxet.cn

PHP:  count($arr);
来源：http://po.chemitech.net.cn

JS:   arr.length
来源：http://ew.hahajie.cn

TS:   arr.length
来源：http://py.bookmarksfly.cn

Java: list.size();
来源：http://qv.hnjuh.cn

Go:   len(arr)
来源：http://oe.hahajie.cn

Ruby: arr.length; arr.size
来源：http://tx.lnxyls.cn

C#:   list.Count;
来源：http://ho.szsharing.cn

[D07] 切片 / 取子数组
来源：http://gl.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pw.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://aa.szsharing.cn

JS:   arr.slice(1, 4);
来源：http://om.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://gx.shxzskj.cn

Java: list.subList(1, 4);
来源：http://tx.haigaiapp.cn

Go:   arr[1:4]
来源：http://bt.shxzukj.cn

Ruby: arr[1, 3]
来源：http://ln.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://if.bookmarksfly.cn

[D08] 合并两个数组
来源：http://wu.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://nh.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://wv.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fq.newstarts.cn

TS:   [...a, ...b];
来源：http://pu.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ql.nicolike.cn

Go:   append(a, b...)
来源：http://qh.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://pg.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://ev.shxzukj.cn

[D09] 排序（升序）
来源：http://lr.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://dm.szsharing.cn

PHP:  sort($arr);
来源：http://jv.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jy.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kt.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yp.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://se.yuexingan06.cn

Ruby: arr.sort
来源：http://al.521024.cn

C#:   list.Sort();
来源：http://bj.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://su.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gb.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ws.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pr.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lw.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ng.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xe.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qa.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bd.newstarts.cn

[D11] 反转数组
来源：http://kh.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rv.colortex.cn

PHP:  array_reverse($arr);
来源：http://jq.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gv.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://qm.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://vt.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://ui.muxihuayi.cn

Ruby: arr.reverse
来源：http://lg.yuexingan06.cn

C#:   list.Reverse();
来源：http://od.nszjky.cn

[D12] 查找元素下标
来源：http://md.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://wv.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://do.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wd.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://je.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://na.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://yn.bjjhwx.cn

Ruby: arr.index(x)
来源：http://ck.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://hy.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://xv.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jm.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xy.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://zq.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://ay.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zo.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zt.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ky.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vz.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://wm.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rx.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fr.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://nu.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://zt.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ku.szsharing.cn

Go:   // 手写循环
来源：http://vp.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tw.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ej.shxzskj.cn

[D15] 去重
来源：http://oq.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oq.shxzskj.cn

PHP:  array_unique($arr);
来源：http://hz.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://vn.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://uh.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gn.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yy.huanxung.cn

Ruby: arr.uniq
来源：http://kz.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://yb.hnjuh.cn

[D16] 求和与平均值
来源：http://vp.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fv.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ca.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rm.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sb.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bh.521024.cn

Go:   // 手写循环累加
来源：http://nq.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rh.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://ar.jctech888.com.cn

[D17] 最大值与最小值
来源：http://bi.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://mw.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://aa.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ue.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://zt.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fa.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tr.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://nz.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://bv.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://gs.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eq.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://dq.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bf.hahajie.cn

TS:   nested.flat();
来源：http://zf.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mv.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://rq.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://gh.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ep.panjiajie.cn

[D19] 按字段分组
来源：http://xd.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eo.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ek.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hy.colortex.cn


<!-- 参考信息 -->