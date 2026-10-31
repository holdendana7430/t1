代发 wailian999

Py:   return a, b
来源：http://xs.szxytkj.cn

PHP:  return [$a, $b];
来源：http://si.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://io.shxzskj.cn

TS:   return { a, b };
来源：http://df.shxzukj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wv.huanxung.cn

Go:   return a, b
来源：http://wp.bjjhwx.cn

Ruby: return a, b
来源：http://rx.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://mu.bookmarksfly.cn

[C06] 匿名函数 / lambda
来源：http://qu.521024.cn

Py:   square = lambda x: x * x
来源：http://io.shxzskj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rj.shxzukj.cn

JS:   const square = x => x * x;
来源：http://ly.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://ly.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ip.chemitech.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bz.szxytkj.cn

Ruby: square = ->(x) { x * x }
来源：http://fj.hnjuh.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mv.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://qk.colortex.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sd.asd995.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xm.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://np.shxzskj.cn

TS:   arr.map(String)
来源：http://kb.yuntaijiaju.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fj.nszjky.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qj.yuexingan06.cn

Ruby: arr.map(&:upcase)
来源：http://jl.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uz.yuntaijiaju.cn

[C08] 闭包
来源：http://ya.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fs.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wl.shxzukj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wd.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cc.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fz.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vu.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oe.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ge.bjjhwx.cn

[C09] 递归
来源：http://mx.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wg.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eh.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://za.yuexingan06.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fj.haigaiapp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xp.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bw.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ek.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://do.jctech888.com.cn

[C10] 变量作用域
来源：http://ow.huixinmuqiang.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fl.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xw.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://js.9csxet.cn

TS:   同 JS
来源：http://rl.huixiangedu.cn

Java: 方法内为块级作用域
来源：http://fc.shxzukj.cn

Go:   花括号块级作用域
来源：http://dw.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lm.shxzskj.cn

C#:   块级作用域
来源：http://mj.bjjhwx.cn

[C11] 模块导入与导出
来源：http://bc.newstarts.cn

Py:   from module import func
来源：http://ev.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://su.hahajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vn.gzmigu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lg.gzmigu.cn

Java: import java.util.List;
来源：http://oa.colortex.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vn.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://us.bjjhwx.cn

C#:   using System.Text;
来源：http://dx.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://wo.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://og.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://np.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://yo.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://bj.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pw.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://vs.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://pv.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ia.huixiangedu.cn

[C13] 类型声明 / 类型注解
来源：http://gb.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wq.huixiangedu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://je.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ue.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mb.bjjhwx.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pj.hnjuh.cn

Go:   func add(a, b int) int
来源：http://jv.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lo.hahajie.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ri.jianghongdianzi.cn

[C14] 泛型函数
来源：http://rk.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bd.wgjwhj.cn

PHP:  // 无泛型
来源：http://pk.yuntaijiaju.cn

JS:   // 无泛型
来源：http://gw.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ao.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pm.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kr.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://do.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tb.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://ib.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zt.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://eq.huanxung.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sy.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sc.wgjwhj.cn

Java: // 无解构
来源：http://pa.jianghongdianzi.cn

Go:   // 无解构
来源：http://pi.huixiangedu.cn

Ruby: a, b = pair
来源：http://de.shxzukj.cn

C#:   var (a, b) = pair;
来源：http://yf.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://hw.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qg.huixiangedu.cn

PHP:  // 无重载
来源：http://yo.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cf.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://rq.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mb.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://pm.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://fr.shxzskj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gp.nszjky.cn

================================================================================
来源：http://wp.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://tn.hahajie.cn

================================================================================
来源：http://uf.521024.cn

[D01] 创建数组 / 列表
来源：http://uq.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gx.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sj.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xd.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yd.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yv.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://uv.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://wz.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://py.colortex.cn

[D02] 追加元素到末尾
来源：http://vn.hahajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://te.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zw.gzmigu.cn

JS:   arr.push(4);
来源：http://iw.colortex.cn

TS:   arr.push(4);
来源：http://fk.panjiajie.cn

Java: list.add(4);
来源：http://zm.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://mv.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://mg.yuexingan06.cn

C#:   list.Add(4);
来源：http://ny.newstarts.cn

[D03] 在指定位置插入元素
来源：http://ds.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://jo.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yo.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://id.shtwfgs.cn

TS:   arr.splice(0, 0, 0);
来源：http://ds.nszjky.cn

Java: list.add(0, 0);
来源：http://az.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vu.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mk.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://uf.hnjuh.cn

[D04] 删除元素
来源：http://ty.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ct.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ts.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pi.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://jz.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gm.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yb.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jb.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bb.gzmigu.cn

[D05] 访问与修改元素
来源：http://ds.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://am.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cr.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jb.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://db.panjiajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://bn.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://wi.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vj.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ud.nicolike.cn

[D06] 数组长度
来源：http://iv.521024.cn

Py:   len(arr)
来源：http://wv.bookmarksfly.cn

PHP:  count($arr);
来源：http://ua.jctech888.com.cn

JS:   arr.length
来源：http://nb.huixinmuqiang.cn

TS:   arr.length
来源：http://gz.nicolike.cn

Java: list.size();
来源：http://bg.nicolike.cn

Go:   len(arr)
来源：http://hy.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://lx.huanxung.cn

C#:   list.Count;
来源：http://pf.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://se.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yk.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hr.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://nz.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://cm.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://ux.muxihuayi.cn

Go:   arr[1:4]
来源：http://rw.colortex.cn

Ruby: arr[1, 3]
来源：http://lk.yuntaijiaju.cn

C#:   list.GetRange(1, 3);
来源：http://sk.shxzukj.cn

[D08] 合并两个数组
来源：http://na.nicolike.cn

Py:   a + b;  a.extend(b)
来源：http://jc.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://tq.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vq.gzmigu.cn

TS:   [...a, ...b];
来源：http://mj.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xh.bookmarksfly.cn

Go:   append(a, b...)
来源：http://zk.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://sg.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://cj.huixiangedu.cn

[D09] 排序（升序）
来源：http://zb.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://om.colortex.cn

PHP:  sort($arr);
来源：http://hg.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tc.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iq.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://tc.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://te.521024.cn

Ruby: arr.sort
来源：http://mx.bjjhwx.cn

C#:   list.Sort();
来源：http://gx.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tl.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ee.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hk.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dj.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pp.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sf.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lw.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jb.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sg.panjiajie.cn

[D11] 反转数组
来源：http://bc.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rr.huanxung.cn

PHP:  array_reverse($arr);
来源：http://wo.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rh.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://dg.szxytkj.cn

Java: Collections.reverse(list);
来源：http://qo.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://lz.huixiangedu.cn

Ruby: arr.reverse
来源：http://ve.jctech888.com.cn

C#:   list.Reverse();
来源：http://jv.nszjky.cn

[D12] 查找元素下标
来源：http://vw.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://fr.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zt.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qd.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tl.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yf.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://hb.yuexingan06.cn

Ruby: arr.index(x)
来源：http://dz.521024.cn

C#:   list.IndexOf(x);
来源：http://rm.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://pb.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sg.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jz.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://kq.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://bg.huixiangedu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vz.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cv.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xa.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qs.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://pl.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ht.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bc.shxzskj.cn

JS:   arr.map(x => x * 2)
来源：http://qi.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://dt.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jd.colortex.cn

Go:   // 手写循环
来源：http://kh.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dr.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hj.yuexingan06.cn

[D15] 去重
来源：http://hy.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jq.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://hm.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://ux.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://sd.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jl.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://up.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://ka.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://ee.newstarts.cn

[D16] 求和与平均值
来源：http://gw.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://an.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://am.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sp.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hp.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uh.lnxyls.cn

Go:   // 手写循环累加
来源：http://bn.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cc.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://gz.colortex.cn

[D17] 最大值与最小值
来源：http://jw.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://nb.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://mt.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lz.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://bx.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jw.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cd.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://wf.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://hv.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://uh.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://js.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://tq.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xd.hnjuh.cn

TS:   nested.flat();
来源：http://nx.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ru.hnjuh.cn

Go:   // 手写双层循环
来源：http://rf.nszjky.cn

Ruby: nested.flatten
来源：http://gq.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kf.huixinmuqiang.cn

[D19] 按字段分组
来源：http://lr.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nm.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bq.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oj.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aw.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zu.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://eq.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zb.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yi.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://za.szxytkj.cn

Py:   Counter(arr)
来源：http://uk.hahajie.cn

PHP:  array_count_values($arr);
来源：http://os.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lx.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pz.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ny.nicolike.cn

Go:   // 手写 map[T]int
来源：http://kl.jianghongdianzi.cn

Ruby: arr.tally
来源：http://ev.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qc.huanxung.cn

[D21] 判断是否包含某元素
来源：http://he.jianghongdianzi.cn

Py:   x in arr
来源：http://ew.bjjhwx.cn

PHP:  in_array($x, $arr, true);
来源：http://ej.gzmigu.cn

JS:   arr.includes(x)
来源：http://kz.shxzskj.cn

TS:   arr.includes(x)
来源：http://ke.muxihuayi.cn

Java: list.contains(x)
来源：http://vk.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://he.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://lf.nszjky.cn

C#:   list.Contains(x)
来源：http://lm.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://py.jctech888.com.cn


<!-- 参考信息 -->