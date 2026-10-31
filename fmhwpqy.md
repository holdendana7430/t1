代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://ps.newstarts.cn

Ruby: f(a: 1, b: 2)
来源：http://qt.szsharing.cn

C#:   f(a: 1, b: 2)
来源：http://up.colortex.cn

[C05] 返回多个值
来源：http://hz.huixiangedu.cn

Py:   return a, b
来源：http://lg.nicolike.cn

PHP:  return [$a, $b];
来源：http://vj.colortex.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://st.szxytkj.cn

TS:   return { a, b };
来源：http://tk.shxzskj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yt.haigaiapp.cn

Go:   return a, b
来源：http://xs.colortex.cn

Ruby: return a, b
来源：http://se.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://ix.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://xm.gzmigu.cn

Py:   square = lambda x: x * x
来源：http://sr.haigaiapp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://st.colortex.cn

JS:   const square = x => x * x;
来源：http://ar.huixinmuqiang.cn

TS:   const square = (x: number): number => x * x;
来源：http://wg.9csxet.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ix.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nm.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://cf.hahajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rx.panjiajie.cn

[C07] 把函数作为参数传入
来源：http://pf.muxihuayi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vj.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mk.shtwfgs.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mk.521024.cn

TS:   arr.map(String)
来源：http://xc.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eh.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ub.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://zy.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zr.521024.cn

[C08] 闭包
来源：http://ey.shxzukj.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ao.hahajie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pt.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eu.huanxung.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ah.gzmigu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pv.szxytkj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nk.nszjky.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://og.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qs.muxihuayi.cn

[C09] 递归
来源：http://kr.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://aa.huanxung.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mw.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gh.szsharing.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ci.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jv.wgjwhj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cx.newstarts.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ew.bookmarksfly.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ib.chemitech.net.cn

[C10] 变量作用域
来源：http://ai.shxzukj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zq.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lj.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dg.shxzukj.cn

TS:   同 JS
来源：http://ll.haigaiapp.cn

Java: 方法内为块级作用域
来源：http://um.asd995.cn

Go:   花括号块级作用域
来源：http://vo.szxytkj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uz.wgjwhj.cn

C#:   块级作用域
来源：http://bu.chemitech.net.cn

[C11] 模块导入与导出
来源：http://zx.521024.cn

Py:   from module import func
来源：http://ua.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://te.hnjuh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bp.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wv.huixinmuqiang.cn

Java: import java.util.List;
来源：http://ck.jianghongdianzi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zy.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://fg.bjjhwx.cn

C#:   using System.Text;
来源：http://gb.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://rx.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://fh.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://rj.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://pf.haigaiapp.cn

TS:   (() => { console.log("run"); })();
来源：http://zr.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ah.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://za.shxzukj.cn

Ruby: -> { puts "run" }.call
来源：http://hg.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://si.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://vx.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cy.asd995.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sm.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rt.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zm.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aa.bjjhwx.cn

Go:   func add(a, b int) int
来源：http://hj.lnxyls.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gn.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ug.huanxung.cn

[C14] 泛型函数
来源：http://yh.bjjhwx.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ln.nicolike.cn

PHP:  // 无泛型
来源：http://ag.yuntaijiaju.cn

JS:   // 无泛型
来源：http://cq.bjjhwx.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ng.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xs.nszjky.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mg.shtwfgs.cn

Ruby: # 无泛型
来源：http://xz.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nb.hahajie.cn

[C15] 解构 / 展开参数
来源：http://wd.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rl.bookmarksfly.cn

PHP:  [$a, $b] = $pair;
来源：http://ek.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yx.hnjuh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sm.jctech888.com.cn

Java: // 无解构
来源：http://rd.shtwfgs.cn

Go:   // 无解构
来源：http://tp.chemitech.net.cn

Ruby: a, b = pair
来源：http://yy.huanxung.cn

C#:   var (a, b) = pair;
来源：http://na.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://rf.shtwfgs.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vd.yuexingan06.cn

PHP:  // 无重载
来源：http://rv.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xo.yuexingan06.cn

TS:   // 用联合类型或重载签名声明
来源：http://kx.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dx.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://sz.szsharing.cn

Ruby: # 无重载：靠动态参数
来源：http://gl.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lx.bjjhwx.cn

================================================================================
来源：http://ez.bookmarksfly.cn

D. 数组 / 列表 / 集合
来源：http://yi.colortex.cn

================================================================================
来源：http://ql.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://vw.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://uy.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uj.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cq.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ok.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rw.nszjky.cn

Go:   arr := []int{1, 2, 3}
来源：http://jq.nicolike.cn

Ruby: arr = [1, 2, 3]
来源：http://ol.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dg.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ux.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nv.szsharing.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rj.newstarts.cn

JS:   arr.push(4);
来源：http://tg.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://ig.yuexingan06.cn

Java: list.add(4);
来源：http://hl.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://my.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://ig.colortex.cn

C#:   list.Add(4);
来源：http://px.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://wg.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://zt.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mb.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gz.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://ol.521024.cn

Java: list.add(0, 0);
来源：http://qb.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pu.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yl.521024.cn

C#:   list.Insert(0, 0);
来源：http://se.newstarts.cn

[D04] 删除元素
来源：http://pz.yuntaijiaju.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gm.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sp.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ds.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://kh.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ir.gzmigu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jz.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gb.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hg.shtwfgs.cn

[D05] 访问与修改元素
来源：http://kh.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ag.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mz.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ty.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://cy.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://qq.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://fg.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://db.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://od.hahajie.cn

[D06] 数组长度
来源：http://jd.lnxyls.cn

Py:   len(arr)
来源：http://hg.yuexingan06.cn

PHP:  count($arr);
来源：http://xk.szsharing.cn

JS:   arr.length
来源：http://hc.nszjky.cn

TS:   arr.length
来源：http://ta.nicolike.cn

Java: list.size();
来源：http://io.9csxet.cn

Go:   len(arr)
来源：http://lg.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://kv.bjjhwx.cn

C#:   list.Count;
来源：http://fv.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://hk.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mf.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lc.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://hp.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://go.huanxung.cn

Java: list.subList(1, 4);
来源：http://yp.hnjuh.cn

Go:   arr[1:4]
来源：http://lx.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://zy.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://zk.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://rg.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://yi.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://yw.haigaiapp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qy.shxzukj.cn

TS:   [...a, ...b];
来源：http://cb.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fl.panjiajie.cn

Go:   append(a, b...)
来源：http://ne.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://kq.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://la.wgjwhj.cn

[D09] 排序（升序）
来源：http://gq.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rx.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://cs.bjjhwx.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://so.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://os.asd995.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xe.521024.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oj.newstarts.cn

Ruby: arr.sort
来源：http://re.huixinmuqiang.cn

C#:   list.Sort();
来源：http://wu.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cc.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qm.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uc.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nw.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ao.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gy.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vj.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ee.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fn.jianghongdianzi.cn

[D11] 反转数组
来源：http://px.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jm.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://ie.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xw.shxzukj.cn

TS:   [...arr].reverse();
来源：http://wv.asd995.cn

Java: Collections.reverse(list);
来源：http://fx.colortex.cn

Go:   slices.Reverse(arr)
来源：http://rp.nszjky.cn

Ruby: arr.reverse
来源：http://wb.panjiajie.cn

C#:   list.Reverse();
来源：http://oi.lnxyls.cn

[D12] 查找元素下标
来源：http://jv.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://iq.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ur.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zv.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sz.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bz.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://sk.jctech888.com.cn

Ruby: arr.index(x)
来源：http://wt.nszjky.cn

C#:   list.IndexOf(x);
来源：http://ci.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://gc.colortex.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ma.jctech888.com.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ax.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://xz.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://dc.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rv.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jn.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rd.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://to.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://zr.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iu.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pk.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://uk.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://nw.asd995.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xe.hnjuh.cn

Go:   // 手写循环
来源：http://bb.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vz.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dh.newstarts.cn

[D15] 去重
来源：http://dj.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fe.asd995.cn

PHP:  array_unique($arr);
来源：http://va.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://no.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://gs.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dj.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iy.huixiangedu.cn

Ruby: arr.uniq
来源：http://to.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://eu.nszjky.cn

[D16] 求和与平均值
来源：http://lj.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xy.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bl.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sq.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://di.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fn.lnxyls.cn

Go:   // 手写循环累加
来源：http://fo.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vj.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://tk.haigaiapp.cn

[D17] 最大值与最小值
来源：http://ag.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://vi.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://hq.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ve.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://pn.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rj.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kr.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://il.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://ob.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://co.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://no.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://oo.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pb.shxzskj.cn

TS:   nested.flat();
来源：http://fz.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ln.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://zh.asd995.cn

Ruby: nested.flatten
来源：http://af.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mv.gzmigu.cn

[D19] 按字段分组
来源：http://xc.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xp.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yw.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qc.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yp.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pu.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://gk.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qe.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vc.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://tb.panjiajie.cn

Py:   Counter(arr)
来源：http://pn.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://gr.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mq.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tg.521024.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mf.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ad.yuexingan06.cn

Ruby: arr.tally
来源：http://uq.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ga.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://mc.huixiangedu.cn

Py:   x in arr
来源：http://ix.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://rb.yuexingan06.cn

JS:   arr.includes(x)
来源：http://sr.hahajie.cn

TS:   arr.includes(x)
来源：http://ub.gzmigu.cn

Java: list.contains(x)
来源：http://hv.lnxyls.cn


<!-- 参考信息 -->