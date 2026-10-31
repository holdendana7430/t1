代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tb.bookmarksfly.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kf.muxihuayi.cn

[D05] 访问与修改元素
来源：http://kz.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gb.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kw.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gv.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://cg.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://wa.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://ia.521024.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://om.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mv.asd995.cn

[D06] 数组长度
来源：http://yi.shxzskj.cn

Py:   len(arr)
来源：http://iq.wgjwhj.cn

PHP:  count($arr);
来源：http://bx.hahajie.cn

JS:   arr.length
来源：http://nt.9csxet.cn

TS:   arr.length
来源：http://nj.shxzskj.cn

Java: list.size();
来源：http://xy.bookmarksfly.cn

Go:   len(arr)
来源：http://cn.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://ie.wgjwhj.cn

C#:   list.Count;
来源：http://xj.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://cg.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wj.huixinmuqiang.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hd.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://el.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://vq.panjiajie.cn

Java: list.subList(1, 4);
来源：http://mq.szsharing.cn

Go:   arr[1:4]
来源：http://vc.lnxyls.cn

Ruby: arr[1, 3]
来源：http://yl.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://if.gzmigu.cn

[D08] 合并两个数组
来源：http://fs.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://ri.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://ji.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yb.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://yl.shxzukj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zp.hahajie.cn

Go:   append(a, b...)
来源：http://im.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ae.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://bj.hnjuh.cn

[D09] 排序（升序）
来源：http://su.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://kb.colortex.cn

PHP:  sort($arr);
来源：http://kj.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qx.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ms.hahajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fc.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eh.szsharing.cn

Ruby: arr.sort
来源：http://yb.szxytkj.cn

C#:   list.Sort();
来源：http://de.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uy.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ra.shtwfgs.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yl.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vx.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ve.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tt.wgjwhj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wn.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ms.wgjwhj.cn

[D11] 反转数组
来源：http://ym.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qz.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://xk.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cz.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://ct.9csxet.cn

Java: Collections.reverse(list);
来源：http://yr.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://iw.bookmarksfly.cn

Ruby: arr.reverse
来源：http://fq.colortex.cn

C#:   list.Reverse();
来源：http://hw.gzmigu.cn

[D12] 查找元素下标
来源：http://ar.nszjky.cn

Py:   arr.index(x);  x in arr
来源：http://la.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xk.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xz.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bk.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://go.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://fy.yuexingan06.cn

Ruby: arr.index(x)
来源：http://sk.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://nt.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://xs.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ii.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mf.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://mf.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://wj.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cq.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cg.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cz.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wa.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://do.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vd.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ss.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://cn.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://fz.hahajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tx.jianghongdianzi.cn

Go:   // 手写循环
来源：http://fv.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qt.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ak.yuexingan06.cn

[D15] 去重
来源：http://gn.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kj.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://mb.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://kh.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://hq.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tp.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bk.hahajie.cn

Ruby: arr.uniq
来源：http://pp.521024.cn

C#:   list.Distinct().ToList()
来源：http://sy.hnjuh.cn

[D16] 求和与平均值
来源：http://hx.huanxung.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sp.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yc.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mk.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://af.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ce.szsharing.cn

Go:   // 手写循环累加
来源：http://ki.shxzukj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zk.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://rc.shxzukj.cn

[D17] 最大值与最小值
来源：http://iu.521024.cn

Py:   max(arr);  min(arr)
来源：http://ia.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://ip.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://as.521024.cn

TS:   Math.max(...arr);
来源：http://fz.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wg.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ds.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://sf.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://bl.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://hw.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dk.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://xk.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fp.gzmigu.cn

TS:   nested.flat();
来源：http://qq.yuntaijiaju.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://os.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://mg.gzmigu.cn

Ruby: nested.flatten
来源：http://co.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://fl.nicolike.cn

[D19] 按字段分组
来源：http://tr.gzmigu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eo.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qv.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bq.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vh.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ga.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://fa.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yg.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xq.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://lc.colortex.cn

Py:   Counter(arr)
来源：http://jy.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://ai.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dj.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://by.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wu.asd995.cn

Go:   // 手写 map[T]int
来源：http://pp.jctech888.com.cn

Ruby: arr.tally
来源：http://kt.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gr.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://eb.chemitech.net.cn

Py:   x in arr
来源：http://sz.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://fg.shxzukj.cn

JS:   arr.includes(x)
来源：http://gc.jctech888.com.cn

TS:   arr.includes(x)
来源：http://cf.jianghongdianzi.cn

Java: list.contains(x)
来源：http://ra.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://lb.asd995.cn

Ruby: arr.include?(x)
来源：http://ag.521024.cn

C#:   list.Contains(x)
来源：http://ef.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://xy.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bl.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bn.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yb.nszjky.cn

TS:   [...arr];
来源：http://vg.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://fs.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ct.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ih.szsharing.cn

C#:   new List<int>(list);
来源：http://ho.nicolike.cn

[D23] reduce 累积计算
来源：http://zj.panjiajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://me.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nw.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gz.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ao.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bm.asd995.cn

Go:   // 手写循环
来源：http://rs.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dm.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gt.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://tb.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ig.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zi.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ey.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xc.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ch.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hi.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uq.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ap.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://tl.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gg.yuexingan06.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://us.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yg.huixinmuqiang.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mq.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dg.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://la.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wh.yuexingan06.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://em.9csxet.cn

[D26] 数组转字符串
来源：http://gd.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://nu.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://kf.panjiajie.cn

JS:   arr.join(", ")
来源：http://bu.muxihuayi.cn

TS:   arr.join(", ")
来源：http://je.asd995.cn

Java: String.join(", ", list)
来源：http://ah.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://re.szxytkj.cn

Ruby: arr.join(", ")
来源：http://pv.gzmigu.cn

C#:   string.Join(", ", list)
来源：http://bl.bjjhwx.cn

================================================================================
来源：http://es.jctech888.com.cn

E. 字符串处理
来源：http://kh.yuntaijiaju.cn

================================================================================
来源：http://on.colortex.cn

[E01] 拼接字符串
来源：http://nc.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hl.nszjky.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wz.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ww.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uf.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wj.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xj.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mn.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gb.szsharing.cn

[E02] 重复字符串
来源：http://om.shxzukj.cn

Py:   "ab" * 3
来源：http://ye.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://ss.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://uh.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://hh.lnxyls.cn

Java: "ab".repeat(3)
来源：http://rb.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://yc.gzmigu.cn

Ruby: "ab" * 3
来源：http://fb.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ll.haigaiapp.cn

[E03] 截取子串
来源：http://dr.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://de.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qd.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ua.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://wn.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://jh.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gw.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ba.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://zc.hnjuh.cn

[E04] 查找子串位置
来源：http://al.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://pm.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://jf.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xa.nszjky.cn

TS:   s.indexOf("x")
来源：http://aw.szsharing.cn

Java: s.indexOf("x")
来源：http://kq.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://eh.szsharing.cn

Ruby: s.index("x")
来源：http://ev.newstarts.cn

C#:   s.IndexOf("x")
来源：http://ic.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rx.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vq.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ts.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ma.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eb.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mt.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bu.9csxet.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xg.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jm.szsharing.cn

[E06] 替换子串
来源：http://kr.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ar.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://um.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qu.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://sp.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dx.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wq.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://di.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://dz.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://nm.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ax.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hs.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ak.yuntaijiaju.cn

TS:   s.split(",")
来源：http://ng.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tj.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cw.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://nx.panjiajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gy.hahajie.cn

[E08] 数组按分隔符合并
来源：http://ce.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://zq.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://is.bjjhwx.cn

JS:   items.join(",")
来源：http://co.asd995.cn

TS:   items.join(",")
来源：http://lg.newstarts.cn

Java: String.join(",", items)
来源：http://mp.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://zi.asd995.cn

Ruby: items.join(",")
来源：http://sw.hnjuh.cn

C#:   string.Join(",", items)
来源：http://jn.9csxet.cn

[E09] 去除所有空白字符
来源：http://im.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://np.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cq.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ol.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://sw.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://uq.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uv.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wu.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pv.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://hu.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qh.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zq.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://bg.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://pd.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://hp.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wu.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rg.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://he.jianghongdianzi.cn

[E11] 反转字符串
来源：http://jw.jctech888.com.cn

Py:   s[::-1]
来源：http://eh.shtwfgs.cn

PHP:  strrev($s);
来源：http://ry.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://nc.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://ls.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tt.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hn.nszjky.cn


<!-- 参考信息 -->