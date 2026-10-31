代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://vp.huixiangedu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tk.hnjuh.cn

[C04] 命名参数 / 关键字参数
来源：http://zb.szsharing.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zj.nicolike.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bd.shtwfgs.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ms.haigaiapp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://va.shxzukj.cn

Java: // 无：用 Builder 模式或 record
来源：http://cc.chemitech.net.cn

Go:   // 无：用配置结构体参数
来源：http://xe.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://gh.gzmigu.cn

C#:   f(a: 1, b: 2)
来源：http://sh.muxihuayi.cn

[C05] 返回多个值
来源：http://cv.newstarts.cn

Py:   return a, b
来源：http://dt.lnxyls.cn

PHP:  return [$a, $b];
来源：http://hd.9csxet.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://by.hnjuh.cn

TS:   return { a, b };
来源：http://ga.szsharing.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ny.nszjky.cn

Go:   return a, b
来源：http://cm.wgjwhj.cn

Ruby: return a, b
来源：http://rz.bjjhwx.cn

C#:   return (a, b);              // ValueTuple
来源：http://pv.yuntaijiaju.cn

[C06] 匿名函数 / lambda
来源：http://ld.huixinmuqiang.cn

Py:   square = lambda x: x * x
来源：http://ok.newstarts.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nq.szxytkj.cn

JS:   const square = x => x * x;
来源：http://ev.shtwfgs.cn

TS:   const square = (x: number): number => x * x;
来源：http://xh.huanxung.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uc.hahajie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hn.jianghongdianzi.cn

Ruby: square = ->(x) { x * x }
来源：http://aa.bjjhwx.cn

C#:   Func<int, int> square = x => x * x;
来源：http://jd.szsharing.cn

[C07] 把函数作为参数传入
来源：http://ik.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kc.szxytkj.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jt.gzmigu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oh.haigaiapp.cn

TS:   arr.map(String)
来源：http://ch.jianghongdianzi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://il.newstarts.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mr.huanxung.cn

Ruby: arr.map(&:upcase)
来源：http://yv.9csxet.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kq.bjjhwx.cn

[C08] 闭包
来源：http://my.panjiajie.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hr.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rl.yuntaijiaju.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xj.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kr.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cv.asd995.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ax.nicolike.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ub.521024.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ud.shtwfgs.cn

[C09] 递归
来源：http://sd.huixinmuqiang.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cv.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cj.asd995.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bu.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.hnjuh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pn.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ka.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ei.asd995.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sl.huixinmuqiang.cn

[C10] 变量作用域
来源：http://py.jianghongdianzi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tn.nszjky.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dd.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qt.asd995.cn

TS:   同 JS
来源：http://pn.shxzukj.cn

Java: 方法内为块级作用域
来源：http://oo.shxzskj.cn

Go:   花括号块级作用域
来源：http://lo.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ca.asd995.cn

C#:   块级作用域
来源：http://wd.wgjwhj.cn

[C11] 模块导入与导出
来源：http://dm.wgjwhj.cn

Py:   from module import func
来源：http://uq.shxzskj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zf.shtwfgs.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vt.9csxet.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dr.jianghongdianzi.cn

Java: import java.util.List;
来源：http://fg.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uh.yuexingan06.cn

Ruby: require "json"; require_relative "./util"
来源：http://dm.huixiangedu.cn

C#:   using System.Text;
来源：http://og.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://va.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://nk.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://bd.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://pg.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://jo.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sh.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://zy.nszjky.cn

Ruby: -> { puts "run" }.call
来源：http://qy.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hn.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ws.hahajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zd.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kd.hahajie.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xl.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mn.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ty.hahajie.cn

Go:   func add(a, b int) int
来源：http://zg.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zd.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://wv.yuexingan06.cn

[C14] 泛型函数
来源：http://ua.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jf.colortex.cn

PHP:  // 无泛型
来源：http://jx.szsharing.cn

JS:   // 无泛型
来源：http://gz.panjiajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qo.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mt.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hb.hnjuh.cn

Ruby: # 无泛型
来源：http://pu.hnjuh.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wb.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://zj.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wt.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://uv.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hk.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hr.asd995.cn

Java: // 无解构
来源：http://wc.haigaiapp.cn

Go:   // 无解构
来源：http://nn.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://im.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://lh.jianghongdianzi.cn

[C16] 函数 / 方法重载
来源：http://ya.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://px.panjiajie.cn

PHP:  // 无重载
来源：http://gz.wgjwhj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qs.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://bc.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gx.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://jm.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://lx.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gk.haigaiapp.cn

================================================================================
来源：http://ds.shxzskj.cn

D. 数组 / 列表 / 集合
来源：http://wo.hnjuh.cn

================================================================================
来源：http://dv.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://xt.521024.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ic.yuntaijiaju.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ol.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ff.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sv.bookmarksfly.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nj.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://dh.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://iv.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rd.9csxet.cn

[D02] 追加元素到末尾
来源：http://zj.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kw.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ax.haigaiapp.cn

JS:   arr.push(4);
来源：http://rn.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://io.yuntaijiaju.cn

Java: list.add(4);
来源：http://bu.colortex.cn

Go:   arr = append(arr, 4)
来源：http://ah.muxihuayi.cn

Ruby: arr << 4; arr.push(5)
来源：http://jc.colortex.cn

C#:   list.Add(4);
来源：http://ae.nszjky.cn

[D03] 在指定位置插入元素
来源：http://qe.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://qs.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ao.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wx.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://sv.bjjhwx.cn

Java: list.add(0, 0);
来源：http://ex.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bg.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wz.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://wk.huanxung.cn

[D04] 删除元素
来源：http://mg.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ek.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pw.colortex.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ck.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://gp.jctech888.com.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hw.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://av.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hb.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rg.newstarts.cn

[D05] 访问与修改元素
来源：http://ei.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pj.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ka.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zw.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://tz.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://bs.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://yk.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vf.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bc.bookmarksfly.cn

[D06] 数组长度
来源：http://np.chemitech.net.cn

Py:   len(arr)
来源：http://fd.bjjhwx.cn

PHP:  count($arr);
来源：http://rf.newstarts.cn

JS:   arr.length
来源：http://pt.bjjhwx.cn

TS:   arr.length
来源：http://mi.chemitech.net.cn

Java: list.size();
来源：http://sr.bjjhwx.cn

Go:   len(arr)
来源：http://vd.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://qk.yuntaijiaju.cn

C#:   list.Count;
来源：http://qf.9csxet.cn

[D07] 切片 / 取子数组
来源：http://jg.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dq.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xp.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ul.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ni.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://zn.yuexingan06.cn

Go:   arr[1:4]
来源：http://ht.huanxung.cn

Ruby: arr[1, 3]
来源：http://hd.gzmigu.cn

C#:   list.GetRange(1, 3);
来源：http://xy.9csxet.cn

[D08] 合并两个数组
来源：http://jz.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://fb.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://fr.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gs.wgjwhj.cn

TS:   [...a, ...b];
来源：http://rt.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rg.bookmarksfly.cn

Go:   append(a, b...)
来源：http://bh.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://yd.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://dc.lnxyls.cn

[D09] 排序（升序）
来源：http://zi.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://op.huixiangedu.cn

PHP:  sort($arr);
来源：http://ur.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bx.gzmigu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lk.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ha.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gg.521024.cn

Ruby: arr.sort
来源：http://xp.huixinmuqiang.cn

C#:   list.Sort();
来源：http://sb.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://es.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vl.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://df.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sd.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lr.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ma.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sj.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yp.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://st.huixinmuqiang.cn

[D11] 反转数组
来源：http://qo.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gu.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://gl.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eu.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://pd.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://ed.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://dw.shxzukj.cn

Ruby: arr.reverse
来源：http://gb.huanxung.cn

C#:   list.Reverse();
来源：http://xy.521024.cn

[D12] 查找元素下标
来源：http://jj.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://fd.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://la.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://je.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sn.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ro.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://rw.huixiangedu.cn

Ruby: arr.index(x)
来源：http://fj.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://wk.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://wz.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://if.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vm.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://eu.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://zk.jctech888.com.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xa.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wx.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://aw.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bp.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://vu.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jy.huixinmuqiang.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nq.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://tj.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://lq.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://du.chemitech.net.cn

Go:   // 手写循环
来源：http://hj.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ul.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zv.asd995.cn

[D15] 去重
来源：http://fx.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pw.colortex.cn

PHP:  array_unique($arr);
来源：http://tv.newstarts.cn

JS:   [...new Set(arr)]
来源：http://ty.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://lv.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uw.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jr.521024.cn

Ruby: arr.uniq
来源：http://rs.521024.cn

C#:   list.Distinct().ToList()
来源：http://vh.colortex.cn

[D16] 求和与平均值
来源：http://hc.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zo.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ka.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ct.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zg.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xc.szsharing.cn

Go:   // 手写循环累加
来源：http://ve.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xp.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://ij.newstarts.cn

[D17] 最大值与最小值
来源：http://rq.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://ge.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://lm.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oh.hnjuh.cn

TS:   Math.max(...arr);
来源：http://jq.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ds.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rf.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ap.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://ty.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://xw.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ea.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://kc.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://li.lnxyls.cn

TS:   nested.flat();
来源：http://xv.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hl.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://so.panjiajie.cn

Ruby: nested.flatten
来源：http://bn.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jh.jianghongdianzi.cn

[D19] 按字段分组
来源：http://fm.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jo.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vq.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ot.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xe.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fy.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://uc.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rs.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ub.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://ni.hahajie.cn

Py:   Counter(arr)
来源：http://vm.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://jr.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hu.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uy.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xl.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://nr.szsharing.cn


<!-- 参考信息 -->