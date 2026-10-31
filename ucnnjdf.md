代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dd.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yz.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://cm.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://na.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ds.yuntaijiaju.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dj.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ci.jianghongdianzi.cn

[D06] 数组长度
来源：http://ml.lnxyls.cn

Py:   len(arr)
来源：http://vg.9csxet.cn

PHP:  count($arr);
来源：http://at.bookmarksfly.cn

JS:   arr.length
来源：http://ha.muxihuayi.cn

TS:   arr.length
来源：http://xn.shtwfgs.cn

Java: list.size();
来源：http://qb.huanxung.cn

Go:   len(arr)
来源：http://gc.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://mf.bjjhwx.cn

C#:   list.Count;
来源：http://jp.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://nh.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wa.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bj.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://gn.shxzukj.cn

TS:   arr.slice(1, 4);
来源：http://mk.nszjky.cn

Java: list.subList(1, 4);
来源：http://qw.bookmarksfly.cn

Go:   arr[1:4]
来源：http://vh.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://uj.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://cj.9csxet.cn

[D08] 合并两个数组
来源：http://on.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://wm.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://cx.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sn.colortex.cn

TS:   [...a, ...b];
来源：http://le.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xm.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://lf.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://lz.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://ep.szsharing.cn

[D09] 排序（升序）
来源：http://vi.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://mu.shxzukj.cn

PHP:  sort($arr);
来源：http://rn.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fp.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yb.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yb.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ld.bjjhwx.cn

Ruby: arr.sort
来源：http://de.hahajie.cn

C#:   list.Sort();
来源：http://pn.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fv.huixiangedu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dh.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://es.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://in.bookmarksfly.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hr.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ow.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ft.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dp.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sz.lnxyls.cn

[D11] 反转数组
来源：http://hq.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ml.nicolike.cn

PHP:  array_reverse($arr);
来源：http://rb.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ge.szxytkj.cn

TS:   [...arr].reverse();
来源：http://ta.gzmigu.cn

Java: Collections.reverse(list);
来源：http://tf.colortex.cn

Go:   slices.Reverse(arr)
来源：http://nz.hahajie.cn

Ruby: arr.reverse
来源：http://ig.nicolike.cn

C#:   list.Reverse();
来源：http://xl.asd995.cn

[D12] 查找元素下标
来源：http://jd.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://rd.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bo.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qv.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sa.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ba.asd995.cn

Go:   slices.Index(arr, x)
来源：http://hk.szsharing.cn

Ruby: arr.index(x)
来源：http://zc.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://kq.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://uo.shtwfgs.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bc.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tj.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://mx.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://zo.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sn.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sy.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fl.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nj.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://tf.521024.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sm.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ns.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://iz.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://ag.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pi.521024.cn

Go:   // 手写循环
来源：http://fd.huixiangedu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://de.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pq.haigaiapp.cn

[D15] 去重
来源：http://xz.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://go.bjjhwx.cn

PHP:  array_unique($arr);
来源：http://ib.hahajie.cn

JS:   [...new Set(arr)]
来源：http://md.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://mx.shxzskj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kp.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ja.9csxet.cn

Ruby: arr.uniq
来源：http://zs.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://wz.hahajie.cn

[D16] 求和与平均值
来源：http://yk.bookmarksfly.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ov.colortex.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fq.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sm.asd995.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xv.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zv.521024.cn

Go:   // 手写循环累加
来源：http://qc.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vp.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://hb.asd995.cn

[D17] 最大值与最小值
来源：http://sa.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://lc.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://ym.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bd.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://cr.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lm.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tj.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://ym.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://od.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://zs.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://je.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://fu.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ba.huixinmuqiang.cn

TS:   nested.flat();
来源：http://eo.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://er.huixiangedu.cn

Go:   // 手写双层循环
来源：http://vp.lnxyls.cn

Ruby: nested.flatten
来源：http://kf.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ws.asd995.cn

[D19] 按字段分组
来源：http://om.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wp.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zg.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yl.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nf.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gt.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://rh.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bs.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://po.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://uj.newstarts.cn

Py:   Counter(arr)
来源：http://lg.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://ae.huixinmuqiang.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oc.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yd.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ja.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://vy.jianghongdianzi.cn

Ruby: arr.tally
来源：http://wa.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qh.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://ly.colortex.cn

Py:   x in arr
来源：http://fk.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://wj.szxytkj.cn

JS:   arr.includes(x)
来源：http://xz.newstarts.cn

TS:   arr.includes(x)
来源：http://zc.nicolike.cn

Java: list.contains(x)
来源：http://xh.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://pm.panjiajie.cn

Ruby: arr.include?(x)
来源：http://ai.newstarts.cn

C#:   list.Contains(x)
来源：http://io.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://cu.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ez.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ae.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vq.chemitech.net.cn

TS:   [...arr];
来源：http://jo.colortex.cn

Java: new ArrayList<>(list);
来源：http://qm.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yc.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://ss.lnxyls.cn

C#:   new List<int>(list);
来源：http://ns.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://iq.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xt.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fd.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ck.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ed.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ak.bjjhwx.cn

Go:   // 手写循环
来源：http://dw.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fl.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ms.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://vx.shxzskj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jl.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sb.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uo.nszjky.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cq.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xa.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://za.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jd.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ke.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://fu.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bh.szsharing.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bs.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zf.shtwfgs.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ya.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ah.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://by.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ee.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://on.szsharing.cn

[D26] 数组转字符串
来源：http://cw.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://sj.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://ht.shxzskj.cn

JS:   arr.join(", ")
来源：http://nj.asd995.cn

TS:   arr.join(", ")
来源：http://is.shxzskj.cn

Java: String.join(", ", list)
来源：http://hp.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://fp.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://qc.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://jj.nicolike.cn

================================================================================
来源：http://bl.huanxung.cn

E. 字符串处理
来源：http://kg.newstarts.cn

================================================================================
来源：http://wt.szsharing.cn

[E01] 拼接字符串
来源：http://jb.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uf.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hx.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xs.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sx.bjjhwx.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kl.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://av.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xb.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lr.yuntaijiaju.cn

[E02] 重复字符串
来源：http://an.huanxung.cn

Py:   "ab" * 3
来源：http://ib.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://jf.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://kq.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://he.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ef.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://qk.huixiangedu.cn

Ruby: "ab" * 3
来源：http://bt.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hg.newstarts.cn

[E03] 截取子串
来源：http://as.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bq.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ou.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nd.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://ky.huanxung.cn

Java: s.substring(1, 4)
来源：http://ud.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eq.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zw.asd995.cn

C#:   s.Substring(1, 3)
来源：http://cx.asd995.cn

[E04] 查找子串位置
来源：http://gz.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://eb.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://fp.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ov.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ip.haigaiapp.cn

Java: s.indexOf("x")
来源：http://fs.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://ak.szsharing.cn

Ruby: s.index("x")
来源：http://dq.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://yt.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sd.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ce.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qm.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eg.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tg.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cd.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hh.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ys.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lf.jctech888.com.cn

[E06] 替换子串
来源：http://ed.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ah.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://ba.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://no.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://fa.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ku.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jd.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lq.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://sx.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://ud.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sy.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xn.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yd.newstarts.cn

TS:   s.split(",")
来源：http://sb.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fk.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sc.asd995.cn

Ruby: s.split(",");  s.split
来源：http://lp.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gd.hahajie.cn

[E08] 数组按分隔符合并
来源：http://ev.wgjwhj.cn

Py:   ",".join(items)
来源：http://cq.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://kq.shxzskj.cn

JS:   items.join(",")
来源：http://cn.huanxung.cn

TS:   items.join(",")
来源：http://kj.wgjwhj.cn

Java: String.join(",", items)
来源：http://mu.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://mk.nicolike.cn

Ruby: items.join(",")
来源：http://bh.lnxyls.cn

C#:   string.Join(",", items)
来源：http://fu.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://os.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://af.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pm.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://sn.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://gl.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://rq.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ls.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wr.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qf.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://pf.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bl.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rk.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://nc.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://fj.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ty.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://do.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nl.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vl.9csxet.cn

[E11] 反转字符串
来源：http://zh.newstarts.cn

Py:   s[::-1]
来源：http://dh.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://ee.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://ov.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://tz.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sr.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://od.yuexingan06.cn

Ruby: s.reverse
来源：http://td.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mb.newstarts.cn

[E12] 统计某字符出现次数
来源：http://lv.szsharing.cn

Py:   s.count("a")
来源：http://fs.colortex.cn


<!-- 参考信息 -->