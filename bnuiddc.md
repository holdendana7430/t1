代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gm.huixiangedu.cn

Ruby: arr.sort
来源：http://vy.chemitech.net.cn

C#:   list.Sort();
来源：http://kb.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ka.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kg.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xq.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ty.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bv.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hg.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tw.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zo.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ui.huixinmuqiang.cn

[D11] 反转数组
来源：http://sy.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ox.shxzskj.cn

PHP:  array_reverse($arr);
来源：http://jy.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ay.huanxung.cn

TS:   [...arr].reverse();
来源：http://vo.szxytkj.cn

Java: Collections.reverse(list);
来源：http://vz.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://ru.haigaiapp.cn

Ruby: arr.reverse
来源：http://ty.bookmarksfly.cn

C#:   list.Reverse();
来源：http://ky.lnxyls.cn

[D12] 查找元素下标
来源：http://cb.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://ge.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://am.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sp.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ps.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eg.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://yd.chemitech.net.cn

Ruby: arr.index(x)
来源：http://uq.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://ku.haigaiapp.cn

[D13] 过滤（保留满足条件的）
来源：http://zc.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fr.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yo.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://ww.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://uo.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wh.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vg.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nv.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ya.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://aj.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dz.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ow.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://ps.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://cc.hnjuh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ek.huixinmuqiang.cn

Go:   // 手写循环
来源：http://rz.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kh.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://px.lnxyls.cn

[D15] 去重
来源：http://fv.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lf.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://gw.9csxet.cn

JS:   [...new Set(arr)]
来源：http://lx.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://xw.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://we.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cu.shtwfgs.cn

Ruby: arr.uniq
来源：http://uc.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://nb.huanxung.cn

[D16] 求和与平均值
来源：http://zz.szsharing.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cp.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mo.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nd.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rb.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ll.nicolike.cn

Go:   // 手写循环累加
来源：http://ix.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eu.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://xf.colortex.cn

[D17] 最大值与最小值
来源：http://uy.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://cg.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://ro.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ib.shxzskj.cn

TS:   Math.max(...arr);
来源：http://td.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xc.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mr.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://bf.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://qa.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://mf.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yf.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://tq.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gh.bookmarksfly.cn

TS:   nested.flat();
来源：http://np.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zh.lnxyls.cn

Go:   // 手写双层循环
来源：http://pw.yuexingan06.cn

Ruby: nested.flatten
来源：http://na.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ys.yuexingan06.cn

[D19] 按字段分组
来源：http://fi.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lx.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://is.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ny.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jt.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ra.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://sy.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bb.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cv.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://ul.asd995.cn

Py:   Counter(arr)
来源：http://ij.newstarts.cn

PHP:  array_count_values($arr);
来源：http://lv.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lr.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tj.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eo.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://pl.colortex.cn

Ruby: arr.tally
来源：http://hl.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oq.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://oj.wgjwhj.cn

Py:   x in arr
来源：http://na.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://hw.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://sx.yuexingan06.cn

TS:   arr.includes(x)
来源：http://dv.chemitech.net.cn

Java: list.contains(x)
来源：http://tp.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://gv.gzmigu.cn

Ruby: arr.include?(x)
来源：http://jo.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://dx.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://op.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jk.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sk.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vm.muxihuayi.cn

TS:   [...arr];
来源：http://kl.asd995.cn

Java: new ArrayList<>(list);
来源：http://lr.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ud.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://wt.panjiajie.cn

C#:   new List<int>(list);
来源：http://pj.wgjwhj.cn

[D23] reduce 累积计算
来源：http://bq.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bg.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dc.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ql.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://if.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rz.nszjky.cn

Go:   // 手写循环
来源：http://yu.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://me.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wv.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://bs.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jq.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ar.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rw.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://le.jianghongdianzi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sl.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ti.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sk.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://of.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://dj.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kg.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hk.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ke.szxytkj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ui.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rr.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ex.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ft.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uq.shtwfgs.cn

[D26] 数组转字符串
来源：http://wg.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://wv.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://xi.szxytkj.cn

JS:   arr.join(", ")
来源：http://yj.9csxet.cn

TS:   arr.join(", ")
来源：http://fi.newstarts.cn

Java: String.join(", ", list)
来源：http://av.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://qz.gzmigu.cn

Ruby: arr.join(", ")
来源：http://mt.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://nf.yuntaijiaju.cn

================================================================================
来源：http://re.shxzskj.cn

E. 字符串处理
来源：http://mh.lnxyls.cn

================================================================================
来源：http://qa.newstarts.cn

[E01] 拼接字符串
来源：http://yx.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jr.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ph.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qb.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dk.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lu.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sq.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zj.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fl.lnxyls.cn

[E02] 重复字符串
来源：http://oa.yuntaijiaju.cn

Py:   "ab" * 3
来源：http://mj.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://re.9csxet.cn

JS:   "ab".repeat(3)
来源：http://xk.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://vi.bookmarksfly.cn

Java: "ab".repeat(3)
来源：http://hz.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://rv.szxytkj.cn

Ruby: "ab" * 3
来源：http://ws.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gq.bjjhwx.cn

[E03] 截取子串
来源：http://vd.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ld.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://py.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eu.9csxet.cn

TS:   s.slice(1, 4)
来源：http://wh.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://uo.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vu.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bi.521024.cn

C#:   s.Substring(1, 3)
来源：http://fw.gzmigu.cn

[E04] 查找子串位置
来源：http://du.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://hp.asd995.cn

PHP:  strpos($s, "x");
来源：http://ja.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ib.521024.cn

TS:   s.indexOf("x")
来源：http://cg.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://zo.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://qq.shtwfgs.cn

Ruby: s.index("x")
来源：http://zf.521024.cn

C#:   s.IndexOf("x")
来源：http://ee.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tp.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hb.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://it.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oj.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://un.jctech888.com.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bg.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gp.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fh.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ru.yuntaijiaju.cn

[E06] 替换子串
来源：http://no.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qb.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://gf.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uv.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://hc.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uo.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ti.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mg.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://li.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://zw.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jx.jctech888.com.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lr.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xt.bjjhwx.cn

TS:   s.split(",")
来源：http://ws.chemitech.net.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tt.bjjhwx.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zc.panjiajie.cn

Ruby: s.split(",");  s.split
来源：http://cd.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vp.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://yj.shxzukj.cn

Py:   ",".join(items)
来源：http://ej.newstarts.cn

PHP:  implode(",", $items);
来源：http://fk.shxzskj.cn

JS:   items.join(",")
来源：http://ib.huanxung.cn

TS:   items.join(",")
来源：http://fo.huanxung.cn

Java: String.join(",", items)
来源：http://yu.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://iq.jctech888.com.cn

Ruby: items.join(",")
来源：http://ht.asd995.cn

C#:   string.Join(",", items)
来源：http://ff.shxzskj.cn

[E09] 去除所有空白字符
来源：http://kl.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qi.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kh.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://xt.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://wg.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://pg.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ge.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rl.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wb.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ak.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zh.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ox.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://ps.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://bg.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://sb.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bi.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hv.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rn.huixiangedu.cn

[E11] 反转字符串
来源：http://mi.chemitech.net.cn

Py:   s[::-1]
来源：http://xk.wgjwhj.cn

PHP:  strrev($s);
来源：http://ss.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://xw.colortex.cn

TS:   [...s].reverse().join("")
来源：http://ta.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://eo.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ml.panjiajie.cn

Ruby: s.reverse
来源：http://xw.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wi.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://jf.yuntaijiaju.cn

Py:   s.count("a")
来源：http://ce.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://iq.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://nf.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://jd.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mj.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ko.jctech888.com.cn

Ruby: s.count("a")
来源：http://vh.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ql.hnjuh.cn

[E13] 逐字符遍历
来源：http://ur.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://hg.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xj.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kw.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gg.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kc.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uk.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wz.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://de.newstarts.cn

[E14] URL 编码与 Base64
来源：http://zh.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jd.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fy.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qm.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ll.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oa.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://on.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wa.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mx.521024.cn

[E15] HTML 转义 / 反转义
来源：http://bd.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jh.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uw.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://et.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://av.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cz.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fy.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pj.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ud.chemitech.net.cn

[E16] 数字千分位
来源：http://zh.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://mk.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://pd.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bt.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zp.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nz.hahajie.cn


<!-- 参考信息 -->