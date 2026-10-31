代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://sj.wgjwhj.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://um.bjjhwx.cn

[C04] 命名参数 / 关键字参数
来源：http://wk.newstarts.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uy.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cm.nszjky.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ov.yuexingan06.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ze.lnxyls.cn

Java: // 无：用 Builder 模式或 record
来源：http://eh.nszjky.cn

Go:   // 无：用配置结构体参数
来源：http://dt.nszjky.cn

Ruby: f(a: 1, b: 2)
来源：http://dh.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://jh.colortex.cn

[C05] 返回多个值
来源：http://uk.521024.cn

Py:   return a, b
来源：http://uq.521024.cn

PHP:  return [$a, $b];
来源：http://no.wgjwhj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ac.shxzukj.cn

TS:   return { a, b };
来源：http://cn.colortex.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rr.shxzskj.cn

Go:   return a, b
来源：http://oc.colortex.cn

Ruby: return a, b
来源：http://ws.gzmigu.cn

C#:   return (a, b);              // ValueTuple
来源：http://ad.9csxet.cn

[C06] 匿名函数 / lambda
来源：http://jx.hahajie.cn

Py:   square = lambda x: x * x
来源：http://dv.9csxet.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ha.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://vv.szsharing.cn

TS:   const square = (x: number): number => x * x;
来源：http://ky.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://th.bjjhwx.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gv.bjjhwx.cn

Ruby: square = ->(x) { x * x }
来源：http://qr.yuntaijiaju.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kj.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://kd.huanxung.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zo.nicolike.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ok.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bo.newstarts.cn

TS:   arr.map(String)
来源：http://al.shxzskj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lw.huixiangedu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://op.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://ch.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wd.huixiangedu.cn

[C08] 闭包
来源：http://zs.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ek.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zy.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ds.muxihuayi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qo.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://or.hnjuh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ts.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ht.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lx.jianghongdianzi.cn

[C09] 递归
来源：http://vb.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://an.asd995.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hf.newstarts.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rb.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dl.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ma.521024.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pu.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://eb.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uy.jianghongdianzi.cn

[C10] 变量作用域
来源：http://du.lnxyls.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ot.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vx.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ak.yuexingan06.cn

TS:   同 JS
来源：http://kh.newstarts.cn

Java: 方法内为块级作用域
来源：http://eh.shtwfgs.cn

Go:   花括号块级作用域
来源：http://af.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ab.jianghongdianzi.cn

C#:   块级作用域
来源：http://ep.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://pu.haigaiapp.cn

Py:   from module import func
来源：http://pq.shxzukj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ff.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://av.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://af.shxzskj.cn

Java: import java.util.List;
来源：http://wt.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hs.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://np.huixinmuqiang.cn

C#:   using System.Text;
来源：http://qh.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://ij.asd995.cn

Py:   (lambda: print("run"))()
来源：http://do.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://ai.huixinmuqiang.cn

JS:   (() => { console.log("run"); })();
来源：http://zz.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://fy.wgjwhj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://if.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://wn.bookmarksfly.cn

Ruby: -> { puts "run" }.call
来源：http://jz.huanxung.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ls.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://lz.nicolike.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://je.yuntaijiaju.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yn.yuexingan06.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lr.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kg.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://me.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://cn.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ez.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fv.colortex.cn

[C14] 泛型函数
来源：http://vk.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://da.panjiajie.cn

PHP:  // 无泛型
来源：http://om.shxzskj.cn

JS:   // 无泛型
来源：http://aq.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oz.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ba.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fo.hnjuh.cn

Ruby: # 无泛型
来源：http://iz.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aj.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://fw.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ev.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://ov.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cb.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wr.huixiangedu.cn

Java: // 无解构
来源：http://xm.yuntaijiaju.cn

Go:   // 无解构
来源：http://tx.muxihuayi.cn

Ruby: a, b = pair
来源：http://nn.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://lk.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://hd.shxzukj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fw.huanxung.cn

PHP:  // 无重载
来源：http://qy.hahajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://er.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://if.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cl.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://cy.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://ib.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jz.shxzukj.cn

================================================================================
来源：http://vy.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://ow.bjjhwx.cn

================================================================================
来源：http://kd.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://qj.huanxung.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kr.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ss.bookmarksfly.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://oa.wgjwhj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hj.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cx.asd995.cn

Go:   arr := []int{1, 2, 3}
来源：http://je.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://bi.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rx.colortex.cn

[D02] 追加元素到末尾
来源：http://rc.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fv.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tb.huanxung.cn

JS:   arr.push(4);
来源：http://xi.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://pa.huanxung.cn

Java: list.add(4);
来源：http://qd.colortex.cn

Go:   arr = append(arr, 4)
来源：http://bu.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://ip.lnxyls.cn

C#:   list.Add(4);
来源：http://mz.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://lw.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://kt.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pz.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dt.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://vg.nicolike.cn

Java: list.add(0, 0);
来源：http://nz.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xh.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fn.9csxet.cn

C#:   list.Insert(0, 0);
来源：http://dz.jianghongdianzi.cn

[D04] 删除元素
来源：http://ks.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://il.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hx.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tu.colortex.cn

TS:   arr.splice(0, 1);
来源：http://rc.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lr.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fe.9csxet.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://st.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bp.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://yl.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://al.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ac.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ae.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://qh.yuexingan06.cn

Java: list.get(0); list.set(0, 9);
来源：http://bk.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://qq.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gv.nicolike.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dc.panjiajie.cn

[D06] 数组长度
来源：http://at.nicolike.cn

Py:   len(arr)
来源：http://tl.lnxyls.cn

PHP:  count($arr);
来源：http://hj.muxihuayi.cn

JS:   arr.length
来源：http://zq.shxzukj.cn

TS:   arr.length
来源：http://mp.newstarts.cn

Java: list.size();
来源：http://ao.panjiajie.cn

Go:   len(arr)
来源：http://yk.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://ew.bjjhwx.cn

C#:   list.Count;
来源：http://oy.huanxung.cn

[D07] 切片 / 取子数组
来源：http://bg.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wp.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jk.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://pj.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://qd.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://rf.szsharing.cn

Go:   arr[1:4]
来源：http://jg.szsharing.cn

Ruby: arr[1, 3]
来源：http://fo.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://mx.shxzskj.cn

[D08] 合并两个数组
来源：http://py.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://sv.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://wo.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://su.szxytkj.cn

TS:   [...a, ...b];
来源：http://qr.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zi.shxzskj.cn

Go:   append(a, b...)
来源：http://bd.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://vy.wgjwhj.cn

C#:   a.Concat(b).ToList()
来源：http://lo.szxytkj.cn

[D09] 排序（升序）
来源：http://gq.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://ab.lnxyls.cn

PHP:  sort($arr);
来源：http://mz.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lb.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vf.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oi.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sn.yuntaijiaju.cn

Ruby: arr.sort
来源：http://mu.haigaiapp.cn

C#:   list.Sort();
来源：http://bs.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fr.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xa.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qj.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ni.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rq.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xw.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vb.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ll.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hw.newstarts.cn

[D11] 反转数组
来源：http://gv.hahajie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hw.nszjky.cn

PHP:  array_reverse($arr);
来源：http://ic.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fd.shxzskj.cn

TS:   [...arr].reverse();
来源：http://yo.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://ta.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://wb.asd995.cn

Ruby: arr.reverse
来源：http://hc.yuexingan06.cn

C#:   list.Reverse();
来源：http://tl.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://ca.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://cs.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hy.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ny.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vu.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ch.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://li.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://ke.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://fk.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://ly.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kr.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rr.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://bp.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://cr.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nb.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kz.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://on.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sz.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://zh.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nz.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gq.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://sz.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://xh.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yi.jctech888.com.cn

Go:   // 手写循环
来源：http://fc.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://id.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wo.bookmarksfly.cn

[D15] 去重
来源：http://lc.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xd.shxzukj.cn

PHP:  array_unique($arr);
来源：http://mb.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://fp.yuexingan06.cn

TS:   [...new Set(arr)]
来源：http://er.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lz.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yj.shxzskj.cn

Ruby: arr.uniq
来源：http://zh.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://qk.asd995.cn

[D16] 求和与平均值
来源：http://lz.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gg.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mk.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yi.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wi.wgjwhj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gv.lnxyls.cn

Go:   // 手写循环累加
来源：http://dk.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://of.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://ur.shtwfgs.cn

[D17] 最大值与最小值
来源：http://gs.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://jg.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://xw.yuntaijiaju.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ic.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://yf.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xe.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bs.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://dj.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://hf.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://ji.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jp.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://or.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xa.hahajie.cn

TS:   nested.flat();
来源：http://hx.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://os.panjiajie.cn

Go:   // 手写双层循环
来源：http://an.muxihuayi.cn

Ruby: nested.flatten
来源：http://hm.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fn.shxzukj.cn

[D19] 按字段分组
来源：http://yo.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rp.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xn.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gu.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xb.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wf.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://wd.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://si.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zv.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ek.haigaiapp.cn

Py:   Counter(arr)
来源：http://jh.nicolike.cn

PHP:  array_count_values($arr);
来源：http://kg.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cx.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yg.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://se.jianghongdianzi.cn

Go:   // 手写 map[T]int
来源：http://xm.bookmarksfly.cn


<!-- 参考信息 -->