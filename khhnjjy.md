代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aj.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://az.nszjky.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pg.newstarts.cn

Java: // 无：用 Builder 模式或 record
来源：http://cj.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://sk.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://cc.wgjwhj.cn

C#:   f(a: 1, b: 2)
来源：http://dz.gzmigu.cn

[C05] 返回多个值
来源：http://pg.haigaiapp.cn

Py:   return a, b
来源：http://dz.panjiajie.cn

PHP:  return [$a, $b];
来源：http://fe.nicolike.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bb.hahajie.cn

TS:   return { a, b };
来源：http://mn.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://id.nszjky.cn

Go:   return a, b
来源：http://yo.shxzukj.cn

Ruby: return a, b
来源：http://kj.521024.cn

C#:   return (a, b);              // ValueTuple
来源：http://rq.hahajie.cn

[C06] 匿名函数 / lambda
来源：http://xr.huixiangedu.cn

Py:   square = lambda x: x * x
来源：http://sb.shtwfgs.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tt.hnjuh.cn

JS:   const square = x => x * x;
来源：http://zj.wgjwhj.cn

TS:   const square = (x: number): number => x * x;
来源：http://xf.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yg.huanxung.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iw.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://jj.jianghongdianzi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cu.szxytkj.cn

[C07] 把函数作为参数传入
来源：http://hv.panjiajie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vc.hnjuh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vg.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ym.shtwfgs.cn

TS:   arr.map(String)
来源：http://yb.nicolike.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bs.muxihuayi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uu.bookmarksfly.cn

Ruby: arr.map(&:upcase)
来源：http://xj.wgjwhj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://za.muxihuayi.cn

[C08] 闭包
来源：http://cb.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ng.panjiajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bo.huixiangedu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vt.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ne.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://po.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sk.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lu.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://re.shxzskj.cn

[C09] 递归
来源：http://tb.nicolike.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ja.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gv.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rk.521024.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zs.yuexingan06.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zz.yuntaijiaju.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://av.wgjwhj.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dx.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lx.shxzukj.cn

[C10] 变量作用域
来源：http://um.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://za.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ue.haigaiapp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ge.yuntaijiaju.cn

TS:   同 JS
来源：http://lw.colortex.cn

Java: 方法内为块级作用域
来源：http://gs.shxzskj.cn

Go:   花括号块级作用域
来源：http://ui.panjiajie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lm.lnxyls.cn

C#:   块级作用域
来源：http://sv.bjjhwx.cn

[C11] 模块导入与导出
来源：http://sn.gzmigu.cn

Py:   from module import func
来源：http://hg.chemitech.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://yn.asd995.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://em.newstarts.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iz.lnxyls.cn

Java: import java.util.List;
来源：http://je.shtwfgs.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ab.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://di.bjjhwx.cn

C#:   using System.Text;
来源：http://eu.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://te.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://qr.shxzskj.cn

PHP:  (function () { echo "run"; })();
来源：http://iu.bookmarksfly.cn

JS:   (() => { console.log("run"); })();
来源：http://vo.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://zw.newstarts.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vk.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://ov.chemitech.net.cn

Ruby: -> { puts "run" }.call
来源：http://zc.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jp.asd995.cn

[C13] 类型声明 / 类型注解
来源：http://wf.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ls.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://in.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pb.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pl.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://ga.szxytkj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yc.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qs.hnjuh.cn

[C14] 泛型函数
来源：http://ub.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ie.9csxet.cn

PHP:  // 无泛型
来源：http://om.newstarts.cn

JS:   // 无泛型
来源：http://gu.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nd.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dl.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ck.521024.cn

Ruby: # 无泛型
来源：http://vp.lnxyls.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://to.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://eu.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vm.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://ig.nicolike.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ke.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zf.szxytkj.cn

Java: // 无解构
来源：http://te.nszjky.cn

Go:   // 无解构
来源：http://go.bjjhwx.cn

Ruby: a, b = pair
来源：http://yt.huanxung.cn

C#:   var (a, b) = pair;
来源：http://zy.9csxet.cn

[C16] 函数 / 方法重载
来源：http://eg.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ob.newstarts.cn

PHP:  // 无重载
来源：http://in.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vz.jianghongdianzi.cn

TS:   // 用联合类型或重载签名声明
来源：http://zn.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kz.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://yz.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://wc.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hg.yuntaijiaju.cn

================================================================================
来源：http://si.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://cy.jianghongdianzi.cn

================================================================================
来源：http://ao.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://gl.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xw.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vp.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zk.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bu.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hq.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://il.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://or.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tm.colortex.cn

[D02] 追加元素到末尾
来源：http://xe.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mo.shxzskj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ue.wgjwhj.cn

JS:   arr.push(4);
来源：http://km.huanxung.cn

TS:   arr.push(4);
来源：http://rw.haigaiapp.cn

Java: list.add(4);
来源：http://gh.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://bx.newstarts.cn

Ruby: arr << 4; arr.push(5)
来源：http://aq.szxytkj.cn

C#:   list.Add(4);
来源：http://as.bookmarksfly.cn

[D03] 在指定位置插入元素
来源：http://fk.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://zw.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dn.huanxung.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://im.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://vg.shxzskj.cn

Java: list.add(0, 0);
来源：http://px.shxzskj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pd.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qa.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://hi.wgjwhj.cn

[D04] 删除元素
来源：http://ne.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gw.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://he.muxihuayi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sb.jctech888.com.cn

TS:   arr.splice(0, 1);
来源：http://vl.lnxyls.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tg.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ym.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ka.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dy.muxihuayi.cn

[D05] 访问与修改元素
来源：http://yj.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wd.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cj.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tp.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://dn.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://is.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://ef.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uw.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kl.huanxung.cn

[D06] 数组长度
来源：http://gb.lnxyls.cn

Py:   len(arr)
来源：http://jt.wgjwhj.cn

PHP:  count($arr);
来源：http://eq.colortex.cn

JS:   arr.length
来源：http://pt.wgjwhj.cn

TS:   arr.length
来源：http://zo.colortex.cn

Java: list.size();
来源：http://rc.bjjhwx.cn

Go:   len(arr)
来源：http://yg.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://bh.nszjky.cn

C#:   list.Count;
来源：http://xb.huanxung.cn

[D07] 切片 / 取子数组
来源：http://ps.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zu.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://tf.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://th.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://qu.lnxyls.cn

Java: list.subList(1, 4);
来源：http://ll.gzmigu.cn

Go:   arr[1:4]
来源：http://uz.colortex.cn

Ruby: arr[1, 3]
来源：http://zx.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://vg.huanxung.cn

[D08] 合并两个数组
来源：http://vw.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://um.asd995.cn

PHP:  array_merge($a, $b);
来源：http://dt.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xo.shxzskj.cn

TS:   [...a, ...b];
来源：http://tm.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://tt.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://iu.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://sl.yuexingan06.cn

[D09] 排序（升序）
来源：http://lk.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://eh.asd995.cn

PHP:  sort($arr);
来源：http://ua.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gp.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nz.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ec.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uz.szsharing.cn

Ruby: arr.sort
来源：http://li.shxzukj.cn

C#:   list.Sort();
来源：http://cg.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xe.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rw.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jg.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qc.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mn.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bk.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ut.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jc.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tg.muxihuayi.cn

[D11] 反转数组
来源：http://ww.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wd.huixiangedu.cn

PHP:  array_reverse($arr);
来源：http://ze.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yj.gzmigu.cn

TS:   [...arr].reverse();
来源：http://jo.szxytkj.cn

Java: Collections.reverse(list);
来源：http://ou.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://pu.yuexingan06.cn

Ruby: arr.reverse
来源：http://uf.panjiajie.cn

C#:   list.Reverse();
来源：http://pa.shtwfgs.cn

[D12] 查找元素下标
来源：http://as.chemitech.net.cn

Py:   arr.index(x);  x in arr
来源：http://iq.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tw.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cm.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zb.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ha.yuexingan06.cn

Go:   slices.Index(arr, x)
来源：http://sw.huixiangedu.cn

Ruby: arr.index(x)
来源：http://or.nicolike.cn

C#:   list.IndexOf(x);
来源：http://oj.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://td.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fe.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oe.newstarts.cn

JS:   arr.filter(x => x > 3)
来源：http://is.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://zl.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xa.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eo.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dx.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oe.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://yg.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xh.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ix.521024.cn

JS:   arr.map(x => x * 2)
来源：http://zz.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://in.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ld.hnjuh.cn

Go:   // 手写循环
来源：http://qe.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yt.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kd.szxytkj.cn

[D15] 去重
来源：http://km.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ef.szsharing.cn

PHP:  array_unique($arr);
来源：http://up.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://nx.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://cg.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wg.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://df.jctech888.com.cn

Ruby: arr.uniq
来源：http://dk.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://mg.panjiajie.cn

[D16] 求和与平均值
来源：http://yn.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ic.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yx.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hv.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ex.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xq.nszjky.cn

Go:   // 手写循环累加
来源：http://nq.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dj.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://na.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://bn.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://fc.521024.cn

PHP:  max($arr);  min($arr);
来源：http://zw.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gk.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://cy.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://af.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gf.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://el.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://cw.jianghongdianzi.cn

[D18] 扁平化嵌套数组
来源：http://lr.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yy.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://jr.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vf.szxytkj.cn

TS:   nested.flat();
来源：http://mi.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sz.jctech888.com.cn

Go:   // 手写双层循环
来源：http://eh.gzmigu.cn

Ruby: nested.flatten
来源：http://ew.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wv.nicolike.cn

[D19] 按字段分组
来源：http://os.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nf.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ck.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kh.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://he.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eh.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://ip.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://az.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hm.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://rz.jctech888.com.cn

Py:   Counter(arr)
来源：http://sy.nszjky.cn

PHP:  array_count_values($arr);
来源：http://to.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://za.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mk.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sp.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://xt.asd995.cn

Ruby: arr.tally
来源：http://vn.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wu.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://gq.huanxung.cn

Py:   x in arr
来源：http://dt.muxihuayi.cn


<!-- 参考信息 -->