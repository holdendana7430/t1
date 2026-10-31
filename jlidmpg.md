代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://hy.lnxyls.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xr.shxzskj.cn

[C04] 命名参数 / 关键字参数
来源：http://ve.bjjhwx.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ox.wgjwhj.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ze.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ae.colortex.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ts.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://gd.jctech888.com.cn

Go:   // 无：用配置结构体参数
来源：http://yz.szsharing.cn

Ruby: f(a: 1, b: 2)
来源：http://yu.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://vb.muxihuayi.cn

[C05] 返回多个值
来源：http://qp.chemitech.net.cn

Py:   return a, b
来源：http://ag.szxytkj.cn

PHP:  return [$a, $b];
来源：http://if.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bp.haigaiapp.cn

TS:   return { a, b };
来源：http://yd.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yu.jctech888.com.cn

Go:   return a, b
来源：http://dc.asd995.cn

Ruby: return a, b
来源：http://cp.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://li.chemitech.net.cn

[C06] 匿名函数 / lambda
来源：http://wp.shxzskj.cn

Py:   square = lambda x: x * x
来源：http://qx.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fz.shxzukj.cn

JS:   const square = x => x * x;
来源：http://ek.521024.cn

TS:   const square = (x: number): number => x * x;
来源：http://qz.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tf.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://za.9csxet.cn

Ruby: square = ->(x) { x * x }
来源：http://ye.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dq.wgjwhj.cn

[C07] 把函数作为参数传入
来源：http://wq.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ve.newstarts.cn

PHP:  array_map("strtoupper", $arr);
来源：http://sp.jctech888.com.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kt.bookmarksfly.cn

TS:   arr.map(String)
来源：http://wb.szxytkj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kg.colortex.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fg.bjjhwx.cn

Ruby: arr.map(&:upcase)
来源：http://zl.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ig.lnxyls.cn

[C08] 闭包
来源：http://je.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hj.9csxet.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kg.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://og.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jd.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zq.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gj.colortex.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lr.9csxet.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sl.haigaiapp.cn

[C09] 递归
来源：http://kb.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qd.wgjwhj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ht.bjjhwx.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tg.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ze.chemitech.net.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ce.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kj.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zd.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vg.shtwfgs.cn

[C10] 变量作用域
来源：http://wj.gzmigu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tm.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://og.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ko.wgjwhj.cn

TS:   同 JS
来源：http://mv.hahajie.cn

Java: 方法内为块级作用域
来源：http://uv.nszjky.cn

Go:   花括号块级作用域
来源：http://cj.huixiangedu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jx.521024.cn

C#:   块级作用域
来源：http://gd.newstarts.cn

[C11] 模块导入与导出
来源：http://ud.asd995.cn

Py:   from module import func
来源：http://sm.huixiangedu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tw.bjjhwx.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hm.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dl.shtwfgs.cn

Java: import java.util.List;
来源：http://gc.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mu.yuntaijiaju.cn

Ruby: require "json"; require_relative "./util"
来源：http://mk.gzmigu.cn

C#:   using System.Text;
来源：http://yc.muxihuayi.cn

[C12] 立即执行函数 IIFE
来源：http://cl.jctech888.com.cn

Py:   (lambda: print("run"))()
来源：http://lw.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://xd.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://vz.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://br.shxzskj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://aa.huixinmuqiang.cn

Go:   func() { fmt.Println("run") }()
来源：http://tr.szsharing.cn

Ruby: -> { puts "run" }.call
来源：http://nw.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ck.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://gx.gzmigu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ls.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mb.lnxyls.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ux.huixinmuqiang.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ac.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kp.shxzukj.cn

Go:   func add(a, b int) int
来源：http://ul.huanxung.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bo.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tc.asd995.cn

[C14] 泛型函数
来源：http://kx.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ns.muxihuayi.cn

PHP:  // 无泛型
来源：http://pm.wgjwhj.cn

JS:   // 无泛型
来源：http://yq.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kr.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mr.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ki.chemitech.net.cn

Ruby: # 无泛型
来源：http://dn.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lt.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://xv.yuexingan06.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mw.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://tu.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jf.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dr.szxytkj.cn

Java: // 无解构
来源：http://iv.szxytkj.cn

Go:   // 无解构
来源：http://mo.shxzskj.cn

Ruby: a, b = pair
来源：http://tr.shtwfgs.cn

C#:   var (a, b) = pair;
来源：http://iy.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://iq.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mv.panjiajie.cn

PHP:  // 无重载
来源：http://ij.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gc.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://zf.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://om.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://yv.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://yo.jianghongdianzi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yz.colortex.cn

================================================================================
来源：http://pt.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://hw.szsharing.cn

================================================================================
来源：http://xd.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://kz.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://di.wgjwhj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sg.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yk.lnxyls.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://aw.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bl.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://lz.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://eb.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eq.hahajie.cn

[D02] 追加元素到末尾
来源：http://lq.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gq.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kc.shxzskj.cn

JS:   arr.push(4);
来源：http://rc.hahajie.cn

TS:   arr.push(4);
来源：http://oo.colortex.cn

Java: list.add(4);
来源：http://my.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://xu.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://nd.wgjwhj.cn

C#:   list.Add(4);
来源：http://tj.colortex.cn

[D03] 在指定位置插入元素
来源：http://xn.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://dl.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ma.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bf.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://el.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://hr.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wo.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sz.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://dr.bookmarksfly.cn

[D04] 删除元素
来源：http://tb.hahajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nh.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://na.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gt.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://id.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yv.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sq.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lt.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gs.shtwfgs.cn

[D05] 访问与修改元素
来源：http://wj.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ev.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ra.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pi.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://tx.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://er.jctech888.com.cn

Go:   arr[0]; arr[0] = 9
来源：http://ad.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ks.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://do.nszjky.cn

[D06] 数组长度
来源：http://hr.panjiajie.cn

Py:   len(arr)
来源：http://ra.huixinmuqiang.cn

PHP:  count($arr);
来源：http://og.wgjwhj.cn

JS:   arr.length
来源：http://jt.yuexingan06.cn

TS:   arr.length
来源：http://mb.muxihuayi.cn

Java: list.size();
来源：http://zm.nszjky.cn

Go:   len(arr)
来源：http://xs.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://ot.shtwfgs.cn

C#:   list.Count;
来源：http://kv.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://pm.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zl.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vo.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://jz.asd995.cn

TS:   arr.slice(1, 4);
来源：http://mq.szsharing.cn

Java: list.subList(1, 4);
来源：http://eb.szxytkj.cn

Go:   arr[1:4]
来源：http://lb.huixinmuqiang.cn

Ruby: arr[1, 3]
来源：http://eu.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://rm.wgjwhj.cn

[D08] 合并两个数组
来源：http://xf.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://gs.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://ql.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vv.newstarts.cn

TS:   [...a, ...b];
来源：http://pk.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zd.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://cu.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://ny.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://fy.bookmarksfly.cn

[D09] 排序（升序）
来源：http://od.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://tn.lnxyls.cn

PHP:  sort($arr);
来源：http://hl.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mm.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gu.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ix.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vg.hnjuh.cn

Ruby: arr.sort
来源：http://cm.haigaiapp.cn

C#:   list.Sort();
来源：http://wg.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kp.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hm.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cv.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lc.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oc.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vl.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kw.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mp.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ga.nicolike.cn

[D11] 反转数组
来源：http://sa.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lk.colortex.cn

PHP:  array_reverse($arr);
来源：http://sd.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://os.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://ql.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://po.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://ls.haigaiapp.cn

Ruby: arr.reverse
来源：http://wc.nszjky.cn

C#:   list.Reverse();
来源：http://oa.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://oo.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://ud.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kg.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jd.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zd.colortex.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sj.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://wi.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://ns.asd995.cn

C#:   list.IndexOf(x);
来源：http://qo.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://xc.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ma.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nf.shxzskj.cn

JS:   arr.filter(x => x > 3)
来源：http://ex.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://oi.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ny.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qj.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qa.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bp.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://cs.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bw.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fw.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://pt.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://ct.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kx.521024.cn

Go:   // 手写循环
来源：http://bg.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ng.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://br.bookmarksfly.cn

[D15] 去重
来源：http://nb.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zg.nszjky.cn

PHP:  array_unique($arr);
来源：http://gz.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://yg.hahajie.cn

TS:   [...new Set(arr)]
来源：http://hb.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ae.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vn.shxzukj.cn

Ruby: arr.uniq
来源：http://la.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://ua.szsharing.cn

[D16] 求和与平均值
来源：http://aa.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tp.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wk.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ci.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ht.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lk.yuexingan06.cn

Go:   // 手写循环累加
来源：http://ap.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://if.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://tv.haigaiapp.cn

[D17] 最大值与最小值
来源：http://fw.521024.cn

Py:   max(arr);  min(arr)
来源：http://qr.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://ar.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yh.huanxung.cn

TS:   Math.max(...arr);
来源：http://gn.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lq.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://po.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://yo.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://do.hahajie.cn

[D18] 扁平化嵌套数组
来源：http://ne.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lp.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://kr.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ya.jianghongdianzi.cn

TS:   nested.flat();
来源：http://vo.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ik.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://kb.haigaiapp.cn

Ruby: nested.flatten
来源：http://av.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tr.newstarts.cn

[D19] 按字段分组
来源：http://tz.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uu.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ab.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pp.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uy.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uk.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://pb.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kp.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ha.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://fh.asd995.cn

Py:   Counter(arr)
来源：http://hl.huanxung.cn

PHP:  array_count_values($arr);
来源：http://li.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hf.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eg.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://to.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://vu.szsharing.cn


<!-- 参考信息 -->