代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://tj.nszjky.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lb.szsharing.cn

[C04] 命名参数 / 关键字参数
来源：http://yl.wgjwhj.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mv.yuexingan06.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mq.hnjuh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yo.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://io.bjjhwx.cn

Java: // 无：用 Builder 模式或 record
来源：http://ti.bjjhwx.cn

Go:   // 无：用配置结构体参数
来源：http://hr.wgjwhj.cn

Ruby: f(a: 1, b: 2)
来源：http://mq.chemitech.net.cn

C#:   f(a: 1, b: 2)
来源：http://is.521024.cn

[C05] 返回多个值
来源：http://ta.colortex.cn

Py:   return a, b
来源：http://ep.lnxyls.cn

PHP:  return [$a, $b];
来源：http://lk.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wx.nszjky.cn

TS:   return { a, b };
来源：http://yd.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://av.wgjwhj.cn

Go:   return a, b
来源：http://zh.huanxung.cn

Ruby: return a, b
来源：http://cu.wgjwhj.cn

C#:   return (a, b);              // ValueTuple
来源：http://gs.huixinmuqiang.cn

[C06] 匿名函数 / lambda
来源：http://ra.haigaiapp.cn

Py:   square = lambda x: x * x
来源：http://iz.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lj.huanxung.cn

JS:   const square = x => x * x;
来源：http://jh.yuntaijiaju.cn

TS:   const square = (x: number): number => x * x;
来源：http://dd.muxihuayi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ge.yuexingan06.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vh.huixiangedu.cn

Ruby: square = ->(x) { x * x }
来源：http://xe.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://uu.haigaiapp.cn

[C07] 把函数作为参数传入
来源：http://jl.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ma.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gs.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wg.panjiajie.cn

TS:   arr.map(String)
来源：http://rr.haigaiapp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://na.jctech888.com.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://za.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://jh.huixinmuqiang.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://em.szxytkj.cn

[C08] 闭包
来源：http://jj.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oo.haigaiapp.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gk.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://if.lnxyls.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rh.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qo.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wu.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ne.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jb.wgjwhj.cn

[C09] 递归
来源：http://fs.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zk.muxihuayi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qx.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ot.szxytkj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yz.asd995.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ld.asd995.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ti.bjjhwx.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sl.yuntaijiaju.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fv.szsharing.cn

[C10] 变量作用域
来源：http://gk.szxytkj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ze.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://se.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mr.jianghongdianzi.cn

TS:   同 JS
来源：http://ho.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://nt.gzmigu.cn

Go:   花括号块级作用域
来源：http://cn.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zy.jctech888.com.cn

C#:   块级作用域
来源：http://wa.chemitech.net.cn

[C11] 模块导入与导出
来源：http://cl.panjiajie.cn

Py:   from module import func
来源：http://pm.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vn.colortex.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jr.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://am.9csxet.cn

Java: import java.util.List;
来源：http://ku.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sd.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://hb.panjiajie.cn

C#:   using System.Text;
来源：http://sd.huixinmuqiang.cn

[C12] 立即执行函数 IIFE
来源：http://zg.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://ui.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://od.jctech888.com.cn

JS:   (() => { console.log("run"); })();
来源：http://mz.hahajie.cn

TS:   (() => { console.log("run"); })();
来源：http://ws.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ri.hahajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://bm.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://pt.newstarts.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ee.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://es.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ep.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://or.shxzskj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tn.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zg.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lp.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://jg.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://su.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jr.nicolike.cn

[C14] 泛型函数
来源：http://im.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qq.shxzskj.cn

PHP:  // 无泛型
来源：http://bj.shxzskj.cn

JS:   // 无泛型
来源：http://hx.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kq.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iw.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hj.newstarts.cn

Ruby: # 无泛型
来源：http://pb.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cl.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://ni.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oo.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://hq.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rt.szsharing.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iw.yuexingan06.cn

Java: // 无解构
来源：http://jt.shtwfgs.cn

Go:   // 无解构
来源：http://is.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://cf.newstarts.cn

C#:   var (a, b) = pair;
来源：http://ai.shtwfgs.cn

[C16] 函数 / 方法重载
来源：http://jd.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zn.jianghongdianzi.cn

PHP:  // 无重载
来源：http://mb.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mh.hnjuh.cn

TS:   // 用联合类型或重载签名声明
来源：http://bd.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rp.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://sl.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://jk.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lu.muxihuayi.cn

================================================================================
来源：http://nj.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://zx.huixiangedu.cn

================================================================================
来源：http://hd.newstarts.cn

[D01] 创建数组 / 列表
来源：http://ha.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uh.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qr.jianghongdianzi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lo.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jk.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qh.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://fv.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://id.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gs.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://um.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ws.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zn.shtwfgs.cn

JS:   arr.push(4);
来源：http://er.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://qw.szxytkj.cn

Java: list.add(4);
来源：http://tj.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://lq.lnxyls.cn

Ruby: arr << 4; arr.push(5)
来源：http://mw.bookmarksfly.cn

C#:   list.Add(4);
来源：http://zs.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://bs.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://kl.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uw.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zv.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://iz.yuexingan06.cn

Java: list.add(0, 0);
来源：http://fw.nicolike.cn

Go:   arr = append([]int{0}, arr...)
来源：http://il.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fy.lnxyls.cn

C#:   list.Insert(0, 0);
来源：http://zj.hahajie.cn

[D04] 删除元素
来源：http://tf.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://de.colortex.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://al.shtwfgs.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ml.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://fd.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hy.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pl.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jt.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://am.521024.cn

[D05] 访问与修改元素
来源：http://it.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dz.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ce.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kk.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://od.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://ra.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://tz.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lr.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qt.shxzskj.cn

[D06] 数组长度
来源：http://vc.nszjky.cn

Py:   len(arr)
来源：http://xi.gzmigu.cn

PHP:  count($arr);
来源：http://px.hnjuh.cn

JS:   arr.length
来源：http://wj.huixiangedu.cn

TS:   arr.length
来源：http://er.yuntaijiaju.cn

Java: list.size();
来源：http://mn.panjiajie.cn

Go:   len(arr)
来源：http://yr.szsharing.cn

Ruby: arr.length; arr.size
来源：http://kr.jianghongdianzi.cn

C#:   list.Count;
来源：http://nq.colortex.cn

[D07] 切片 / 取子数组
来源：http://po.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vb.shxzukj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://eh.colortex.cn

JS:   arr.slice(1, 4);
来源：http://hp.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://sh.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://ix.huixiangedu.cn

Go:   arr[1:4]
来源：http://je.panjiajie.cn

Ruby: arr[1, 3]
来源：http://nu.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://zc.haigaiapp.cn

[D08] 合并两个数组
来源：http://wk.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://hj.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://sg.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zs.521024.cn

TS:   [...a, ...b];
来源：http://oq.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wr.shtwfgs.cn

Go:   append(a, b...)
来源：http://vr.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://km.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://es.shxzukj.cn

[D09] 排序（升序）
来源：http://wh.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://qf.newstarts.cn

PHP:  sort($arr);
来源：http://py.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ey.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xb.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mt.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bc.9csxet.cn

Ruby: arr.sort
来源：http://hg.shxzskj.cn

C#:   list.Sort();
来源：http://sm.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mj.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vh.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lw.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://le.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pv.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rx.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://to.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kb.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wy.hnjuh.cn

[D11] 反转数组
来源：http://ju.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vh.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://ok.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ac.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://xt.9csxet.cn

Java: Collections.reverse(list);
来源：http://dv.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://bj.shxzukj.cn

Ruby: arr.reverse
来源：http://oq.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://kz.huanxung.cn

[D12] 查找元素下标
来源：http://kv.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://bx.nszjky.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ia.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kh.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vr.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ci.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://ri.9csxet.cn

Ruby: arr.index(x)
来源：http://mp.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://qy.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://rj.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ev.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nn.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://gq.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://yy.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zt.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uf.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fg.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fl.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://bg.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nh.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tg.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://gc.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://hv.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hj.huixinmuqiang.cn

Go:   // 手写循环
来源：http://yb.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ol.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ps.shtwfgs.cn

[D15] 去重
来源：http://xh.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rr.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://ea.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://qn.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://cm.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xn.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eb.asd995.cn

Ruby: arr.uniq
来源：http://bi.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://op.bjjhwx.cn

[D16] 求和与平均值
来源：http://kt.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oz.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fh.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rx.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bg.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://op.nszjky.cn

Go:   // 手写循环累加
来源：http://po.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qc.szsharing.cn

C#:   list.Sum();  list.Average()
来源：http://mm.jctech888.com.cn

[D17] 最大值与最小值
来源：http://ny.huanxung.cn

Py:   max(arr);  min(arr)
来源：http://ip.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://gq.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xb.lnxyls.cn

TS:   Math.max(...arr);
来源：http://ei.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://me.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://we.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://cx.colortex.cn

C#:   list.Max();  list.Min()
来源：http://et.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://px.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xg.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://ex.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hc.huanxung.cn

TS:   nested.flat();
来源：http://ff.colortex.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pt.hahajie.cn

Go:   // 手写双层循环
来源：http://yj.newstarts.cn

Ruby: nested.flatten
来源：http://zf.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://us.jctech888.com.cn

[D19] 按字段分组
来源：http://st.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zz.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nw.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vt.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://un.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gk.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://dq.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wg.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xu.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://ow.huixiangedu.cn

Py:   Counter(arr)
来源：http://bc.9csxet.cn

PHP:  array_count_values($arr);
来源：http://hd.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cl.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dx.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ai.yuntaijiaju.cn

Go:   // 手写 map[T]int
来源：http://wd.nicolike.cn


<!-- 参考信息 -->