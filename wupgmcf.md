代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ej.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tk.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://rc.bjjhwx.cn

Java: list.get(0); list.set(0, 9);
来源：http://ls.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://dk.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cx.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ns.wgjwhj.cn

[D06] 数组长度
来源：http://oj.shxzukj.cn

Py:   len(arr)
来源：http://ly.hnjuh.cn

PHP:  count($arr);
来源：http://tl.gzmigu.cn

JS:   arr.length
来源：http://am.hahajie.cn

TS:   arr.length
来源：http://tf.huanxung.cn

Java: list.size();
来源：http://pk.gzmigu.cn

Go:   len(arr)
来源：http://cm.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://tm.chemitech.net.cn

C#:   list.Count;
来源：http://la.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://br.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ur.bookmarksfly.cn

PHP:  array_slice($arr, 1, 3);
来源：http://it.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://xk.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://kw.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://mp.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://uw.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://gq.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://to.jctech888.com.cn

[D08] 合并两个数组
来源：http://gt.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://tz.gzmigu.cn

PHP:  array_merge($a, $b);
来源：http://vj.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aq.shxzukj.cn

TS:   [...a, ...b];
来源：http://sr.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ec.bjjhwx.cn

Go:   append(a, b...)
来源：http://th.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://uf.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://qh.yuexingan06.cn

[D09] 排序（升序）
来源：http://qj.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://nk.wgjwhj.cn

PHP:  sort($arr);
来源：http://of.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dl.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tg.colortex.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rd.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qn.huanxung.cn

Ruby: arr.sort
来源：http://ip.asd995.cn

C#:   list.Sort();
来源：http://he.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://je.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kv.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://le.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gw.colortex.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ng.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tf.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dv.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fs.jctech888.com.cn

[D11] 反转数组
来源：http://tp.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xo.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://cn.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qw.9csxet.cn

TS:   [...arr].reverse();
来源：http://ip.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://pw.521024.cn

Go:   slices.Reverse(arr)
来源：http://iw.szsharing.cn

Ruby: arr.reverse
来源：http://qj.hnjuh.cn

C#:   list.Reverse();
来源：http://tw.panjiajie.cn

[D12] 查找元素下标
来源：http://mm.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://ng.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yb.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mx.hnjuh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pt.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eh.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://ac.panjiajie.cn

Ruby: arr.index(x)
来源：http://uo.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://es.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://cv.muxihuayi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nv.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ms.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://dd.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://kq.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pn.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bq.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ml.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ri.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://lw.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lr.szsharing.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iu.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://rl.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://ow.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uo.haigaiapp.cn

Go:   // 手写循环
来源：http://uf.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oj.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vp.chemitech.net.cn

[D15] 去重
来源：http://ca.huixiangedu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dk.shxzukj.cn

PHP:  array_unique($arr);
来源：http://tk.shxzskj.cn

JS:   [...new Set(arr)]
来源：http://pt.asd995.cn

TS:   [...new Set(arr)]
来源：http://fq.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kx.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vg.newstarts.cn

Ruby: arr.uniq
来源：http://nz.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://zp.hnjuh.cn

[D16] 求和与平均值
来源：http://nq.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gk.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nb.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tw.nicolike.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wj.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rh.asd995.cn

Go:   // 手写循环累加
来源：http://lg.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lz.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://tw.haigaiapp.cn

[D17] 最大值与最小值
来源：http://cx.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://vv.521024.cn

PHP:  max($arr);  min($arr);
来源：http://cn.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mt.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://op.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yv.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xd.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://lw.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://uv.521024.cn

[D18] 扁平化嵌套数组
来源：http://to.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ks.shxzukj.cn

PHP:  array_merge(...$nested);
来源：http://md.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yn.shxzskj.cn

TS:   nested.flat();
来源：http://pb.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tk.jctech888.com.cn

Go:   // 手写双层循环
来源：http://rn.panjiajie.cn

Ruby: nested.flatten
来源：http://gz.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rp.muxihuayi.cn

[D19] 按字段分组
来源：http://tx.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rs.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rz.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jr.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sr.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hs.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://oi.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qi.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hp.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://vk.bookmarksfly.cn

Py:   Counter(arr)
来源：http://zg.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://vu.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wm.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gm.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lp.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://bu.yuntaijiaju.cn

Ruby: arr.tally
来源：http://nt.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qd.newstarts.cn

[D21] 判断是否包含某元素
来源：http://pu.lnxyls.cn

Py:   x in arr
来源：http://zz.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://xi.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://ig.wgjwhj.cn

TS:   arr.includes(x)
来源：http://wc.haigaiapp.cn

Java: list.contains(x)
来源：http://jh.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://mc.shxzskj.cn

Ruby: arr.include?(x)
来源：http://od.shxzukj.cn

C#:   list.Contains(x)
来源：http://dk.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://mw.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://px.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bk.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sn.huanxung.cn

TS:   [...arr];
来源：http://bh.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://li.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qi.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://ux.521024.cn

C#:   new List<int>(list);
来源：http://jj.gzmigu.cn

[D23] reduce 累积计算
来源：http://ou.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ij.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jh.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iy.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zx.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gv.huixinmuqiang.cn

Go:   // 手写循环
来源：http://qa.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hf.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cg.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://vu.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xh.wgjwhj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jx.asd995.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hy.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tn.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fc.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iz.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yd.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tu.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://nt.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xm.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qs.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://en.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fn.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ht.muxihuayi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jm.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pp.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://av.muxihuayi.cn

[D26] 数组转字符串
来源：http://mj.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://wj.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://sx.bookmarksfly.cn

JS:   arr.join(", ")
来源：http://ee.huixiangedu.cn

TS:   arr.join(", ")
来源：http://yd.hahajie.cn

Java: String.join(", ", list)
来源：http://rx.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://ir.9csxet.cn

Ruby: arr.join(", ")
来源：http://qv.hahajie.cn

C#:   string.Join(", ", list)
来源：http://ff.szxytkj.cn

================================================================================
来源：http://yx.asd995.cn

E. 字符串处理
来源：http://te.shxzskj.cn

================================================================================
来源：http://bp.wgjwhj.cn

[E01] 拼接字符串
来源：http://vv.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jp.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kf.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://os.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rz.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zh.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://by.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://am.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cp.jianghongdianzi.cn

[E02] 重复字符串
来源：http://tz.521024.cn

Py:   "ab" * 3
来源：http://ii.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://uf.nicolike.cn

JS:   "ab".repeat(3)
来源：http://vt.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://er.hnjuh.cn

Java: "ab".repeat(3)
来源：http://yk.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://rt.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://jt.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wj.9csxet.cn

[E03] 截取子串
来源：http://oi.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vy.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nz.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://de.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://pe.huanxung.cn

Java: s.substring(1, 4)
来源：http://wi.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wp.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mf.colortex.cn

C#:   s.Substring(1, 3)
来源：http://rw.shxzukj.cn

[E04] 查找子串位置
来源：http://gb.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://pb.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://jb.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kw.hnjuh.cn

TS:   s.indexOf("x")
来源：http://gn.hahajie.cn

Java: s.indexOf("x")
来源：http://iv.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://df.jctech888.com.cn

Ruby: s.index("x")
来源：http://jp.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://ur.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yr.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fm.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yc.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nv.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uj.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wa.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://we.shtwfgs.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jw.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dc.521024.cn

[E06] 替换子串
来源：http://lt.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dz.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://za.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kt.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://pl.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zb.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eh.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kj.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://kc.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://zb.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hu.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://io.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oc.yuntaijiaju.cn

TS:   s.split(",")
来源：http://pq.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cb.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ma.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://oh.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qg.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://fb.asd995.cn

Py:   ",".join(items)
来源：http://le.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ik.hnjuh.cn

JS:   items.join(",")
来源：http://up.yuntaijiaju.cn

TS:   items.join(",")
来源：http://sk.huanxung.cn

Java: String.join(",", items)
来源：http://ai.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://ox.huixiangedu.cn

Ruby: items.join(",")
来源：http://lx.lnxyls.cn

C#:   string.Join(",", items)
来源：http://gm.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://mv.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ls.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bu.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://zg.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://md.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://fq.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jx.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dq.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sn.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://tz.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pv.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dz.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://iw.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://yn.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://qr.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zg.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dr.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fz.muxihuayi.cn

[E11] 反转字符串
来源：http://da.hnjuh.cn

Py:   s[::-1]
来源：http://iz.huanxung.cn

PHP:  strrev($s);
来源：http://qp.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://ox.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://za.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ww.shxzskj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dp.muxihuayi.cn

Ruby: s.reverse
来源：http://ux.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://im.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://dt.shxzukj.cn

Py:   s.count("a")
来源：http://ru.9csxet.cn


<!-- 参考信息 -->