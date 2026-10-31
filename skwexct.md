代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://vr.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://gk.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ys.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://un.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://in.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bl.szsharing.cn

JS:   arr.push(4);
来源：http://hz.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://af.panjiajie.cn

Java: list.add(4);
来源：http://wj.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://kc.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://et.shxzukj.cn

C#:   list.Add(4);
来源：http://rj.nicolike.cn

[D03] 在指定位置插入元素
来源：http://ex.haigaiapp.cn

Py:   arr.insert(0, 0)
来源：http://cm.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://su.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lt.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://vx.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://jm.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://em.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gj.szsharing.cn

C#:   list.Insert(0, 0);
来源：http://sj.shxzskj.cn

[D04] 删除元素
来源：http://ss.shtwfgs.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dz.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rv.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qm.colortex.cn

TS:   arr.splice(0, 1);
来源：http://rf.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://du.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://su.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oj.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uy.gzmigu.cn

[D05] 访问与修改元素
来源：http://bp.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nc.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eo.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gf.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://lq.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://is.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://zl.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lx.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vn.muxihuayi.cn

[D06] 数组长度
来源：http://px.521024.cn

Py:   len(arr)
来源：http://fu.shxzukj.cn

PHP:  count($arr);
来源：http://un.yuexingan06.cn

JS:   arr.length
来源：http://nt.yuexingan06.cn

TS:   arr.length
来源：http://pg.huixinmuqiang.cn

Java: list.size();
来源：http://wk.huanxung.cn

Go:   len(arr)
来源：http://ih.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://gy.wgjwhj.cn

C#:   list.Count;
来源：http://vp.9csxet.cn

[D07] 切片 / 取子数组
来源：http://bo.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jd.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ui.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://ty.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://vx.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://ri.panjiajie.cn

Go:   arr[1:4]
来源：http://pa.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://xa.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://bi.szsharing.cn

[D08] 合并两个数组
来源：http://oe.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://cq.huixiangedu.cn

PHP:  array_merge($a, $b);
来源：http://fx.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qw.szxytkj.cn

TS:   [...a, ...b];
来源：http://jt.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gp.yuexingan06.cn

Go:   append(a, b...)
来源：http://aq.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://lx.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://ux.521024.cn

[D09] 排序（升序）
来源：http://io.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://se.shxzukj.cn

PHP:  sort($arr);
来源：http://mq.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://he.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ic.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ay.colortex.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mm.jctech888.com.cn

Ruby: arr.sort
来源：http://qa.muxihuayi.cn

C#:   list.Sort();
来源：http://ts.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gt.yuntaijiaju.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ag.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ey.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eo.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hi.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://up.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ak.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vh.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sk.colortex.cn

[D11] 反转数组
来源：http://vb.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fe.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://li.yuntaijiaju.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oa.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://ci.asd995.cn

Java: Collections.reverse(list);
来源：http://dp.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://eb.bjjhwx.cn

Ruby: arr.reverse
来源：http://bx.haigaiapp.cn

C#:   list.Reverse();
来源：http://qc.szxytkj.cn

[D12] 查找元素下标
来源：http://zm.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://hc.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eh.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ah.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fs.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qq.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://zu.panjiajie.cn

Ruby: arr.index(x)
来源：http://ev.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://pn.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://lz.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://en.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hj.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://pl.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://mu.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ms.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iu.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dk.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ab.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://hp.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ou.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ix.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://zc.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://rt.haigaiapp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fz.nszjky.cn

Go:   // 手写循环
来源：http://ni.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yb.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://in.panjiajie.cn

[D15] 去重
来源：http://hs.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gt.huanxung.cn

PHP:  array_unique($arr);
来源：http://fd.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://yv.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ch.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mf.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qb.hnjuh.cn

Ruby: arr.uniq
来源：http://mf.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://mu.colortex.cn

[D16] 求和与平均值
来源：http://dl.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ka.bjjhwx.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lw.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ky.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cy.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xm.nszjky.cn

Go:   // 手写循环累加
来源：http://ab.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pi.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://ol.chemitech.net.cn

[D17] 最大值与最小值
来源：http://kd.colortex.cn

Py:   max(arr);  min(arr)
来源：http://zq.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://uh.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ws.huanxung.cn

TS:   Math.max(...arr);
来源：http://vf.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xi.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ob.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://td.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://wb.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://qp.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://my.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://vm.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uc.shxzukj.cn

TS:   nested.flat();
来源：http://ui.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vm.newstarts.cn

Go:   // 手写双层循环
来源：http://ik.shxzskj.cn

Ruby: nested.flatten
来源：http://eu.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wk.shxzukj.cn

[D19] 按字段分组
来源：http://uc.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nw.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yo.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ik.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hy.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xf.asd995.cn

Go:   // 手写 map[string][]T
来源：http://fk.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dk.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zf.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://wv.jctech888.com.cn

Py:   Counter(arr)
来源：http://jm.asd995.cn

PHP:  array_count_values($arr);
来源：http://ip.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://br.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hq.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gx.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://ym.shtwfgs.cn

Ruby: arr.tally
来源：http://yb.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fi.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://bo.huixiangedu.cn

Py:   x in arr
来源：http://jc.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://yf.muxihuayi.cn

JS:   arr.includes(x)
来源：http://sj.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://nz.9csxet.cn

Java: list.contains(x)
来源：http://hf.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://qg.nicolike.cn

Ruby: arr.include?(x)
来源：http://kz.asd995.cn

C#:   list.Contains(x)
来源：http://pj.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://pa.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ih.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://np.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qp.shxzskj.cn

TS:   [...arr];
来源：http://cx.521024.cn

Java: new ArrayList<>(list);
来源：http://bs.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ox.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://xn.shxzskj.cn

C#:   new List<int>(list);
来源：http://gk.haigaiapp.cn

[D23] reduce 累积计算
来源：http://xv.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bs.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kw.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ff.521024.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kp.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zw.nszjky.cn

Go:   // 手写循环
来源：http://td.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gu.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lk.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://vd.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oi.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mr.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vt.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://py.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sx.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ns.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fc.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gm.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://dc.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xh.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ba.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pe.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gm.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jb.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uh.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iw.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ea.nicolike.cn

[D26] 数组转字符串
来源：http://jl.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://vs.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://co.colortex.cn

JS:   arr.join(", ")
来源：http://cv.yuexingan06.cn

TS:   arr.join(", ")
来源：http://ix.wgjwhj.cn

Java: String.join(", ", list)
来源：http://vk.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://jr.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://wh.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://dg.521024.cn

================================================================================
来源：http://rf.nszjky.cn

E. 字符串处理
来源：http://bs.521024.cn

================================================================================
来源：http://to.lnxyls.cn

[E01] 拼接字符串
来源：http://vs.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gw.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tl.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://py.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://li.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pw.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ra.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://aq.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sx.jianghongdianzi.cn

[E02] 重复字符串
来源：http://bv.yuexingan06.cn

Py:   "ab" * 3
来源：http://ll.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://zw.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://tu.9csxet.cn

TS:   "ab".repeat(3)
来源：http://vr.hnjuh.cn

Java: "ab".repeat(3)
来源：http://nn.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://pt.hahajie.cn

Ruby: "ab" * 3
来源：http://il.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wn.huixinmuqiang.cn

[E03] 截取子串
来源：http://lp.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ec.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ub.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://re.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://lb.nicolike.cn

Java: s.substring(1, 4)
来源：http://tf.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ve.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://go.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://at.nicolike.cn

[E04] 查找子串位置
来源：http://bu.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://hv.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://al.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bj.9csxet.cn

TS:   s.indexOf("x")
来源：http://oo.nszjky.cn

Java: s.indexOf("x")
来源：http://wu.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://jc.colortex.cn

Ruby: s.index("x")
来源：http://vb.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://dh.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ul.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mq.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ue.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qv.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://so.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sw.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ea.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yn.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yq.yuexingan06.cn

[E06] 替换子串
来源：http://cu.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jp.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://zw.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tm.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://yl.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bo.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zz.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mg.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://pa.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://ps.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ob.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://an.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zp.asd995.cn

TS:   s.split(",")
来源：http://vi.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xg.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jd.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://hu.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kw.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://nz.huixinmuqiang.cn

Py:   ",".join(items)
来源：http://ob.lnxyls.cn

PHP:  implode(",", $items);
来源：http://jm.bookmarksfly.cn

JS:   items.join(",")
来源：http://su.hnjuh.cn

TS:   items.join(",")
来源：http://dg.panjiajie.cn

Java: String.join(",", items)
来源：http://fs.colortex.cn


<!-- 参考信息 -->