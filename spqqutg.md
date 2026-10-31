代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://kl.asd995.cn

C#:   using System.Text;
来源：http://zc.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://un.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://wq.shtwfgs.cn

PHP:  (function () { echo "run"; })();
来源：http://mp.muxihuayi.cn

JS:   (() => { console.log("run"); })();
来源：http://dw.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://ts.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qp.huanxung.cn

Go:   func() { fmt.Println("run") }()
来源：http://fg.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://ka.asd995.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://av.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://mw.colortex.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gl.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iq.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yh.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pg.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xr.wgjwhj.cn

Go:   func add(a, b int) int
来源：http://vu.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://om.9csxet.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xq.shxzskj.cn

[C14] 泛型函数
来源：http://nm.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ul.colortex.cn

PHP:  // 无泛型
来源：http://ll.chemitech.net.cn

JS:   // 无泛型
来源：http://oa.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uz.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yr.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lp.shxzskj.cn

Ruby: # 无泛型
来源：http://yo.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mw.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://va.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dt.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://di.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://um.yuntaijiaju.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xe.huanxung.cn

Java: // 无解构
来源：http://dr.huixiangedu.cn

Go:   // 无解构
来源：http://px.nszjky.cn

Ruby: a, b = pair
来源：http://zi.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://ov.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://bt.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tx.521024.cn

PHP:  // 无重载
来源：http://go.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bf.521024.cn

TS:   // 用联合类型或重载签名声明
来源：http://ol.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://am.huixiangedu.cn

Go:   // 无重载：用不同函数名
来源：http://ym.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://yp.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lw.shtwfgs.cn

================================================================================
来源：http://ln.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://ip.newstarts.cn

================================================================================
来源：http://zy.newstarts.cn

[D01] 创建数组 / 列表
来源：http://dn.shtwfgs.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ws.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gp.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ws.bookmarksfly.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mp.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mo.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://pb.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://pb.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sx.newstarts.cn

[D02] 追加元素到末尾
来源：http://hq.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hl.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pv.newstarts.cn

JS:   arr.push(4);
来源：http://vy.haigaiapp.cn

TS:   arr.push(4);
来源：http://mz.panjiajie.cn

Java: list.add(4);
来源：http://tf.muxihuayi.cn

Go:   arr = append(arr, 4)
来源：http://vq.szsharing.cn

Ruby: arr << 4; arr.push(5)
来源：http://yh.asd995.cn

C#:   list.Add(4);
来源：http://gy.huanxung.cn

[D03] 在指定位置插入元素
来源：http://ho.nicolike.cn

Py:   arr.insert(0, 0)
来源：http://jx.bookmarksfly.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ao.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ji.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://uh.9csxet.cn

Java: list.add(0, 0);
来源：http://km.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xh.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lc.muxihuayi.cn

C#:   list.Insert(0, 0);
来源：http://qu.asd995.cn

[D04] 删除元素
来源：http://yj.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sw.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zd.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qa.colortex.cn

TS:   arr.splice(0, 1);
来源：http://rt.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ju.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vo.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rd.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cz.jctech888.com.cn

[D05] 访问与修改元素
来源：http://no.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://et.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eu.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vk.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://rb.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://gx.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://ct.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kf.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oo.huanxung.cn

[D06] 数组长度
来源：http://un.newstarts.cn

Py:   len(arr)
来源：http://so.521024.cn

PHP:  count($arr);
来源：http://tq.huanxung.cn

JS:   arr.length
来源：http://em.asd995.cn

TS:   arr.length
来源：http://rl.hahajie.cn

Java: list.size();
来源：http://xj.huanxung.cn

Go:   len(arr)
来源：http://ih.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://nu.chemitech.net.cn

C#:   list.Count;
来源：http://se.521024.cn

[D07] 切片 / 取子数组
来源：http://eg.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mf.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jq.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://hk.gzmigu.cn

TS:   arr.slice(1, 4);
来源：http://wx.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://xq.shxzukj.cn

Go:   arr[1:4]
来源：http://ht.newstarts.cn

Ruby: arr[1, 3]
来源：http://od.huixinmuqiang.cn

C#:   list.GetRange(1, 3);
来源：http://ri.bjjhwx.cn

[D08] 合并两个数组
来源：http://gt.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://cb.yuexingan06.cn

PHP:  array_merge($a, $b);
来源：http://sb.nicolike.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://js.gzmigu.cn

TS:   [...a, ...b];
来源：http://lr.hnjuh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eb.shxzukj.cn

Go:   append(a, b...)
来源：http://so.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://nf.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://bx.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://wu.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://cg.gzmigu.cn

PHP:  sort($arr);
来源：http://ri.szxytkj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xr.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ct.huixiangedu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://my.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xo.gzmigu.cn

Ruby: arr.sort
来源：http://qa.szsharing.cn

C#:   list.Sort();
来源：http://ot.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wt.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qw.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ex.hnjuh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gj.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xb.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dy.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sy.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hh.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ok.jianghongdianzi.cn

[D11] 反转数组
来源：http://fk.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zp.nszjky.cn

PHP:  array_reverse($arr);
来源：http://pr.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qh.nszjky.cn

TS:   [...arr].reverse();
来源：http://bv.hnjuh.cn

Java: Collections.reverse(list);
来源：http://bb.521024.cn

Go:   slices.Reverse(arr)
来源：http://hf.newstarts.cn

Ruby: arr.reverse
来源：http://lo.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://vo.shxzukj.cn

[D12] 查找元素下标
来源：http://lt.521024.cn

Py:   arr.index(x);  x in arr
来源：http://mh.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wn.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vt.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vl.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://of.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://uy.521024.cn

Ruby: arr.index(x)
来源：http://ef.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://uo.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://wj.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sh.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kl.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://ri.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://jl.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://es.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ck.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vw.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jr.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://sn.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://an.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jj.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://mx.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://oj.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nh.lnxyls.cn

Go:   // 手写循环
来源：http://gk.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cs.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sd.shxzukj.cn

[D15] 去重
来源：http://js.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mb.bookmarksfly.cn

PHP:  array_unique($arr);
来源：http://ba.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://qm.huanxung.cn

TS:   [...new Set(arr)]
来源：http://zl.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sr.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vd.huanxung.cn

Ruby: arr.uniq
来源：http://gq.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://fp.panjiajie.cn

[D16] 求和与平均值
来源：http://hv.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jn.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ij.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gy.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ys.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ba.asd995.cn

Go:   // 手写循环累加
来源：http://my.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iy.521024.cn

C#:   list.Sum();  list.Average()
来源：http://rc.9csxet.cn

[D17] 最大值与最小值
来源：http://cy.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://lj.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://hh.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bh.nszjky.cn

TS:   Math.max(...arr);
来源：http://ae.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ns.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kq.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://eh.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://qp.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://ld.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pt.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://mt.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ry.bjjhwx.cn

TS:   nested.flat();
来源：http://kl.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://at.muxihuayi.cn

Go:   // 手写双层循环
来源：http://ea.gzmigu.cn

Ruby: nested.flatten
来源：http://mn.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://me.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ga.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://un.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://km.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://si.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qr.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zu.colortex.cn

Go:   // 手写 map[string][]T
来源：http://zv.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zp.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ya.colortex.cn

[D20] 统计每个元素出现次数
来源：http://ux.bookmarksfly.cn

Py:   Counter(arr)
来源：http://st.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://uz.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sd.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rv.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eb.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://cf.muxihuayi.cn

Ruby: arr.tally
来源：http://uq.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wc.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://zd.yuntaijiaju.cn

Py:   x in arr
来源：http://dv.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://of.521024.cn

JS:   arr.includes(x)
来源：http://da.yuexingan06.cn

TS:   arr.includes(x)
来源：http://vw.nicolike.cn

Java: list.contains(x)
来源：http://rm.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://hr.nicolike.cn

Ruby: arr.include?(x)
来源：http://gg.hahajie.cn

C#:   list.Contains(x)
来源：http://hv.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://li.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vp.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tv.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lc.521024.cn

TS:   [...arr];
来源：http://pp.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://uf.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nm.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://cn.gzmigu.cn

C#:   new List<int>(list);
来源：http://ld.lnxyls.cn

[D23] reduce 累积计算
来源：http://ls.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rd.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://py.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rx.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gd.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ci.521024.cn

Go:   // 手写循环
来源：http://ie.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://er.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pj.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://rj.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://si.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mh.hahajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wg.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://po.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yo.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rw.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://da.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cz.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://tx.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gq.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ts.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hd.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://el.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://df.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rk.szxytkj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zt.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://is.lnxyls.cn

[D26] 数组转字符串
来源：http://pa.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://va.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://kr.asd995.cn

JS:   arr.join(", ")
来源：http://kw.lnxyls.cn

TS:   arr.join(", ")
来源：http://al.gzmigu.cn

Java: String.join(", ", list)
来源：http://hm.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://cn.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://wc.nszjky.cn

C#:   string.Join(", ", list)
来源：http://hm.9csxet.cn

================================================================================
来源：http://ol.huixinmuqiang.cn

E. 字符串处理
来源：http://cb.shtwfgs.cn

================================================================================
来源：http://do.gzmigu.cn

[E01] 拼接字符串
来源：http://tb.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qi.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kz.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ww.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://le.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ub.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bn.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bm.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qc.521024.cn

[E02] 重复字符串
来源：http://tl.9csxet.cn

Py:   "ab" * 3
来源：http://sm.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://kv.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://ma.panjiajie.cn


<!-- 参考信息 -->