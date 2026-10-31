代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://pi.hahajie.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mi.colortex.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qe.hnjuh.cn

Ruby: square = ->(x) { x * x }
来源：http://qp.huanxung.cn

C#:   Func<int, int> square = x => x * x;
来源：http://bb.muxihuayi.cn

[C07] 把函数作为参数传入
来源：http://fv.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hf.gzmigu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cg.szsharing.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aq.wgjwhj.cn

TS:   arr.map(String)
来源：http://lq.muxihuayi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cp.521024.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ca.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://cr.shtwfgs.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ym.szxytkj.cn

[C08] 闭包
来源：http://no.asd995.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ey.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nz.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qn.jctech888.com.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qr.hnjuh.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ys.jianghongdianzi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://re.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zk.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gv.nszjky.cn

[C09] 递归
来源：http://ez.haigaiapp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rn.szxytkj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rg.chemitech.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cl.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fy.9csxet.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zn.9csxet.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://my.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nu.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dp.huixinmuqiang.cn

[C10] 变量作用域
来源：http://up.yuexingan06.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://li.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://se.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pj.szxytkj.cn

TS:   同 JS
来源：http://fd.gzmigu.cn

Java: 方法内为块级作用域
来源：http://tb.szxytkj.cn

Go:   花括号块级作用域
来源：http://zr.hahajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qs.colortex.cn

C#:   块级作用域
来源：http://gs.asd995.cn

[C11] 模块导入与导出
来源：http://ef.haigaiapp.cn

Py:   from module import func
来源：http://fm.yuexingan06.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kh.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gf.colortex.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fk.asd995.cn

Java: import java.util.List;
来源：http://wq.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://em.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://xn.hahajie.cn

C#:   using System.Text;
来源：http://fa.jctech888.com.cn

[C12] 立即执行函数 IIFE
来源：http://ns.521024.cn

Py:   (lambda: print("run"))()
来源：http://zx.szxytkj.cn

PHP:  (function () { echo "run"; })();
来源：http://op.lnxyls.cn

JS:   (() => { console.log("run"); })();
来源：http://ii.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://yc.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mv.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://qr.9csxet.cn

Ruby: -> { puts "run" }.call
来源：http://nz.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ge.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://lz.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://af.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vb.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zj.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ms.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wj.szsharing.cn

Go:   func add(a, b int) int
来源：http://up.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sa.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mw.nicolike.cn

[C14] 泛型函数
来源：http://ec.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bm.huanxung.cn

PHP:  // 无泛型
来源：http://ib.huanxung.cn

JS:   // 无泛型
来源：http://jp.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ug.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nq.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ce.huanxung.cn

Ruby: # 无泛型
来源：http://aj.yuexingan06.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lo.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://jx.huixiangedu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hh.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://px.huixiangedu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://li.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kh.asd995.cn

Java: // 无解构
来源：http://rh.asd995.cn

Go:   // 无解构
来源：http://gw.lnxyls.cn

Ruby: a, b = pair
来源：http://yd.jctech888.com.cn

C#:   var (a, b) = pair;
来源：http://gw.asd995.cn

[C16] 函数 / 方法重载
来源：http://vt.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oc.shtwfgs.cn

PHP:  // 无重载
来源：http://nv.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sf.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://un.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jz.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ky.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://yw.hnjuh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ff.shxzskj.cn

================================================================================
来源：http://au.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://nx.asd995.cn

================================================================================
来源：http://py.colortex.cn

[D01] 创建数组 / 列表
来源：http://jz.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://aw.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bb.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sr.asd995.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yw.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cz.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://kq.yuexingan06.cn

Ruby: arr = [1, 2, 3]
来源：http://aa.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zo.newstarts.cn

[D02] 追加元素到末尾
来源：http://hm.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://en.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pc.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://fg.shxzskj.cn

TS:   arr.push(4);
来源：http://am.9csxet.cn

Java: list.add(4);
来源：http://do.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://bk.colortex.cn

Ruby: arr << 4; arr.push(5)
来源：http://dz.bjjhwx.cn

C#:   list.Add(4);
来源：http://si.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://dk.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://gz.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ro.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://az.szsharing.cn

TS:   arr.splice(0, 0, 0);
来源：http://pu.yuexingan06.cn

Java: list.add(0, 0);
来源：http://uc.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://il.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wv.colortex.cn

C#:   list.Insert(0, 0);
来源：http://sg.huanxung.cn

[D04] 删除元素
来源：http://aw.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zf.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ic.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fu.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://ye.asd995.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rs.lnxyls.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qg.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gv.521024.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jq.hnjuh.cn

[D05] 访问与修改元素
来源：http://lq.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nc.hahajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zm.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ba.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://ho.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://kv.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ia.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sz.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ch.bookmarksfly.cn

[D06] 数组长度
来源：http://fo.hahajie.cn

Py:   len(arr)
来源：http://ib.shxzukj.cn

PHP:  count($arr);
来源：http://nu.huanxung.cn

JS:   arr.length
来源：http://uv.bookmarksfly.cn

TS:   arr.length
来源：http://fd.lnxyls.cn

Java: list.size();
来源：http://sj.bookmarksfly.cn

Go:   len(arr)
来源：http://rd.hahajie.cn

Ruby: arr.length; arr.size
来源：http://ha.huanxung.cn

C#:   list.Count;
来源：http://kr.shtwfgs.cn

[D07] 切片 / 取子数组
来源：http://hp.wgjwhj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lj.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yj.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://gr.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://ta.huixiangedu.cn

Java: list.subList(1, 4);
来源：http://qi.szsharing.cn

Go:   arr[1:4]
来源：http://vo.panjiajie.cn

Ruby: arr[1, 3]
来源：http://ok.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://ne.nszjky.cn

[D08] 合并两个数组
来源：http://ss.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://tc.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://gj.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wz.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://wr.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lc.muxihuayi.cn

Go:   append(a, b...)
来源：http://mw.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://xj.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://ex.hnjuh.cn

[D09] 排序（升序）
来源：http://zy.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://zn.bjjhwx.cn

PHP:  sort($arr);
来源：http://qj.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mz.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lx.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jd.chemitech.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wi.nicolike.cn

Ruby: arr.sort
来源：http://dx.wgjwhj.cn

C#:   list.Sort();
来源：http://wi.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ii.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hp.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cz.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qa.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ds.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dm.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uq.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hf.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hn.nszjky.cn

[D11] 反转数组
来源：http://rl.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://od.nszjky.cn

PHP:  array_reverse($arr);
来源：http://vo.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dr.haigaiapp.cn

TS:   [...arr].reverse();
来源：http://wu.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://gp.asd995.cn

Go:   slices.Reverse(arr)
来源：http://dp.jctech888.com.cn

Ruby: arr.reverse
来源：http://yf.muxihuayi.cn

C#:   list.Reverse();
来源：http://oh.szxytkj.cn

[D12] 查找元素下标
来源：http://iq.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://pz.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tu.huixiangedu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cr.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://la.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rw.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://gs.521024.cn

Ruby: arr.index(x)
来源：http://bu.nicolike.cn

C#:   list.IndexOf(x);
来源：http://wu.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://tu.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hx.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gr.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://xe.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://dw.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zr.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ys.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wi.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qr.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://ze.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://od.gzmigu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ah.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://zn.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://he.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iw.nszjky.cn

Go:   // 手写循环
来源：http://fl.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gp.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gn.hnjuh.cn

[D15] 去重
来源：http://st.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zu.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://od.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://bt.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://gj.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hc.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://js.bookmarksfly.cn

Ruby: arr.uniq
来源：http://cr.521024.cn

C#:   list.Distinct().ToList()
来源：http://wj.bookmarksfly.cn

[D16] 求和与平均值
来源：http://yw.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sz.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nl.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gl.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pm.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gr.panjiajie.cn

Go:   // 手写循环累加
来源：http://fl.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eg.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://vf.wgjwhj.cn

[D17] 最大值与最小值
来源：http://yp.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://ug.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://ma.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ns.521024.cn

TS:   Math.max(...arr);
来源：http://dx.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jh.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tw.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://uv.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://zl.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://do.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mp.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://nk.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rc.9csxet.cn

TS:   nested.flat();
来源：http://pw.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vk.hnjuh.cn

Go:   // 手写双层循环
来源：http://yp.521024.cn

Ruby: nested.flatten
来源：http://rh.panjiajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tn.haigaiapp.cn

[D19] 按字段分组
来源：http://sz.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ta.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ev.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mo.shtwfgs.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tv.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jz.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://wg.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mx.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wu.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://gt.bjjhwx.cn

Py:   Counter(arr)
来源：http://mi.colortex.cn

PHP:  array_count_values($arr);
来源：http://yp.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://be.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yh.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xd.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://vc.szsharing.cn

Ruby: arr.tally
来源：http://gx.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nw.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://ij.muxihuayi.cn

Py:   x in arr
来源：http://zn.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://bj.muxihuayi.cn

JS:   arr.includes(x)
来源：http://ba.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://kw.jctech888.com.cn

Java: list.contains(x)
来源：http://in.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://fl.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://xl.nszjky.cn

C#:   list.Contains(x)
来源：http://ec.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://mt.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ea.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eo.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zv.wgjwhj.cn

TS:   [...arr];
来源：http://fp.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://ab.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ld.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://qo.yuexingan06.cn

C#:   new List<int>(list);
来源：http://rl.newstarts.cn

[D23] reduce 累积计算
来源：http://hj.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lz.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cf.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gu.gzmigu.cn


<!-- 参考信息 -->