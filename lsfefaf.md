代发 wailian999

C#:   块级作用域
来源：http://kn.huixinmuqiang.cn

[C11] 模块导入与导出
来源：http://ky.bjjhwx.cn

Py:   from module import func
来源：http://vv.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jx.bookmarksfly.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://nm.nicolike.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gv.colortex.cn

Java: import java.util.List;
来源：http://pa.gzmigu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hb.wgjwhj.cn

Ruby: require "json"; require_relative "./util"
来源：http://at.9csxet.cn

C#:   using System.Text;
来源：http://zd.nicolike.cn

[C12] 立即执行函数 IIFE
来源：http://gf.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://tp.haigaiapp.cn

PHP:  (function () { echo "run"; })();
来源：http://qn.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://kx.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://kp.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wh.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://ol.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://bz.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ue.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://cf.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xg.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vq.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fl.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vz.jianghongdianzi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gs.asd995.cn

Go:   func add(a, b int) int
来源：http://pr.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pi.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://pk.huixinmuqiang.cn

[C14] 泛型函数
来源：http://ri.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oo.szxytkj.cn

PHP:  // 无泛型
来源：http://am.shxzskj.cn

JS:   // 无泛型
来源：http://dw.wgjwhj.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ba.colortex.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lf.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qd.huixiangedu.cn

Ruby: # 无泛型
来源：http://jx.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wg.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://dk.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kf.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://dn.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dx.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wt.chemitech.net.cn

Java: // 无解构
来源：http://ho.newstarts.cn

Go:   // 无解构
来源：http://pm.jctech888.com.cn

Ruby: a, b = pair
来源：http://dv.nicolike.cn

C#:   var (a, b) = pair;
来源：http://zu.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://oo.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tx.bookmarksfly.cn

PHP:  // 无重载
来源：http://xe.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jb.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://ck.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yp.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://vn.nszjky.cn

Ruby: # 无重载：靠动态参数
来源：http://oa.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ft.huixiangedu.cn

================================================================================
来源：http://ja.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://jn.bookmarksfly.cn

================================================================================
来源：http://ul.chemitech.net.cn

[D01] 创建数组 / 列表
来源：http://tk.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yq.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gl.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mo.shtwfgs.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yt.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://su.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://vv.hnjuh.cn

Ruby: arr = [1, 2, 3]
来源：http://bg.szxytkj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ns.gzmigu.cn

[D02] 追加元素到末尾
来源：http://ow.nszjky.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pm.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gr.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://tg.haigaiapp.cn

TS:   arr.push(4);
来源：http://zp.huanxung.cn

Java: list.add(4);
来源：http://mg.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://mt.yuntaijiaju.cn

Ruby: arr << 4; arr.push(5)
来源：http://ci.yuntaijiaju.cn

C#:   list.Add(4);
来源：http://nh.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://uh.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://pr.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eb.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qc.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://ny.huixiangedu.cn

Java: list.add(0, 0);
来源：http://xl.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kr.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vw.asd995.cn

C#:   list.Insert(0, 0);
来源：http://rh.chemitech.net.cn

[D04] 删除元素
来源：http://ri.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pi.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://za.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://je.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://jt.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://io.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pj.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dk.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://iw.bjjhwx.cn

[D05] 访问与修改元素
来源：http://ux.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zy.yuexingan06.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ay.huixinmuqiang.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zb.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://bf.bookmarksfly.cn

Java: list.get(0); list.set(0, 9);
来源：http://jo.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://qk.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bf.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dp.shxzskj.cn

[D06] 数组长度
来源：http://zu.muxihuayi.cn

Py:   len(arr)
来源：http://ap.nicolike.cn

PHP:  count($arr);
来源：http://vr.szsharing.cn

JS:   arr.length
来源：http://dd.nicolike.cn

TS:   arr.length
来源：http://yu.9csxet.cn

Java: list.size();
来源：http://my.jianghongdianzi.cn

Go:   len(arr)
来源：http://gz.hahajie.cn

Ruby: arr.length; arr.size
来源：http://mv.hahajie.cn

C#:   list.Count;
来源：http://nj.bjjhwx.cn

[D07] 切片 / 取子数组
来源：http://jd.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rz.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rz.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://ng.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://yc.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://ev.wgjwhj.cn

Go:   arr[1:4]
来源：http://vc.nszjky.cn

Ruby: arr[1, 3]
来源：http://mj.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://dh.nicolike.cn

[D08] 合并两个数组
来源：http://fj.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://vu.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://np.muxihuayi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ym.szxytkj.cn

TS:   [...a, ...b];
来源：http://ph.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lu.colortex.cn

Go:   append(a, b...)
来源：http://oq.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://dw.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://ww.wgjwhj.cn

[D09] 排序（升序）
来源：http://rl.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://dz.gzmigu.cn

PHP:  sort($arr);
来源：http://kj.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gu.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lp.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mm.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nq.hnjuh.cn

Ruby: arr.sort
来源：http://ck.haigaiapp.cn

C#:   list.Sort();
来源：http://hr.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zi.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fr.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yq.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zj.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bd.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wi.yuntaijiaju.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://du.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bw.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ei.shxzukj.cn

[D11] 反转数组
来源：http://db.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zh.huanxung.cn

PHP:  array_reverse($arr);
来源：http://wy.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gq.szsharing.cn

TS:   [...arr].reverse();
来源：http://qd.colortex.cn

Java: Collections.reverse(list);
来源：http://sr.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://wq.huixiangedu.cn

Ruby: arr.reverse
来源：http://wz.hnjuh.cn

C#:   list.Reverse();
来源：http://fn.hnjuh.cn

[D12] 查找元素下标
来源：http://zq.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://if.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pe.haigaiapp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ef.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mx.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nz.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://kk.nicolike.cn

Ruby: arr.index(x)
来源：http://zj.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://lp.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://gw.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://on.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yq.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://fs.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://mh.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pd.hnjuh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lm.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bo.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dg.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://lm.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oi.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bs.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://xi.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://rl.bjjhwx.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eh.nszjky.cn

Go:   // 手写循环
来源：http://os.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kz.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yb.newstarts.cn

[D15] 去重
来源：http://oa.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tx.lnxyls.cn

PHP:  array_unique($arr);
来源：http://mh.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://cr.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://nt.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ne.bookmarksfly.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yy.shxzukj.cn

Ruby: arr.uniq
来源：http://tw.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://pg.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://eh.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ns.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jv.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pb.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sf.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dl.shxzskj.cn

Go:   // 手写循环累加
来源：http://hc.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oj.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://na.jctech888.com.cn

[D17] 最大值与最小值
来源：http://ji.lnxyls.cn

Py:   max(arr);  min(arr)
来源：http://mi.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://ka.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rf.gzmigu.cn

TS:   Math.max(...arr);
来源：http://rd.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://as.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ep.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://hn.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://iz.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://rk.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qf.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://ll.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jt.yuexingan06.cn

TS:   nested.flat();
来源：http://aw.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tf.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://wy.lnxyls.cn

Ruby: nested.flatten
来源：http://zf.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wf.lnxyls.cn

[D19] 按字段分组
来源：http://mg.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jl.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uc.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xm.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jp.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ck.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://ky.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ud.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nk.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://dh.huanxung.cn

Py:   Counter(arr)
来源：http://wf.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://mc.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hf.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sd.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rf.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://eh.hahajie.cn

Ruby: arr.tally
来源：http://uh.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://el.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://ko.shtwfgs.cn

Py:   x in arr
来源：http://ja.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://fu.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://sv.9csxet.cn

TS:   arr.includes(x)
来源：http://hy.gzmigu.cn

Java: list.contains(x)
来源：http://cg.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://zb.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://fb.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://la.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://vf.huixinmuqiang.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ei.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ip.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hp.muxihuayi.cn

TS:   [...arr];
来源：http://jz.521024.cn

Java: new ArrayList<>(list);
来源：http://sp.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ud.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://th.hahajie.cn

C#:   new List<int>(list);
来源：http://cm.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://ge.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zx.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bk.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tg.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cv.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fs.yuntaijiaju.cn

Go:   // 手写循环
来源：http://fe.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zt.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gt.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://ik.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yo.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ln.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://es.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ou.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ap.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yz.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bd.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qw.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://jk.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fj.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://px.yuexingan06.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cf.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mu.colortex.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hr.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vn.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qn.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jh.szsharing.cn

[D26] 数组转字符串
来源：http://ld.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://ln.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://kp.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://xz.panjiajie.cn

TS:   arr.join(", ")
来源：http://cb.hnjuh.cn

Java: String.join(", ", list)
来源：http://oc.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://me.newstarts.cn

Ruby: arr.join(", ")
来源：http://qy.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ou.wgjwhj.cn

================================================================================
来源：http://vl.shxzskj.cn

E. 字符串处理
来源：http://kj.yuexingan06.cn

================================================================================
来源：http://xw.jctech888.com.cn

[E01] 拼接字符串
来源：http://vg.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://it.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pv.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uo.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://do.shxzukj.cn


<!-- 参考信息 -->