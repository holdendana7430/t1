代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xf.521024.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tf.jctech888.com.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cd.huixiangedu.cn

Java: // 无：用 Builder 模式或 record
来源：http://bc.jianghongdianzi.cn

Go:   // 无：用配置结构体参数
来源：http://xf.shxzukj.cn

Ruby: f(a: 1, b: 2)
来源：http://cm.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://vy.shxzskj.cn

[C05] 返回多个值
来源：http://xs.panjiajie.cn

Py:   return a, b
来源：http://hf.shxzskj.cn

PHP:  return [$a, $b];
来源：http://yv.szxytkj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://li.colortex.cn

TS:   return { a, b };
来源：http://xo.nszjky.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mt.shxzukj.cn

Go:   return a, b
来源：http://gt.chemitech.net.cn

Ruby: return a, b
来源：http://oy.hahajie.cn

C#:   return (a, b);              // ValueTuple
来源：http://dp.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://ci.hahajie.cn

Py:   square = lambda x: x * x
来源：http://iq.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://oi.521024.cn

JS:   const square = x => x * x;
来源：http://fv.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://wr.lnxyls.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jx.huixinmuqiang.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jb.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://ow.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lb.yuexingan06.cn

[C07] 把函数作为参数传入
来源：http://tb.9csxet.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sj.shxzukj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rg.lnxyls.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://in.szxytkj.cn

TS:   arr.map(String)
来源：http://iz.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dx.jianghongdianzi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ec.jianghongdianzi.cn

Ruby: arr.map(&:upcase)
来源：http://iq.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zb.wgjwhj.cn

[C08] 闭包
来源：http://kh.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vi.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wa.shxzskj.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eu.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pc.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wl.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yz.newstarts.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://um.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pm.bjjhwx.cn

[C09] 递归
来源：http://ay.bookmarksfly.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mu.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ay.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://un.muxihuayi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hm.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bu.newstarts.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://op.huixiangedu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pk.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bm.9csxet.cn

[C10] 变量作用域
来源：http://zd.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hi.panjiajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pm.panjiajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qa.shxzskj.cn

TS:   同 JS
来源：http://pt.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://su.huixinmuqiang.cn

Go:   花括号块级作用域
来源：http://gs.haigaiapp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nc.lnxyls.cn

C#:   块级作用域
来源：http://xv.szxytkj.cn

[C11] 模块导入与导出
来源：http://zv.521024.cn

Py:   from module import func
来源：http://zi.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rb.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://od.shxzukj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wc.nszjky.cn

Java: import java.util.List;
来源：http://of.bookmarksfly.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lb.haigaiapp.cn

Ruby: require "json"; require_relative "./util"
来源：http://zl.muxihuayi.cn

C#:   using System.Text;
来源：http://ck.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://ml.521024.cn

Py:   (lambda: print("run"))()
来源：http://tf.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://ls.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://qa.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://bv.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ul.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://dm.jctech888.com.cn

Ruby: -> { puts "run" }.call
来源：http://md.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ov.521024.cn

[C13] 类型声明 / 类型注解
来源：http://ma.szsharing.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yb.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nc.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vo.shtwfgs.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://li.gzmigu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dn.asd995.cn

Go:   func add(a, b int) int
来源：http://vy.haigaiapp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sy.colortex.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hx.asd995.cn

[C14] 泛型函数
来源：http://dm.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ws.jianghongdianzi.cn

PHP:  // 无泛型
来源：http://wb.panjiajie.cn

JS:   // 无泛型
来源：http://in.shxzskj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zw.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ma.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://go.haigaiapp.cn

Ruby: # 无泛型
来源：http://bc.gzmigu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wx.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://bl.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ou.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://xc.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jq.yuexingan06.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kt.colortex.cn

Java: // 无解构
来源：http://lk.haigaiapp.cn

Go:   // 无解构
来源：http://zz.shtwfgs.cn

Ruby: a, b = pair
来源：http://jn.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://wt.asd995.cn

[C16] 函数 / 方法重载
来源：http://iz.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uj.haigaiapp.cn

PHP:  // 无重载
来源：http://nu.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ad.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://vc.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bd.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://uw.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://hq.chemitech.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jy.lnxyls.cn

================================================================================
来源：http://py.521024.cn

D. 数组 / 列表 / 集合
来源：http://oc.shxzskj.cn

================================================================================
来源：http://kh.hahajie.cn

[D01] 创建数组 / 列表
来源：http://np.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zq.szxytkj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mi.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hw.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vg.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ak.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://sl.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://hr.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://md.panjiajie.cn

[D02] 追加元素到末尾
来源：http://yj.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rv.gzmigu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hp.gzmigu.cn

JS:   arr.push(4);
来源：http://ou.chemitech.net.cn

TS:   arr.push(4);
来源：http://ra.yuexingan06.cn

Java: list.add(4);
来源：http://eh.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://nh.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://rr.huixiangedu.cn

C#:   list.Add(4);
来源：http://nu.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://pv.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://su.huanxung.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://su.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gn.shxzukj.cn

TS:   arr.splice(0, 0, 0);
来源：http://ta.chemitech.net.cn

Java: list.add(0, 0);
来源：http://cg.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vc.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rz.jctech888.com.cn

C#:   list.Insert(0, 0);
来源：http://ba.huixinmuqiang.cn

[D04] 删除元素
来源：http://fb.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iz.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tn.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sf.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://vi.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ae.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dc.muxihuayi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lc.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bd.hahajie.cn

[D05] 访问与修改元素
来源：http://zi.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zw.bookmarksfly.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://at.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ol.chemitech.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://tg.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://th.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://xk.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tn.bookmarksfly.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oe.yuexingan06.cn

[D06] 数组长度
来源：http://uk.panjiajie.cn

Py:   len(arr)
来源：http://ua.bookmarksfly.cn

PHP:  count($arr);
来源：http://eh.haigaiapp.cn

JS:   arr.length
来源：http://sp.jianghongdianzi.cn

TS:   arr.length
来源：http://er.szxytkj.cn

Java: list.size();
来源：http://bh.szxytkj.cn

Go:   len(arr)
来源：http://lc.newstarts.cn

Ruby: arr.length; arr.size
来源：http://to.521024.cn

C#:   list.Count;
来源：http://rv.nszjky.cn

[D07] 切片 / 取子数组
来源：http://if.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uq.shtwfgs.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gs.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://wm.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://er.szsharing.cn

Java: list.subList(1, 4);
来源：http://fa.chemitech.net.cn

Go:   arr[1:4]
来源：http://jg.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://xf.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://yk.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://yd.szsharing.cn

Py:   a + b;  a.extend(b)
来源：http://oc.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://lx.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ah.shxzukj.cn

TS:   [...a, ...b];
来源：http://ef.panjiajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bb.shtwfgs.cn

Go:   append(a, b...)
来源：http://lb.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://sg.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://os.szsharing.cn

[D09] 排序（升序）
来源：http://cn.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://wj.shxzukj.cn

PHP:  sort($arr);
来源：http://zx.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ui.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qw.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rq.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mz.huixinmuqiang.cn

Ruby: arr.sort
来源：http://rg.nicolike.cn

C#:   list.Sort();
来源：http://wv.muxihuayi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nv.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gq.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wk.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ah.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hf.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ty.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nt.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kr.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bx.bookmarksfly.cn

[D11] 反转数组
来源：http://lm.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cf.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://fs.newstarts.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pj.asd995.cn

TS:   [...arr].reverse();
来源：http://zg.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://ny.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://dj.9csxet.cn

Ruby: arr.reverse
来源：http://mn.nszjky.cn

C#:   list.Reverse();
来源：http://fx.lnxyls.cn

[D12] 查找元素下标
来源：http://op.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://cg.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ra.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bq.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qd.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pm.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://zc.lnxyls.cn

Ruby: arr.index(x)
来源：http://sh.9csxet.cn

C#:   list.IndexOf(x);
来源：http://zl.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://if.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rh.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://db.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://sh.bjjhwx.cn

TS:   arr.filter(x => x > 3)
来源：http://id.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lj.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hl.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oe.huixinmuqiang.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ki.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://bw.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://re.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ev.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://xt.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://iw.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tl.521024.cn

Go:   // 手写循环
来源：http://wh.shxzskj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ui.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sg.bjjhwx.cn

[D15] 去重
来源：http://eq.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qt.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://rj.huanxung.cn

JS:   [...new Set(arr)]
来源：http://hl.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://hl.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qq.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rs.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://ka.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://xe.hahajie.cn

[D16] 求和与平均值
来源：http://dn.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hm.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sw.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nq.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cq.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://et.huixiangedu.cn

Go:   // 手写循环累加
来源：http://me.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rc.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://so.hahajie.cn

[D17] 最大值与最小值
来源：http://ms.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://ka.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://wz.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wl.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://yo.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zq.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lh.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://rr.asd995.cn

C#:   list.Max();  list.Min()
来源：http://py.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://hj.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dl.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://pp.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ov.nszjky.cn

TS:   nested.flat();
来源：http://ng.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jn.nszjky.cn

Go:   // 手写双层循环
来源：http://wl.chemitech.net.cn

Ruby: nested.flatten
来源：http://au.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ym.jctech888.com.cn

[D19] 按字段分组
来源：http://dh.nicolike.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qz.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xv.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ph.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://be.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wn.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://tn.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dl.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ym.asd995.cn

[D20] 统计每个元素出现次数
来源：http://cj.szsharing.cn

Py:   Counter(arr)
来源：http://gk.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://fh.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yw.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cy.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mb.nicolike.cn

Go:   // 手写 map[T]int
来源：http://xb.bjjhwx.cn

Ruby: arr.tally
来源：http://hz.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dn.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://vl.haigaiapp.cn

Py:   x in arr
来源：http://yc.huixiangedu.cn


<!-- 参考信息 -->