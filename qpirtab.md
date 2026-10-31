代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sb.szxytkj.cn

JS:   arr.filter(x => x > 3)
来源：http://te.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://ho.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ny.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tj.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fn.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eu.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://ol.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hk.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vm.huanxung.cn

JS:   arr.map(x => x * 2)
来源：http://ux.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://yu.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gy.nicolike.cn

Go:   // 手写循环
来源：http://jf.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zw.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fc.shtwfgs.cn

[D15] 去重
来源：http://ei.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cx.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://nd.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://kx.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://ci.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ih.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rc.haigaiapp.cn

Ruby: arr.uniq
来源：http://nf.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://zx.9csxet.cn

[D16] 求和与平均值
来源：http://nq.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tl.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bb.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lr.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iy.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lx.lnxyls.cn

Go:   // 手写循环累加
来源：http://fg.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fd.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://vz.shtwfgs.cn

[D17] 最大值与最小值
来源：http://tq.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://nh.gzmigu.cn

PHP:  max($arr);  min($arr);
来源：http://qz.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vs.lnxyls.cn

TS:   Math.max(...arr);
来源：http://lf.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xx.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://js.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://ah.521024.cn

C#:   list.Max();  list.Min()
来源：http://cc.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://bo.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xg.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://xe.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pr.chemitech.net.cn

TS:   nested.flat();
来源：http://sm.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rr.szxytkj.cn

Go:   // 手写双层循环
来源：http://db.lnxyls.cn

Ruby: nested.flatten
来源：http://jx.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dy.bookmarksfly.cn

[D19] 按字段分组
来源：http://lm.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kh.chemitech.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pm.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bz.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vh.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sw.jctech888.com.cn

Go:   // 手写 map[string][]T
来源：http://fs.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://po.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nk.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://wh.muxihuayi.cn

Py:   Counter(arr)
来源：http://vw.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://iq.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pm.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gz.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://la.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://xo.asd995.cn

Ruby: arr.tally
来源：http://si.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://te.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://yp.nszjky.cn

Py:   x in arr
来源：http://tv.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://oj.panjiajie.cn

JS:   arr.includes(x)
来源：http://dq.szsharing.cn

TS:   arr.includes(x)
来源：http://wy.muxihuayi.cn

Java: list.contains(x)
来源：http://np.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://pt.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://bb.hahajie.cn

C#:   list.Contains(x)
来源：http://dw.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://kt.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hi.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nc.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ks.szxytkj.cn

TS:   [...arr];
来源：http://km.asd995.cn

Java: new ArrayList<>(list);
来源：http://id.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wk.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://wh.jctech888.com.cn

C#:   new List<int>(list);
来源：http://rm.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://jk.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://om.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cf.jctech888.com.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://os.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fs.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://to.newstarts.cn

Go:   // 手写循环
来源：http://lh.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://th.newstarts.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ti.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://wd.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kz.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ej.yuntaijiaju.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bq.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iz.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sz.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sb.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ie.jctech888.com.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zq.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://jz.asd995.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lx.chemitech.net.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hc.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bg.hnjuh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ry.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dd.szxytkj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://df.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hv.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://si.lnxyls.cn

[D26] 数组转字符串
来源：http://nq.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://ul.hahajie.cn

PHP:  implode(", ", $arr);
来源：http://bc.szxytkj.cn

JS:   arr.join(", ")
来源：http://vy.colortex.cn

TS:   arr.join(", ")
来源：http://no.shxzukj.cn

Java: String.join(", ", list)
来源：http://wc.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://mh.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://ns.colortex.cn

C#:   string.Join(", ", list)
来源：http://xs.yuexingan06.cn

================================================================================
来源：http://vf.nszjky.cn

E. 字符串处理
来源：http://ix.hnjuh.cn

================================================================================
来源：http://bd.lnxyls.cn

[E01] 拼接字符串
来源：http://fa.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pe.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uf.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qo.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lw.muxihuayi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kr.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lr.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://va.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yu.huanxung.cn

[E02] 重复字符串
来源：http://pk.nicolike.cn

Py:   "ab" * 3
来源：http://ti.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://ms.nszjky.cn

JS:   "ab".repeat(3)
来源：http://oy.hahajie.cn

TS:   "ab".repeat(3)
来源：http://bo.asd995.cn

Java: "ab".repeat(3)
来源：http://iw.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://zw.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://lk.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://of.newstarts.cn

[E03] 截取子串
来源：http://yz.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zo.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dw.yuntaijiaju.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mv.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://ee.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://tz.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://es.asd995.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xr.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://eq.huanxung.cn

[E04] 查找子串位置
来源：http://gj.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://oo.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://vh.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ng.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://az.bjjhwx.cn

Java: s.indexOf("x")
来源：http://gc.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://tz.asd995.cn

Ruby: s.index("x")
来源：http://qw.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://jl.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wg.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://az.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zv.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jn.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eb.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bk.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bz.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lt.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eb.panjiajie.cn

[E06] 替换子串
来源：http://ke.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gh.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://bv.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rw.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://yf.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sj.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dy.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ez.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://et.asd995.cn

[E07] 按分隔符拆分
来源：http://bu.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rb.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pb.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fk.huanxung.cn

TS:   s.split(",")
来源：http://ji.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pu.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wb.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://qe.shxzukj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://is.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://tp.asd995.cn

Py:   ",".join(items)
来源：http://xl.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://nl.huixiangedu.cn

JS:   items.join(",")
来源：http://dm.shxzskj.cn

TS:   items.join(",")
来源：http://dk.hahajie.cn

Java: String.join(",", items)
来源：http://dy.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://dc.shtwfgs.cn

Ruby: items.join(",")
来源：http://tq.gzmigu.cn

C#:   string.Join(",", items)
来源：http://oc.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://jv.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pw.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cb.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://nj.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ym.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://tq.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vz.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dv.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pi.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://zw.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://an.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ds.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://et.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://vl.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://lu.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pi.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nl.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ca.nszjky.cn

[E11] 反转字符串
来源：http://du.hnjuh.cn

Py:   s[::-1]
来源：http://hw.shxzukj.cn

PHP:  strrev($s);
来源：http://dq.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://pt.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://mg.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ef.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ge.huixiangedu.cn

Ruby: s.reverse
来源：http://ie.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wv.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://ud.hahajie.cn

Py:   s.count("a")
来源：http://bs.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://xi.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://pm.nicolike.cn

TS:   s.split("a").length - 1
来源：http://yb.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ws.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://uv.shxzskj.cn

Ruby: s.count("a")
来源：http://ej.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://jd.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://zc.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://cu.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lc.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kp.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sx.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://id.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eq.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pq.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://za.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://tv.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uo.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wi.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ik.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rg.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fp.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vw.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gr.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qa.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://cu.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sw.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fp.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iq.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fs.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cl.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sf.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ge.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ma.yuexingan06.cn

[E16] 数字千分位
来源：http://hi.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://jm.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ce.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ub.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ji.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zd.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fk.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kx.colortex.cn

C#:   1234567.ToString("N0")
来源：http://ts.newstarts.cn

[E17] 首字母大写
来源：http://so.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wx.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kd.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wy.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ct.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lr.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fn.9csxet.cn

Ruby: s.capitalize
来源：http://xm.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fb.asd995.cn

[E18] 模板占位符替换
来源：http://gj.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fn.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fn.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://km.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wy.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ny.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ea.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://px.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tl.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://yk.521024.cn

Py:   s.splitlines()
来源：http://da.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jz.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://jh.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://kp.nicolike.cn

Java: s.lines().toList()
来源：http://mk.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://ka.521024.cn

Ruby: s.lines
来源：http://ki.bjjhwx.cn

C#:   s.Split('\n')
来源：http://mf.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://hn.gzmigu.cn

Py:   if not s:
来源：http://me.hnjuh.cn


<!-- 参考信息 -->