代发 wailian999

PHP:  sort($arr);
来源：http://ei.gzmigu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dm.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gx.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wa.szxytkj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xp.shxzskj.cn

Ruby: arr.sort
来源：http://qp.huixinmuqiang.cn

C#:   list.Sort();
来源：http://ic.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://az.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ma.szsharing.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://da.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://em.newstarts.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cz.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ab.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gy.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jk.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ay.huanxung.cn

[D11] 反转数组
来源：http://na.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ql.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://hv.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://ok.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://vt.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://gl.newstarts.cn

Ruby: arr.reverse
来源：http://co.jctech888.com.cn

C#:   list.Reverse();
来源：http://ss.hahajie.cn

[D12] 查找元素下标
来源：http://xc.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://xd.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ea.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cl.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hu.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ad.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://ms.haigaiapp.cn

Ruby: arr.index(x)
来源：http://ti.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://jh.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://tk.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mz.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tf.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://wb.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://wb.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jk.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uv.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gc.shtwfgs.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://av.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://hy.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jc.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://df.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://of.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://mg.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://oc.szxytkj.cn

Go:   // 手写循环
来源：http://lo.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yk.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sq.nszjky.cn

[D15] 去重
来源：http://jx.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nc.hahajie.cn

PHP:  array_unique($arr);
来源：http://mz.asd995.cn

JS:   [...new Set(arr)]
来源：http://kb.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://rf.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zo.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ry.shxzukj.cn

Ruby: arr.uniq
来源：http://ze.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://yc.huixiangedu.cn

[D16] 求和与平均值
来源：http://sa.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pw.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zx.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ut.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hx.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xr.szsharing.cn

Go:   // 手写循环累加
来源：http://kd.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jp.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ke.gzmigu.cn

[D17] 最大值与最小值
来源：http://yq.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://pr.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://ka.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vb.asd995.cn

TS:   Math.max(...arr);
来源：http://fk.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sn.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rn.haigaiapp.cn

Ruby: arr.max;  arr.min
来源：http://yx.jianghongdianzi.cn

C#:   list.Max();  list.Min()
来源：http://jr.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://np.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hd.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://ul.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nh.szsharing.cn

TS:   nested.flat();
来源：http://cb.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ea.haigaiapp.cn

Go:   // 手写双层循环
来源：http://kr.huanxung.cn

Ruby: nested.flatten
来源：http://qk.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ms.hnjuh.cn

[D19] 按字段分组
来源：http://ij.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tc.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jt.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://um.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://em.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wz.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://zi.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oq.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kl.shtwfgs.cn

[D20] 统计每个元素出现次数
来源：http://mi.nszjky.cn

Py:   Counter(arr)
来源：http://qk.hahajie.cn

PHP:  array_count_values($arr);
来源：http://cv.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zf.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eb.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mc.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://hj.szxytkj.cn

Ruby: arr.tally
来源：http://ga.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uo.colortex.cn

[D21] 判断是否包含某元素
来源：http://bl.521024.cn

Py:   x in arr
来源：http://or.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://uf.hnjuh.cn

JS:   arr.includes(x)
来源：http://xq.asd995.cn

TS:   arr.includes(x)
来源：http://yl.9csxet.cn

Java: list.contains(x)
来源：http://no.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://dt.hnjuh.cn

Ruby: arr.include?(x)
来源：http://xf.shtwfgs.cn

C#:   list.Contains(x)
来源：http://su.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://mr.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ly.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ka.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uv.bjjhwx.cn

TS:   [...arr];
来源：http://cn.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://sb.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://pl.lnxyls.cn

Ruby: arr.dup;  arr.clone
来源：http://jh.huixiangedu.cn

C#:   new List<int>(list);
来源：http://cn.huixiangedu.cn

[D23] reduce 累积计算
来源：http://zh.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bc.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cd.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zp.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vc.jctech888.com.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xe.newstarts.cn

Go:   // 手写循环
来源：http://ty.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pb.asd995.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gk.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://dt.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wj.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jx.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ln.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vl.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xs.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jc.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tt.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zh.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://hz.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xf.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lh.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://im.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://za.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pa.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://br.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bk.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ld.gzmigu.cn

[D26] 数组转字符串
来源：http://ed.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://za.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://mp.asd995.cn

JS:   arr.join(", ")
来源：http://uu.jctech888.com.cn

TS:   arr.join(", ")
来源：http://sh.nszjky.cn

Java: String.join(", ", list)
来源：http://js.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://yh.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://nv.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://cv.gzmigu.cn

================================================================================
来源：http://kt.jianghongdianzi.cn

E. 字符串处理
来源：http://eq.gzmigu.cn

================================================================================
来源：http://ne.newstarts.cn

[E01] 拼接字符串
来源：http://uu.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ek.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yl.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nx.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aq.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nq.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tx.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dg.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xe.wgjwhj.cn

[E02] 重复字符串
来源：http://va.colortex.cn

Py:   "ab" * 3
来源：http://dt.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://yp.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://me.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://by.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://on.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://rp.newstarts.cn

Ruby: "ab" * 3
来源：http://ay.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dd.jctech888.com.cn

[E03] 截取子串
来源：http://qi.shxzskj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bi.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nl.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ej.nszjky.cn

TS:   s.slice(1, 4)
来源：http://rq.huanxung.cn

Java: s.substring(1, 4)
来源：http://ic.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://md.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mf.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://zw.bjjhwx.cn

[E04] 查找子串位置
来源：http://qq.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://iz.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://pv.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://al.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://ve.asd995.cn

Java: s.indexOf("x")
来源：http://rj.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://pi.hnjuh.cn

Ruby: s.index("x")
来源：http://yv.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://mz.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ht.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dk.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gd.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lu.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sl.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xq.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ha.shxzukj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://re.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yu.shxzukj.cn

[E06] 替换子串
来源：http://jo.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lr.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://qe.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cd.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://hp.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://om.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qk.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iv.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://bf.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://qv.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ky.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pf.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gt.521024.cn

TS:   s.split(",")
来源：http://kn.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kp.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ws.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://lo.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rj.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://pv.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://xj.newstarts.cn

PHP:  implode(",", $items);
来源：http://qu.huixiangedu.cn

JS:   items.join(",")
来源：http://tr.chemitech.net.cn

TS:   items.join(",")
来源：http://fv.shxzukj.cn

Java: String.join(",", items)
来源：http://fm.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://gy.9csxet.cn

Ruby: items.join(",")
来源：http://oe.hnjuh.cn

C#:   string.Join(",", items)
来源：http://ay.szxytkj.cn

[E09] 去除所有空白字符
来源：http://ks.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lz.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rg.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://tu.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://iv.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://zs.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nh.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kj.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bs.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://zs.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lq.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oe.521024.cn

JS:   "7".padStart(3, "0")
来源：http://dq.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://uj.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://cl.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ld.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kq.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ym.wgjwhj.cn

[E11] 反转字符串
来源：http://et.shxzukj.cn

Py:   s[::-1]
来源：http://bi.asd995.cn

PHP:  strrev($s);
来源：http://im.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://ab.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://li.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aq.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xu.nszjky.cn

Ruby: s.reverse
来源：http://da.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ke.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://pw.nszjky.cn

Py:   s.count("a")
来源：http://ms.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ov.521024.cn

JS:   s.split("a").length - 1
来源：http://iv.shtwfgs.cn

TS:   s.split("a").length - 1
来源：http://nu.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nq.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ms.nszjky.cn

Ruby: s.count("a")
来源：http://kq.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://oy.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://nj.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://mt.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sp.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://du.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ig.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://au.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gc.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gu.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://co.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://vq.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gz.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fn.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gs.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ek.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eb.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ep.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dh.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pq.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://fw.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sj.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hf.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://op.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qd.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vf.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://py.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fo.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qk.gzmigu.cn

[E16] 数字千分位
来源：http://hg.asd995.cn

Py:   f"{1234567:,}"
来源：http://vp.huixiangedu.cn


<!-- 参考信息 -->