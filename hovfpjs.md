代发 wailian999

[C14] 泛型函数
来源：http://lw.gzmigu.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nr.gzmigu.cn

PHP:  // 无泛型
来源：http://tb.huixinmuqiang.cn

JS:   // 无泛型
来源：http://al.asd995.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://da.newstarts.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yp.haigaiapp.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://if.asd995.cn

Ruby: # 无泛型
来源：http://me.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gc.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://bi.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kp.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://fg.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bl.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://no.shxzukj.cn

Java: // 无解构
来源：http://uc.bookmarksfly.cn

Go:   // 无解构
来源：http://xd.gzmigu.cn

Ruby: a, b = pair
来源：http://eu.muxihuayi.cn

C#:   var (a, b) = pair;
来源：http://rk.nicolike.cn

[C16] 函数 / 方法重载
来源：http://ir.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://it.colortex.cn

PHP:  // 无重载
来源：http://nv.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hp.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://sb.bjjhwx.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://di.colortex.cn

Go:   // 无重载：用不同函数名
来源：http://fq.newstarts.cn

Ruby: # 无重载：靠动态参数
来源：http://fu.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wg.jianghongdianzi.cn

================================================================================
来源：http://vn.chemitech.net.cn

D. 数组 / 列表 / 集合
来源：http://dm.shxzskj.cn

================================================================================
来源：http://za.hahajie.cn

[D01] 创建数组 / 列表
来源：http://pp.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://hj.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ro.9csxet.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ok.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ai.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cw.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://pg.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://pe.newstarts.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pf.colortex.cn

[D02] 追加元素到末尾
来源：http://ir.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vt.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zz.shxzukj.cn

JS:   arr.push(4);
来源：http://sn.shxzskj.cn

TS:   arr.push(4);
来源：http://ql.yuexingan06.cn

Java: list.add(4);
来源：http://xg.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://ag.521024.cn

Ruby: arr << 4; arr.push(5)
来源：http://xr.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://ih.nszjky.cn

[D03] 在指定位置插入元素
来源：http://ns.panjiajie.cn

Py:   arr.insert(0, 0)
来源：http://ev.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gi.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lw.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://zd.bjjhwx.cn

Java: list.add(0, 0);
来源：http://oc.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ml.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bp.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://fh.chemitech.net.cn

[D04] 删除元素
来源：http://ky.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sp.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lb.521024.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bb.bjjhwx.cn

TS:   arr.splice(0, 1);
来源：http://tg.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cf.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://um.panjiajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ra.huixiangedu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vk.lnxyls.cn

[D05] 访问与修改元素
来源：http://fs.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wg.shxzukj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ca.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sk.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://zy.muxihuayi.cn

Java: list.get(0); list.set(0, 9);
来源：http://zx.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://rk.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jh.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jr.jctech888.com.cn

[D06] 数组长度
来源：http://te.gzmigu.cn

Py:   len(arr)
来源：http://ec.nszjky.cn

PHP:  count($arr);
来源：http://ty.lnxyls.cn

JS:   arr.length
来源：http://iy.jctech888.com.cn

TS:   arr.length
来源：http://qq.colortex.cn

Java: list.size();
来源：http://wm.muxihuayi.cn

Go:   len(arr)
来源：http://bd.szsharing.cn

Ruby: arr.length; arr.size
来源：http://uw.newstarts.cn

C#:   list.Count;
来源：http://wp.nicolike.cn

[D07] 切片 / 取子数组
来源：http://en.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kx.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ic.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://pf.yuntaijiaju.cn

TS:   arr.slice(1, 4);
来源：http://fi.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://oc.shxzukj.cn

Go:   arr[1:4]
来源：http://cf.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://cs.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://bt.chemitech.net.cn

[D08] 合并两个数组
来源：http://mz.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://mu.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://wc.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hn.chemitech.net.cn

TS:   [...a, ...b];
来源：http://ib.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oi.9csxet.cn

Go:   append(a, b...)
来源：http://xi.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://ju.shtwfgs.cn

C#:   a.Concat(b).ToList()
来源：http://ki.huixiangedu.cn

[D09] 排序（升序）
来源：http://or.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ex.szxytkj.cn

PHP:  sort($arr);
来源：http://ul.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mk.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cr.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sa.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ql.521024.cn

Ruby: arr.sort
来源：http://sm.shxzskj.cn

C#:   list.Sort();
来源：http://xv.nicolike.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bl.hahajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gz.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ty.muxihuayi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pk.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fy.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://un.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rl.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hn.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nw.colortex.cn

[D11] 反转数组
来源：http://eu.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hk.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://dn.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wo.asd995.cn

TS:   [...arr].reverse();
来源：http://ts.nicolike.cn

Java: Collections.reverse(list);
来源：http://ad.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://yo.yuexingan06.cn

Ruby: arr.reverse
来源：http://yz.shxzskj.cn

C#:   list.Reverse();
来源：http://mf.gzmigu.cn

[D12] 查找元素下标
来源：http://ra.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://fl.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yk.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cu.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ej.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dr.colortex.cn

Go:   slices.Index(arr, x)
来源：http://kt.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://oi.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://ox.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://tt.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vf.wgjwhj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kh.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://vr.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://ac.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ac.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ax.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pd.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jj.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://lh.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hd.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vx.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://uh.nicolike.cn

TS:   arr.map(x => x * 2)
来源：http://zs.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ne.szxytkj.cn

Go:   // 手写循环
来源：http://ik.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yt.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fx.lnxyls.cn

[D15] 去重
来源：http://zb.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://as.gzmigu.cn

PHP:  array_unique($arr);
来源：http://do.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://aw.nicolike.cn

TS:   [...new Set(arr)]
来源：http://th.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uk.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xs.newstarts.cn

Ruby: arr.uniq
来源：http://en.hnjuh.cn

C#:   list.Distinct().ToList()
来源：http://ir.shtwfgs.cn

[D16] 求和与平均值
来源：http://ox.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ab.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hu.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vf.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://au.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mq.wgjwhj.cn

Go:   // 手写循环累加
来源：http://yu.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jp.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://mp.szxytkj.cn

[D17] 最大值与最小值
来源：http://rk.colortex.cn

Py:   max(arr);  min(arr)
来源：http://cx.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://da.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ul.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://gi.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xm.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xq.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://xa.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://ct.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://zx.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vt.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://cm.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kz.chemitech.net.cn

TS:   nested.flat();
来源：http://ha.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bs.hahajie.cn

Go:   // 手写双层循环
来源：http://cr.nicolike.cn

Ruby: nested.flatten
来源：http://br.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qa.nicolike.cn

[D19] 按字段分组
来源：http://xb.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rl.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aa.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xf.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xe.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oh.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://vn.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://om.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fn.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://fw.bjjhwx.cn

Py:   Counter(arr)
来源：http://uv.hahajie.cn

PHP:  array_count_values($arr);
来源：http://ga.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oc.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jx.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lo.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://iu.shxzskj.cn

Ruby: arr.tally
来源：http://hr.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rk.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://vh.haigaiapp.cn

Py:   x in arr
来源：http://js.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://ow.panjiajie.cn

JS:   arr.includes(x)
来源：http://mb.asd995.cn

TS:   arr.includes(x)
来源：http://qv.szsharing.cn

Java: list.contains(x)
来源：http://jn.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://kh.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://gs.nszjky.cn

C#:   list.Contains(x)
来源：http://rs.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://ca.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ly.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gd.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vl.shxzskj.cn

TS:   [...arr];
来源：http://mn.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://nw.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pk.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://rm.szxytkj.cn

C#:   new List<int>(list);
来源：http://dw.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://uu.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pa.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lc.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lv.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tx.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://go.521024.cn

Go:   // 手写循环
来源：http://fr.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vn.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nc.521024.cn

[D24] 字典 / Map 基本操作
来源：http://wl.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fb.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ow.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oz.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yj.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fs.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://li.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jp.wgjwhj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ed.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://vj.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wu.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ry.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cf.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tw.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tl.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bh.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vk.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yu.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ij.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://iq.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://ya.shxzskj.cn

JS:   arr.join(", ")
来源：http://re.shxzukj.cn

TS:   arr.join(", ")
来源：http://sf.muxihuayi.cn

Java: String.join(", ", list)
来源：http://yy.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://uk.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://xh.hahajie.cn

C#:   string.Join(", ", list)
来源：http://bx.521024.cn

================================================================================
来源：http://vr.chemitech.net.cn

E. 字符串处理
来源：http://bo.yuexingan06.cn

================================================================================
来源：http://vf.szsharing.cn

[E01] 拼接字符串
来源：http://pz.huixinmuqiang.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qg.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fc.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jx.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ra.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dw.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qa.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hd.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ay.yuexingan06.cn

[E02] 重复字符串
来源：http://rt.huixiangedu.cn

Py:   "ab" * 3
来源：http://iw.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://eu.asd995.cn

JS:   "ab".repeat(3)
来源：http://nn.9csxet.cn

TS:   "ab".repeat(3)
来源：http://zt.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://tb.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://sr.shxzukj.cn

Ruby: "ab" * 3
来源：http://rx.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bc.nszjky.cn

[E03] 截取子串
来源：http://bx.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ws.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fd.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jh.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://cz.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://wy.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jw.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zi.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://mt.colortex.cn

[E04] 查找子串位置
来源：http://cu.nszjky.cn

Py:   s.find("x");  s.index("x")
来源：http://qc.9csxet.cn

PHP:  strpos($s, "x");
来源：http://xu.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vo.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://qt.shxzskj.cn

Java: s.indexOf("x")
来源：http://yj.bookmarksfly.cn


<!-- 参考信息 -->