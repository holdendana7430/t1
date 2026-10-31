代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://cr.szsharing.cn

C#:   using System.Text;
来源：http://co.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://rv.szsharing.cn

Py:   (lambda: print("run"))()
来源：http://fe.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://mv.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://wf.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://rl.jctech888.com.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gj.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://ky.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://am.wgjwhj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://du.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://wa.panjiajie.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://du.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jg.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gp.chemitech.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hl.huixiangedu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lq.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://rz.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gn.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://an.shxzskj.cn

[C14] 泛型函数
来源：http://mj.jianghongdianzi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vv.bjjhwx.cn

PHP:  // 无泛型
来源：http://le.huixinmuqiang.cn

JS:   // 无泛型
来源：http://zj.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zu.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yg.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tu.yuntaijiaju.cn

Ruby: # 无泛型
来源：http://vu.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wo.nszjky.cn

[C15] 解构 / 展开参数
来源：http://sa.9csxet.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hk.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://ml.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ah.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vw.jctech888.com.cn

Java: // 无解构
来源：http://pp.nszjky.cn

Go:   // 无解构
来源：http://oc.yuntaijiaju.cn

Ruby: a, b = pair
来源：http://lx.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://zd.colortex.cn

[C16] 函数 / 方法重载
来源：http://cp.bjjhwx.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xq.yuntaijiaju.cn

PHP:  // 无重载
来源：http://te.lnxyls.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nx.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://hv.huixiangedu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mh.nicolike.cn

Go:   // 无重载：用不同函数名
来源：http://er.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://xq.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ee.521024.cn

================================================================================
来源：http://vq.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://us.jctech888.com.cn

================================================================================
来源：http://ow.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://qk.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wp.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jr.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ov.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hu.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vd.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://lx.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://pv.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.panjiajie.cn

[D02] 追加元素到末尾
来源：http://ub.bjjhwx.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jf.shtwfgs.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rm.521024.cn

JS:   arr.push(4);
来源：http://ak.shxzskj.cn

TS:   arr.push(4);
来源：http://yw.hnjuh.cn

Java: list.add(4);
来源：http://hq.521024.cn

Go:   arr = append(arr, 4)
来源：http://mc.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://tq.521024.cn

C#:   list.Add(4);
来源：http://mf.asd995.cn

[D03] 在指定位置插入元素
来源：http://ax.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://jv.newstarts.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wp.wgjwhj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jp.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://em.shtwfgs.cn

Java: list.add(0, 0);
来源：http://qr.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://oq.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iv.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://ls.muxihuayi.cn

[D04] 删除元素
来源：http://rk.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://in.bjjhwx.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kb.asd995.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xs.521024.cn

TS:   arr.splice(0, 1);
来源：http://zv.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ut.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jb.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nl.chemitech.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rm.muxihuayi.cn

[D05] 访问与修改元素
来源：http://wg.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cu.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dv.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ap.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://oh.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://qg.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://fk.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oj.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ol.lnxyls.cn

[D06] 数组长度
来源：http://mt.wgjwhj.cn

Py:   len(arr)
来源：http://hj.9csxet.cn

PHP:  count($arr);
来源：http://ej.shxzskj.cn

JS:   arr.length
来源：http://kj.chemitech.net.cn

TS:   arr.length
来源：http://em.521024.cn

Java: list.size();
来源：http://jb.wgjwhj.cn

Go:   len(arr)
来源：http://du.colortex.cn

Ruby: arr.length; arr.size
来源：http://tp.bookmarksfly.cn

C#:   list.Count;
来源：http://yd.colortex.cn

[D07] 切片 / 取子数组
来源：http://dh.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xz.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pi.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://go.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://fo.panjiajie.cn

Java: list.subList(1, 4);
来源：http://jc.wgjwhj.cn

Go:   arr[1:4]
来源：http://bl.jctech888.com.cn

Ruby: arr[1, 3]
来源：http://gh.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://gz.shxzskj.cn

[D08] 合并两个数组
来源：http://xv.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://by.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://jm.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xi.colortex.cn

TS:   [...a, ...b];
来源：http://io.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pv.huanxung.cn

Go:   append(a, b...)
来源：http://cl.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://zj.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://cj.gzmigu.cn

[D09] 排序（升序）
来源：http://fz.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://mb.yuntaijiaju.cn

PHP:  sort($arr);
来源：http://jq.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ds.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fi.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ko.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ue.nicolike.cn

Ruby: arr.sort
来源：http://ul.yuexingan06.cn

C#:   list.Sort();
来源：http://bt.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tf.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sk.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ll.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://if.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oi.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wc.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sq.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qm.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wo.jianghongdianzi.cn

[D11] 反转数组
来源：http://qd.wgjwhj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hw.newstarts.cn

PHP:  array_reverse($arr);
来源：http://iv.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dn.bjjhwx.cn

TS:   [...arr].reverse();
来源：http://pv.panjiajie.cn

Java: Collections.reverse(list);
来源：http://yj.521024.cn

Go:   slices.Reverse(arr)
来源：http://cx.bookmarksfly.cn

Ruby: arr.reverse
来源：http://fe.521024.cn

C#:   list.Reverse();
来源：http://xt.huixiangedu.cn

[D12] 查找元素下标
来源：http://pr.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://gl.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xy.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mx.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uu.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wj.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://la.yuexingan06.cn

Ruby: arr.index(x)
来源：http://vc.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://uz.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://pl.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bv.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yf.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://la.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://jl.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wl.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ln.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bc.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zg.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://qf.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ra.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qh.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://kj.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://uk.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tb.yuntaijiaju.cn

Go:   // 手写循环
来源：http://cw.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://df.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jr.huixiangedu.cn

[D15] 去重
来源：http://mb.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zu.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://co.newstarts.cn

JS:   [...new Set(arr)]
来源：http://qp.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://yr.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://av.szsharing.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zi.panjiajie.cn

Ruby: arr.uniq
来源：http://be.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://kz.asd995.cn

[D16] 求和与平均值
来源：http://fi.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pz.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tn.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nc.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bf.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cj.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://nm.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jy.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://za.szxytkj.cn

[D17] 最大值与最小值
来源：http://qd.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://cr.shtwfgs.cn

PHP:  max($arr);  min($arr);
来源：http://hn.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oq.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://zv.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qs.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rb.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://ne.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://pc.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://zf.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uq.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://qa.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sx.nicolike.cn

TS:   nested.flat();
来源：http://ci.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jj.yuexingan06.cn

Go:   // 手写双层循环
来源：http://kt.bjjhwx.cn

Ruby: nested.flatten
来源：http://kv.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bp.shxzukj.cn

[D19] 按字段分组
来源：http://eo.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uj.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ic.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hu.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fj.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xc.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://bw.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qw.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mt.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://re.9csxet.cn

Py:   Counter(arr)
来源：http://ki.newstarts.cn

PHP:  array_count_values($arr);
来源：http://ut.haigaiapp.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ai.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ot.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hy.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://ij.jctech888.com.cn

Ruby: arr.tally
来源：http://az.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jy.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://lv.bookmarksfly.cn

Py:   x in arr
来源：http://if.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://bf.shtwfgs.cn

JS:   arr.includes(x)
来源：http://wa.szsharing.cn

TS:   arr.includes(x)
来源：http://pe.bookmarksfly.cn

Java: list.contains(x)
来源：http://kl.521024.cn

Go:   slices.Contains(arr, x)
来源：http://js.newstarts.cn

Ruby: arr.include?(x)
来源：http://gv.nszjky.cn

C#:   list.Contains(x)
来源：http://iw.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://zj.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dr.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://or.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pp.asd995.cn

TS:   [...arr];
来源：http://ft.9csxet.cn

Java: new ArrayList<>(list);
来源：http://vd.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://be.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://fc.hnjuh.cn

C#:   new List<int>(list);
来源：http://dn.huixiangedu.cn

[D23] reduce 累积计算
来源：http://xv.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rj.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://af.huanxung.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xa.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zx.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ik.hnjuh.cn

Go:   // 手写循环
来源：http://zq.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ut.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oz.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://dm.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eg.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pg.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ko.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://op.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dd.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zv.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lf.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hx.colortex.cn

[D25] Set 集合去重与交并差
来源：http://qs.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wr.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ye.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mo.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bf.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dz.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qy.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ah.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mu.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://sr.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://fp.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://nl.yuexingan06.cn

JS:   arr.join(", ")
来源：http://pr.asd995.cn

TS:   arr.join(", ")
来源：http://fz.521024.cn

Java: String.join(", ", list)
来源：http://ti.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://xd.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://bw.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://zb.jianghongdianzi.cn

================================================================================
来源：http://bz.nszjky.cn

E. 字符串处理
来源：http://qt.haigaiapp.cn

================================================================================
来源：http://ak.hahajie.cn

[E01] 拼接字符串
来源：http://hu.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wz.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rd.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cx.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vb.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bh.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ej.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jj.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fk.panjiajie.cn

[E02] 重复字符串
来源：http://rb.jctech888.com.cn

Py:   "ab" * 3
来源：http://me.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://qj.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://pg.yuntaijiaju.cn


<!-- 参考信息 -->