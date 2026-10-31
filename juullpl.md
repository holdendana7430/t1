代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pp.asd995.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qe.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nt.colortex.cn

Ruby: # 无泛型
来源：http://ea.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lp.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://ja.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ru.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://su.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://db.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://up.asd995.cn

Java: // 无解构
来源：http://sm.newstarts.cn

Go:   // 无解构
来源：http://cb.shxzskj.cn

Ruby: a, b = pair
来源：http://pc.huanxung.cn

C#:   var (a, b) = pair;
来源：http://of.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://ab.shxzskj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hj.shtwfgs.cn

PHP:  // 无重载
来源：http://sp.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cc.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://gc.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jv.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://ee.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://oa.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uf.bjjhwx.cn

================================================================================
来源：http://zr.muxihuayi.cn

D. 数组 / 列表 / 集合
来源：http://hh.panjiajie.cn

================================================================================
来源：http://xi.newstarts.cn

[D01] 创建数组 / 列表
来源：http://su.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vx.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://in.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://od.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ra.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gd.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://xj.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://he.521024.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mx.shxzskj.cn

[D02] 追加元素到末尾
来源：http://xq.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kl.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wj.chemitech.net.cn

JS:   arr.push(4);
来源：http://qk.bjjhwx.cn

TS:   arr.push(4);
来源：http://qh.szsharing.cn

Java: list.add(4);
来源：http://og.yuexingan06.cn

Go:   arr = append(arr, 4)
来源：http://fy.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://tw.huixiangedu.cn

C#:   list.Add(4);
来源：http://gz.szsharing.cn

[D03] 在指定位置插入元素
来源：http://mk.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://yc.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bv.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rj.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://yh.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://zw.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://du.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jk.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://ed.wgjwhj.cn

[D04] 删除元素
来源：http://az.newstarts.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sv.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://av.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lp.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://ku.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ug.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vb.yuexingan06.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rr.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zv.hnjuh.cn

[D05] 访问与修改元素
来源：http://hp.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gy.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oj.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mj.huanxung.cn

TS:   arr[0]; arr.at(-1);
来源：http://iy.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://lr.yuexingan06.cn

Go:   arr[0]; arr[0] = 9
来源：http://cb.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dh.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qf.9csxet.cn

[D06] 数组长度
来源：http://jl.asd995.cn

Py:   len(arr)
来源：http://bn.panjiajie.cn

PHP:  count($arr);
来源：http://cx.chemitech.net.cn

JS:   arr.length
来源：http://eb.yuexingan06.cn

TS:   arr.length
来源：http://ne.hnjuh.cn

Java: list.size();
来源：http://uo.colortex.cn

Go:   len(arr)
来源：http://dt.huanxung.cn

Ruby: arr.length; arr.size
来源：http://ht.wgjwhj.cn

C#:   list.Count;
来源：http://wi.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://ms.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wp.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kv.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://uh.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://os.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://fp.shtwfgs.cn

Go:   arr[1:4]
来源：http://tv.szxytkj.cn

Ruby: arr[1, 3]
来源：http://oo.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ju.nicolike.cn

[D08] 合并两个数组
来源：http://sk.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://hz.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://iq.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ro.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://hb.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yx.shtwfgs.cn

Go:   append(a, b...)
来源：http://ck.lnxyls.cn

Ruby: a + b;  a.concat(b)
来源：http://kr.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://qi.hahajie.cn

[D09] 排序（升序）
来源：http://vd.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://iz.gzmigu.cn

PHP:  sort($arr);
来源：http://vq.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dn.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nw.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sv.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wc.newstarts.cn

Ruby: arr.sort
来源：http://mh.szsharing.cn

C#:   list.Sort();
来源：http://my.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yi.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qs.shxzskj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lg.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yv.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sg.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ux.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ke.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gg.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vs.haigaiapp.cn

[D11] 反转数组
来源：http://vk.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gq.asd995.cn

PHP:  array_reverse($arr);
来源：http://qr.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wc.newstarts.cn

TS:   [...arr].reverse();
来源：http://hm.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://og.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://iy.huanxung.cn

Ruby: arr.reverse
来源：http://zj.haigaiapp.cn

C#:   list.Reverse();
来源：http://yo.huixinmuqiang.cn

[D12] 查找元素下标
来源：http://al.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://zi.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://og.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dt.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bj.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uw.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://pl.chemitech.net.cn

Ruby: arr.index(x)
来源：http://dk.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://ps.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ui.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iy.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yn.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://te.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://ab.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gw.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://de.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wh.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qe.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://dl.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uv.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zz.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://gc.521024.cn

TS:   arr.map(x => x * 2)
来源：http://xr.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sj.wgjwhj.cn

Go:   // 手写循环
来源：http://mg.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ck.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zq.shxzskj.cn

[D15] 去重
来源：http://au.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rm.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://yw.huanxung.cn

JS:   [...new Set(arr)]
来源：http://sc.9csxet.cn

TS:   [...new Set(arr)]
来源：http://rj.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ck.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vz.shtwfgs.cn

Ruby: arr.uniq
来源：http://nm.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://xd.shtwfgs.cn

[D16] 求和与平均值
来源：http://px.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uz.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vq.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rl.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mu.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bp.yuexingan06.cn

Go:   // 手写循环累加
来源：http://un.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xl.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://eg.hahajie.cn

[D17] 最大值与最小值
来源：http://ro.bookmarksfly.cn

Py:   max(arr);  min(arr)
来源：http://xn.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://ir.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hc.panjiajie.cn

TS:   Math.max(...arr);
来源：http://gi.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tm.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nw.asd995.cn

Ruby: arr.max;  arr.min
来源：http://ka.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://ov.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://xu.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lq.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://yi.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://em.shxzskj.cn

TS:   nested.flat();
来源：http://qi.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cl.jctech888.com.cn

Go:   // 手写双层循环
来源：http://vb.szsharing.cn

Ruby: nested.flatten
来源：http://bq.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nicolike.cn

[D19] 按字段分组
来源：http://yd.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dz.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ih.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ij.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tf.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nt.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://bc.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yy.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ie.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ii.huanxung.cn

Py:   Counter(arr)
来源：http://na.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://es.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pz.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uf.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dn.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://ft.szxytkj.cn

Ruby: arr.tally
来源：http://ku.bjjhwx.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nx.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://xg.chemitech.net.cn

Py:   x in arr
来源：http://be.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://ud.nszjky.cn

JS:   arr.includes(x)
来源：http://rp.huixiangedu.cn

TS:   arr.includes(x)
来源：http://td.colortex.cn

Java: list.contains(x)
来源：http://fi.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://kv.hnjuh.cn

Ruby: arr.include?(x)
来源：http://ex.yuexingan06.cn

C#:   list.Contains(x)
来源：http://pr.yuntaijiaju.cn

[D22] 复制数组（避免共享引用）
来源：http://fg.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bj.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ez.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bg.muxihuayi.cn

TS:   [...arr];
来源：http://mp.9csxet.cn

Java: new ArrayList<>(list);
来源：http://oi.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://di.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://bk.shxzukj.cn

C#:   new List<int>(list);
来源：http://qg.haigaiapp.cn

[D23] reduce 累积计算
来源：http://sr.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://su.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cw.yuexingan06.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ri.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jo.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zy.jianghongdianzi.cn

Go:   // 手写循环
来源：http://bl.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xo.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iv.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://fq.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pk.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gp.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fy.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://al.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yb.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mz.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xr.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xo.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://df.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wu.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vo.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pl.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nm.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cr.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jv.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ik.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xy.jctech888.com.cn

[D26] 数组转字符串
来源：http://bm.asd995.cn

Py:   ", ".join(map(str, arr))
来源：http://ca.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://st.shtwfgs.cn

JS:   arr.join(", ")
来源：http://tn.huixiangedu.cn

TS:   arr.join(", ")
来源：http://kc.colortex.cn

Java: String.join(", ", list)
来源：http://il.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://rq.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://lp.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://gd.yuexingan06.cn

================================================================================
来源：http://hz.9csxet.cn

E. 字符串处理
来源：http://pk.jctech888.com.cn

================================================================================
来源：http://dw.yuexingan06.cn

[E01] 拼接字符串
来源：http://ws.bjjhwx.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ul.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ks.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://au.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gp.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fo.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://je.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ux.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tk.521024.cn

[E02] 重复字符串
来源：http://po.bookmarksfly.cn

Py:   "ab" * 3
来源：http://gu.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://mv.521024.cn

JS:   "ab".repeat(3)
来源：http://en.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://qf.szsharing.cn

Java: "ab".repeat(3)
来源：http://zt.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://im.shtwfgs.cn

Ruby: "ab" * 3
来源：http://jh.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vu.yuexingan06.cn

[E03] 截取子串
来源：http://ay.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ij.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zs.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ad.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://aw.shxzskj.cn

Java: s.substring(1, 4)
来源：http://ba.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rz.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bq.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://xq.bookmarksfly.cn

[E04] 查找子串位置
来源：http://ui.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://pt.szsharing.cn

PHP:  strpos($s, "x");
来源：http://yc.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ky.shxzskj.cn

TS:   s.indexOf("x")
来源：http://nw.muxihuayi.cn

Java: s.indexOf("x")
来源：http://au.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://nn.521024.cn

Ruby: s.index("x")
来源：http://sk.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://wg.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://da.hnjuh.cn


<!-- 参考信息 -->