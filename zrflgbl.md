代发 wailian999

TS:   arr.slice(1, 4);
来源：http://cu.shxzskj.cn

Java: list.subList(1, 4);
来源：http://kp.shtwfgs.cn

Go:   arr[1:4]
来源：http://og.szxytkj.cn

Ruby: arr[1, 3]
来源：http://kz.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://lj.hahajie.cn

[D08] 合并两个数组
来源：http://ay.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://hk.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://vq.bjjhwx.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yy.haigaiapp.cn

TS:   [...a, ...b];
来源：http://zh.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wu.gzmigu.cn

Go:   append(a, b...)
来源：http://lo.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://dm.panjiajie.cn

C#:   a.Concat(b).ToList()
来源：http://ko.huanxung.cn

[D09] 排序（升序）
来源：http://rt.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://fq.huixiangedu.cn

PHP:  sort($arr);
来源：http://gf.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vc.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zx.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rg.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bl.lnxyls.cn

Ruby: arr.sort
来源：http://mt.hahajie.cn

C#:   list.Sort();
来源：http://kc.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ur.hnjuh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nf.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eh.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nf.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jo.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jy.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xy.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qo.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kz.521024.cn

[D11] 反转数组
来源：http://cs.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://by.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://wb.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://to.hahajie.cn

TS:   [...arr].reverse();
来源：http://am.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://gj.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://es.chemitech.net.cn

Ruby: arr.reverse
来源：http://zx.chemitech.net.cn

C#:   list.Reverse();
来源：http://qo.haigaiapp.cn

[D12] 查找元素下标
来源：http://uk.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://zh.huixinmuqiang.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ut.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mi.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wv.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bt.asd995.cn

Go:   slices.Index(arr, x)
来源：http://dx.nszjky.cn

Ruby: arr.index(x)
来源：http://qd.521024.cn

C#:   list.IndexOf(x);
来源：http://mh.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ay.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bb.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ze.shxzukj.cn

JS:   arr.filter(x => x > 3)
来源：http://pf.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://np.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yy.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ju.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gy.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vh.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://fh.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://co.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ng.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://rv.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://oj.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fr.yuexingan06.cn

Go:   // 手写循环
来源：http://yy.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yl.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iy.yuntaijiaju.cn

[D15] 去重
来源：http://rk.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ff.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://vj.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://we.colortex.cn

TS:   [...new Set(arr)]
来源：http://ts.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://op.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hz.huixiangedu.cn

Ruby: arr.uniq
来源：http://lq.asd995.cn

C#:   list.Distinct().ToList()
来源：http://ta.hahajie.cn

[D16] 求和与平均值
来源：http://ft.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cf.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://of.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pd.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rc.521024.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ht.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://gv.bookmarksfly.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vf.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://vs.szxytkj.cn

[D17] 最大值与最小值
来源：http://qs.jianghongdianzi.cn

Py:   max(arr);  min(arr)
来源：http://vp.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://no.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dx.nszjky.cn

TS:   Math.max(...arr);
来源：http://hc.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gr.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uu.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://ph.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://tf.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://pm.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yk.shtwfgs.cn

PHP:  array_merge(...$nested);
来源：http://uv.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://co.asd995.cn

TS:   nested.flat();
来源：http://xm.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mo.gzmigu.cn

Go:   // 手写双层循环
来源：http://sm.huixinmuqiang.cn

Ruby: nested.flatten
来源：http://la.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tp.jctech888.com.cn

[D19] 按字段分组
来源：http://ut.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yq.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hx.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bo.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fc.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ni.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://gt.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kx.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ww.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ut.colortex.cn

Py:   Counter(arr)
来源：http://ja.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://gz.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lq.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://th.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yl.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://mp.haigaiapp.cn

Ruby: arr.tally
来源：http://hb.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ps.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://tt.nicolike.cn

Py:   x in arr
来源：http://cu.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://hm.muxihuayi.cn

JS:   arr.includes(x)
来源：http://rt.nicolike.cn

TS:   arr.includes(x)
来源：http://ds.haigaiapp.cn

Java: list.contains(x)
来源：http://wl.lnxyls.cn

Go:   slices.Contains(arr, x)
来源：http://vp.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://ia.szsharing.cn

C#:   list.Contains(x)
来源：http://jl.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://ab.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fj.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zg.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://am.panjiajie.cn

TS:   [...arr];
来源：http://gr.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://js.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bo.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://ir.bookmarksfly.cn

C#:   new List<int>(list);
来源：http://ul.521024.cn

[D23] reduce 累积计算
来源：http://td.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wz.hahajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ca.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uw.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ct.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://az.hnjuh.cn

Go:   // 手写循环
来源：http://fn.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jk.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ar.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://oz.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://py.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ex.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rg.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bw.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zp.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nu.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cw.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qp.panjiajie.cn

[D25] Set 集合去重与交并差
来源：http://fk.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jy.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mu.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kt.muxihuayi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://if.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nm.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gf.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ks.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ss.shxzukj.cn

[D26] 数组转字符串
来源：http://ke.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://eu.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://ue.hahajie.cn

JS:   arr.join(", ")
来源：http://yp.nicolike.cn

TS:   arr.join(", ")
来源：http://uk.shxzukj.cn

Java: String.join(", ", list)
来源：http://gz.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://oa.521024.cn

Ruby: arr.join(", ")
来源：http://lt.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://ke.shxzskj.cn

================================================================================
来源：http://qk.bjjhwx.cn

E. 字符串处理
来源：http://uv.yuexingan06.cn

================================================================================
来源：http://wr.asd995.cn

[E01] 拼接字符串
来源：http://mc.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wt.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uc.shtwfgs.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gr.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sd.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oa.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rq.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fd.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cz.hnjuh.cn

[E02] 重复字符串
来源：http://pw.shxzskj.cn

Py:   "ab" * 3
来源：http://ps.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://sb.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://ba.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://gb.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://yn.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://mt.bjjhwx.cn

Ruby: "ab" * 3
来源：http://df.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ig.haigaiapp.cn

[E03] 截取子串
来源：http://rs.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lu.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vp.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://na.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://ct.shxzskj.cn

Java: s.substring(1, 4)
来源：http://si.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://we.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ve.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://ti.wgjwhj.cn

[E04] 查找子串位置
来源：http://uo.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://it.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://yh.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gp.hahajie.cn

TS:   s.indexOf("x")
来源：http://gw.hnjuh.cn

Java: s.indexOf("x")
来源：http://kc.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://uh.hahajie.cn

Ruby: s.index("x")
来源：http://tn.521024.cn

C#:   s.IndexOf("x")
来源：http://ww.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dm.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xx.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wj.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zy.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vf.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xw.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eu.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://et.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gu.wgjwhj.cn

[E06] 替换子串
来源：http://pj.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kg.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://sq.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sc.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://ei.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ou.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sq.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fc.hahajie.cn

C#:   s.Replace("a", "b")
来源：http://nz.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://ha.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gt.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fd.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xg.yuexingan06.cn

TS:   s.split(",")
来源：http://jx.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vd.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://va.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://nt.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lm.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://od.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://qf.panjiajie.cn

PHP:  implode(",", $items);
来源：http://ef.hahajie.cn

JS:   items.join(",")
来源：http://dq.521024.cn

TS:   items.join(",")
来源：http://pp.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://hi.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://lm.asd995.cn

Ruby: items.join(",")
来源：http://dl.9csxet.cn

C#:   string.Join(",", items)
来源：http://ek.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ss.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yk.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ag.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://gf.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://js.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://lz.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pg.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hy.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xy.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://lq.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sw.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tz.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://wq.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://gl.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://ss.bjjhwx.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zg.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://em.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xw.gzmigu.cn

[E11] 反转字符串
来源：http://je.colortex.cn

Py:   s[::-1]
来源：http://no.hnjuh.cn

PHP:  strrev($s);
来源：http://ly.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://up.521024.cn

TS:   [...s].reverse().join("")
来源：http://xg.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qh.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zg.gzmigu.cn

Ruby: s.reverse
来源：http://dk.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sr.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://hx.panjiajie.cn

Py:   s.count("a")
来源：http://qd.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://xk.hahajie.cn

JS:   s.split("a").length - 1
来源：http://vm.colortex.cn

TS:   s.split("a").length - 1
来源：http://al.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://th.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://it.lnxyls.cn

Ruby: s.count("a")
来源：http://sa.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://gt.szxytkj.cn

[E13] 逐字符遍历
来源：http://uh.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://ft.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lt.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bi.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pv.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ba.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ev.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xu.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fw.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://uf.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://na.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gl.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yh.panjiajie.cn


<!-- 参考信息 -->