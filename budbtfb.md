代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://li.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hm.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nn.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://ss.muxihuayi.cn

Ruby: arr.index(x)
来源：http://gz.bookmarksfly.cn

C#:   list.IndexOf(x);
来源：http://pi.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://sf.hahajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cj.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rr.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://jn.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://nc.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kx.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xs.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sr.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xb.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://as.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ab.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ps.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://em.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://ek.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tl.colortex.cn

Go:   // 手写循环
来源：http://xi.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ro.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ii.muxihuayi.cn

[D15] 去重
来源：http://qo.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hc.huanxung.cn

PHP:  array_unique($arr);
来源：http://gu.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://we.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://gw.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fu.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rf.yuexingan06.cn

Ruby: arr.uniq
来源：http://oc.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://pu.chemitech.net.cn

[D16] 求和与平均值
来源：http://bc.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kz.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ck.shtwfgs.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sy.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cy.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wn.shtwfgs.cn

Go:   // 手写循环累加
来源：http://vl.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pz.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://pi.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://vb.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://lc.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://lj.nszjky.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ke.huanxung.cn

TS:   Math.max(...arr);
来源：http://lc.hnjuh.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bi.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ra.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://ay.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://cq.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://he.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yq.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://yk.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://im.hnjuh.cn

TS:   nested.flat();
来源：http://bz.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rq.szxytkj.cn

Go:   // 手写双层循环
来源：http://sp.bjjhwx.cn

Ruby: nested.flatten
来源：http://sk.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://md.yuntaijiaju.cn

[D19] 按字段分组
来源：http://vj.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mm.muxihuayi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qw.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fu.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rn.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hw.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://dg.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pt.asd995.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ha.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://ll.nicolike.cn

Py:   Counter(arr)
来源：http://su.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://gw.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://no.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xj.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ip.hahajie.cn

Go:   // 手写 map[T]int
来源：http://ad.521024.cn

Ruby: arr.tally
来源：http://dt.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ne.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://ya.yuntaijiaju.cn

Py:   x in arr
来源：http://mc.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://go.nicolike.cn

JS:   arr.includes(x)
来源：http://ts.szxytkj.cn

TS:   arr.includes(x)
来源：http://dn.haigaiapp.cn

Java: list.contains(x)
来源：http://hh.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://xc.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://zy.lnxyls.cn

C#:   list.Contains(x)
来源：http://bp.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://xu.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lf.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ad.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iw.9csxet.cn

TS:   [...arr];
来源：http://ql.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://qj.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qa.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://jt.huanxung.cn

C#:   new List<int>(list);
来源：http://tq.huixiangedu.cn

[D23] reduce 累积计算
来源：http://uw.bookmarksfly.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ec.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wm.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ve.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kl.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://im.yuntaijiaju.cn

Go:   // 手写循环
来源：http://dt.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dh.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zc.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://mk.wgjwhj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://al.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ye.panjiajie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ni.haigaiapp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vd.9csxet.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rd.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wq.hnjuh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://da.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mq.wgjwhj.cn

[D25] Set 集合去重与交并差
来源：http://gy.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://co.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sk.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bd.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cu.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mk.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uw.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wv.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hl.huixiangedu.cn

[D26] 数组转字符串
来源：http://hl.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://me.521024.cn

PHP:  implode(", ", $arr);
来源：http://wb.colortex.cn

JS:   arr.join(", ")
来源：http://xp.huanxung.cn

TS:   arr.join(", ")
来源：http://on.nszjky.cn

Java: String.join(", ", list)
来源：http://on.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://ug.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://km.colortex.cn

C#:   string.Join(", ", list)
来源：http://em.huixinmuqiang.cn

================================================================================
来源：http://lh.chemitech.net.cn

E. 字符串处理
来源：http://by.9csxet.cn

================================================================================
来源：http://mb.muxihuayi.cn

[E01] 拼接字符串
来源：http://ec.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wu.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zg.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ls.521024.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://es.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vz.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ub.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tg.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yb.newstarts.cn

[E02] 重复字符串
来源：http://dh.nszjky.cn

Py:   "ab" * 3
来源：http://xe.wgjwhj.cn

PHP:  str_repeat("ab", 3);
来源：http://bb.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://eh.nszjky.cn

TS:   "ab".repeat(3)
来源：http://pz.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://sj.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://ky.muxihuayi.cn

Ruby: "ab" * 3
来源：http://ir.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qx.nicolike.cn

[E03] 截取子串
来源：http://vs.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://az.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ks.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zq.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://pi.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://ij.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ve.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pk.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ur.nicolike.cn

[E04] 查找子串位置
来源：http://rr.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://ki.nicolike.cn

PHP:  strpos($s, "x");
来源：http://vd.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xh.hahajie.cn

TS:   s.indexOf("x")
来源：http://wn.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://uq.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://go.nszjky.cn

Ruby: s.index("x")
来源：http://hg.newstarts.cn

C#:   s.IndexOf("x")
来源：http://wz.shxzukj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oz.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xu.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xc.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pt.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ao.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uy.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tc.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yt.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gx.hnjuh.cn

[E06] 替换子串
来源：http://fo.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://df.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://cc.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://um.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://aq.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bq.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xc.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ec.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://io.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://bp.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oa.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jg.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ke.shxzskj.cn

TS:   s.split(",")
来源：http://pv.nicolike.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gu.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fk.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://el.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://di.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://zx.shxzukj.cn

Py:   ",".join(items)
来源：http://ez.szsharing.cn

PHP:  implode(",", $items);
来源：http://yf.nicolike.cn

JS:   items.join(",")
来源：http://jq.newstarts.cn

TS:   items.join(",")
来源：http://ms.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://qi.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://an.huixiangedu.cn

Ruby: items.join(",")
来源：http://gg.shxzskj.cn

C#:   string.Join(",", items)
来源：http://ak.hnjuh.cn

[E09] 去除所有空白字符
来源：http://mt.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://av.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lu.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://ju.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://ty.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://cm.nszjky.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cr.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xk.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rx.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://jq.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vo.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mm.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://qz.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://mf.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://qc.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hm.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ze.yuexingan06.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sd.hnjuh.cn

[E11] 反转字符串
来源：http://nv.gzmigu.cn

Py:   s[::-1]
来源：http://yu.lnxyls.cn

PHP:  strrev($s);
来源：http://ma.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://kt.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://vg.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rf.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lj.bjjhwx.cn

Ruby: s.reverse
来源：http://hg.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pw.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://ic.hahajie.cn

Py:   s.count("a")
来源：http://xn.colortex.cn

PHP:  substr_count($s, "a");
来源：http://qc.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://ns.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://li.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xz.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://px.yuexingan06.cn

Ruby: s.count("a")
来源：http://xt.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://fd.shxzukj.cn

[E13] 逐字符遍历
来源：http://az.colortex.cn

Py:   for ch in s: print(ch)
来源：http://bi.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yl.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://im.bookmarksfly.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sa.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gb.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gn.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zx.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jf.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://oa.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yt.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dv.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gk.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yl.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://za.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hx.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ne.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fi.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://hr.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://he.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xw.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xx.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nx.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ge.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xp.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tu.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vq.bjjhwx.cn

[E16] 数字千分位
来源：http://wp.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://iy.hahajie.cn

PHP:  number_format(1234567);
来源：http://fk.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iv.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ab.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ji.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rv.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tc.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ip.panjiajie.cn

[E17] 首字母大写
来源：http://ou.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://km.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cl.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tg.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xq.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xo.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ta.hahajie.cn

Ruby: s.capitalize
来源：http://ut.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://km.panjiajie.cn

[E18] 模板占位符替换
来源：http://hl.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mj.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ty.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://um.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://da.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://er.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vc.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://im.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gi.asd995.cn

[E19] 多行文本按行拆分
来源：http://uw.szsharing.cn

Py:   s.splitlines()
来源：http://mp.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://on.chemitech.net.cn


<!-- 参考信息 -->