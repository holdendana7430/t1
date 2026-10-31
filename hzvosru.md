代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hh.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rn.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kw.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rc.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ww.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ca.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lf.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ge.huixiangedu.cn

[C10] 变量作用域
来源：http://br.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://um.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gp.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gr.huixinmuqiang.cn

TS:   同 JS
来源：http://hn.hahajie.cn

Java: 方法内为块级作用域
来源：http://br.shtwfgs.cn

Go:   花括号块级作用域
来源：http://ut.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sp.shxzukj.cn

C#:   块级作用域
来源：http://nj.newstarts.cn

[C11] 模块导入与导出
来源：http://vn.yuntaijiaju.cn

Py:   from module import func
来源：http://zs.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ut.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jk.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zf.szxytkj.cn

Java: import java.util.List;
来源：http://qk.szsharing.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bf.hnjuh.cn

Ruby: require "json"; require_relative "./util"
来源：http://bq.panjiajie.cn

C#:   using System.Text;
来源：http://je.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://va.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://mz.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://qy.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://zd.hnjuh.cn

TS:   (() => { console.log("run"); })();
来源：http://ld.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lf.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://zg.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://uy.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hk.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://bd.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ui.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sh.huixiangedu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ti.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oc.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://eh.nszjky.cn

Go:   func add(a, b int) int
来源：http://tl.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jr.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kd.szxytkj.cn

[C14] 泛型函数
来源：http://ad.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jt.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://tb.szsharing.cn

JS:   // 无泛型
来源：http://zx.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qs.shxzukj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yg.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wo.shxzukj.cn

Ruby: # 无泛型
来源：http://er.newstarts.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://od.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://aa.hnjuh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ut.huixinmuqiang.cn

PHP:  [$a, $b] = $pair;
来源：http://bw.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://px.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dj.huanxung.cn

Java: // 无解构
来源：http://ot.bjjhwx.cn

Go:   // 无解构
来源：http://sj.nszjky.cn

Ruby: a, b = pair
来源：http://fl.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://wc.huanxung.cn

[C16] 函数 / 方法重载
来源：http://qo.haigaiapp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rm.muxihuayi.cn

PHP:  // 无重载
来源：http://ug.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://om.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://wj.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bp.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://ij.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://wt.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tu.jianghongdianzi.cn

================================================================================
来源：http://ca.jianghongdianzi.cn

D. 数组 / 列表 / 集合
来源：http://kq.colortex.cn

================================================================================
来源：http://kk.shxzukj.cn

[D01] 创建数组 / 列表
来源：http://jj.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pa.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oa.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uk.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vx.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dn.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://cb.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://pj.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ml.asd995.cn

[D02] 追加元素到末尾
来源：http://we.lnxyls.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xj.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rm.shtwfgs.cn

JS:   arr.push(4);
来源：http://th.hnjuh.cn

TS:   arr.push(4);
来源：http://al.bjjhwx.cn

Java: list.add(4);
来源：http://dw.hnjuh.cn

Go:   arr = append(arr, 4)
来源：http://cn.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://iz.wgjwhj.cn

C#:   list.Add(4);
来源：http://vp.asd995.cn

[D03] 在指定位置插入元素
来源：http://tg.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://hg.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wh.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://op.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://zk.huanxung.cn

Java: list.add(0, 0);
来源：http://tb.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ul.gzmigu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wk.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://ck.9csxet.cn

[D04] 删除元素
来源：http://yd.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lg.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fi.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qe.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://cn.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fe.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ve.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://az.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tl.bookmarksfly.cn

[D05] 访问与修改元素
来源：http://gi.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cl.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vt.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mj.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://yt.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://nv.huixiangedu.cn

Go:   arr[0]; arr[0] = 9
来源：http://hr.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pi.gzmigu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nx.shtwfgs.cn

[D06] 数组长度
来源：http://pu.9csxet.cn

Py:   len(arr)
来源：http://ur.jctech888.com.cn

PHP:  count($arr);
来源：http://kw.shxzskj.cn

JS:   arr.length
来源：http://ma.shxzukj.cn

TS:   arr.length
来源：http://md.haigaiapp.cn

Java: list.size();
来源：http://la.huixinmuqiang.cn

Go:   len(arr)
来源：http://ey.colortex.cn

Ruby: arr.length; arr.size
来源：http://xw.wgjwhj.cn

C#:   list.Count;
来源：http://yc.newstarts.cn

[D07] 切片 / 取子数组
来源：http://uc.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zg.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bz.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://nc.colortex.cn

TS:   arr.slice(1, 4);
来源：http://nl.colortex.cn

Java: list.subList(1, 4);
来源：http://wl.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://dd.panjiajie.cn

Ruby: arr[1, 3]
来源：http://iy.shxzukj.cn

C#:   list.GetRange(1, 3);
来源：http://nx.jctech888.com.cn

[D08] 合并两个数组
来源：http://tt.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://is.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://ot.shtwfgs.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pv.haigaiapp.cn

TS:   [...a, ...b];
来源：http://ju.yuexingan06.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mz.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://hd.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://zl.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://mx.newstarts.cn

[D09] 排序（升序）
来源：http://ur.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://aq.gzmigu.cn

PHP:  sort($arr);
来源：http://xt.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ma.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fo.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ag.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qe.haigaiapp.cn

Ruby: arr.sort
来源：http://nt.yuexingan06.cn

C#:   list.Sort();
来源：http://ws.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rk.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nx.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ta.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jd.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mq.szsharing.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ld.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pf.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hb.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bv.yuexingan06.cn

[D11] 反转数组
来源：http://sg.gzmigu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kx.wgjwhj.cn

PHP:  array_reverse($arr);
来源：http://on.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ac.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://hi.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://rx.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://tw.asd995.cn

Ruby: arr.reverse
来源：http://ps.huixiangedu.cn

C#:   list.Reverse();
来源：http://hu.hnjuh.cn

[D12] 查找元素下标
来源：http://gb.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://kk.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tv.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tw.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lj.haigaiapp.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eh.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://um.colortex.cn

Ruby: arr.index(x)
来源：http://ws.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://he.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://ns.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kj.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cf.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://hx.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://lg.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://je.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://er.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xv.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vh.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://ui.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lw.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vv.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://st.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://rm.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ie.gzmigu.cn

Go:   // 手写循环
来源：http://jk.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fy.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rp.bookmarksfly.cn

[D15] 去重
来源：http://xt.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dl.asd995.cn

PHP:  array_unique($arr);
来源：http://pc.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://aw.9csxet.cn

TS:   [...new Set(arr)]
来源：http://ap.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uf.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rl.hahajie.cn

Ruby: arr.uniq
来源：http://aq.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://vq.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://ql.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cf.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mh.hnjuh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kx.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dh.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ws.huixiangedu.cn

Go:   // 手写循环累加
来源：http://no.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ao.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://el.muxihuayi.cn

[D17] 最大值与最小值
来源：http://yp.hnjuh.cn

Py:   max(arr);  min(arr)
来源：http://zo.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://iu.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pz.shxzukj.cn

TS:   Math.max(...arr);
来源：http://xe.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hf.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://su.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://li.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://ls.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://hl.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pu.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://ln.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hh.bookmarksfly.cn

TS:   nested.flat();
来源：http://fb.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://br.gzmigu.cn

Go:   // 手写双层循环
来源：http://ok.shxzskj.cn

Ruby: nested.flatten
来源：http://ft.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://id.asd995.cn

[D19] 按字段分组
来源：http://pv.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ns.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lz.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sr.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://on.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gh.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://pm.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nm.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qw.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://gc.huanxung.cn

Py:   Counter(arr)
来源：http://ec.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://qb.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tz.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ea.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pa.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://lw.huixiangedu.cn

Ruby: arr.tally
来源：http://np.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cl.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://bj.9csxet.cn

Py:   x in arr
来源：http://cw.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://bs.lnxyls.cn

JS:   arr.includes(x)
来源：http://no.lnxyls.cn

TS:   arr.includes(x)
来源：http://ol.hahajie.cn

Java: list.contains(x)
来源：http://cz.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://ol.hnjuh.cn

Ruby: arr.include?(x)
来源：http://nj.panjiajie.cn

C#:   list.Contains(x)
来源：http://jy.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://lj.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eo.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fb.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ey.asd995.cn

TS:   [...arr];
来源：http://ee.asd995.cn

Java: new ArrayList<>(list);
来源：http://gn.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tb.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://uy.521024.cn

C#:   new List<int>(list);
来源：http://wm.gzmigu.cn

[D23] reduce 累积计算
来源：http://vm.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ne.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nx.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wv.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://th.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ym.nszjky.cn

Go:   // 手写循环
来源：http://qc.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ql.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mc.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://ja.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fc.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iw.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ts.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://go.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xy.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://og.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://au.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://da.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://fi.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ms.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pf.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cn.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lk.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gc.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iv.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tr.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ox.gzmigu.cn

[D26] 数组转字符串
来源：http://ep.muxihuayi.cn


<!-- 参考信息 -->