代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vt.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://yi.haigaiapp.cn

[D17] 最大值与最小值
来源：http://ct.9csxet.cn

Py:   max(arr);  min(arr)
来源：http://pq.521024.cn

PHP:  max($arr);  min($arr);
来源：http://pf.shtwfgs.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ya.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://da.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uz.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://du.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://fl.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://ip.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://ae.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vb.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://va.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vi.lnxyls.cn

TS:   nested.flat();
来源：http://bo.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mp.521024.cn

Go:   // 手写双层循环
来源：http://or.shtwfgs.cn

Ruby: nested.flatten
来源：http://iy.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ik.shxzukj.cn

[D19] 按字段分组
来源：http://jq.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hv.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ny.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lc.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://sz.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hn.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://rg.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cq.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pp.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://jj.jctech888.com.cn

Py:   Counter(arr)
来源：http://bm.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://sj.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sa.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qd.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cf.nszjky.cn

Go:   // 手写 map[T]int
来源：http://ik.hnjuh.cn

Ruby: arr.tally
来源：http://zx.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bc.hahajie.cn

[D21] 判断是否包含某元素
来源：http://gz.huixiangedu.cn

Py:   x in arr
来源：http://pe.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://np.panjiajie.cn

JS:   arr.includes(x)
来源：http://dv.huixiangedu.cn

TS:   arr.includes(x)
来源：http://gj.haigaiapp.cn

Java: list.contains(x)
来源：http://uz.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://ox.shxzskj.cn

Ruby: arr.include?(x)
来源：http://ws.nicolike.cn

C#:   list.Contains(x)
来源：http://qr.jctech888.com.cn

[D22] 复制数组（避免共享引用）
来源：http://po.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ae.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rt.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wk.muxihuayi.cn

TS:   [...arr];
来源：http://kj.asd995.cn

Java: new ArrayList<>(list);
来源：http://rb.jianghongdianzi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fz.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://vt.shxzskj.cn

C#:   new List<int>(list);
来源：http://ox.jianghongdianzi.cn

[D23] reduce 累积计算
来源：http://nl.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zg.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://au.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bz.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ct.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ye.521024.cn

Go:   // 手写循环
来源：http://oi.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zl.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qt.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://ir.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ap.yuexingan06.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://th.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rs.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xz.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hn.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uc.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kj.9csxet.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fg.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://ny.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ty.asd995.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ut.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rl.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oz.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ht.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bs.jianghongdianzi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kk.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ni.colortex.cn

[D26] 数组转字符串
来源：http://ly.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://py.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://lr.shxzskj.cn

JS:   arr.join(", ")
来源：http://nu.haigaiapp.cn

TS:   arr.join(", ")
来源：http://gu.shxzukj.cn

Java: String.join(", ", list)
来源：http://bj.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://wu.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://il.colortex.cn

C#:   string.Join(", ", list)
来源：http://rq.huanxung.cn

================================================================================
来源：http://zt.wgjwhj.cn

E. 字符串处理
来源：http://dh.gzmigu.cn

================================================================================
来源：http://bp.huixiangedu.cn

[E01] 拼接字符串
来源：http://xd.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ub.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bj.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mx.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oz.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bz.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qh.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://du.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://li.panjiajie.cn

[E02] 重复字符串
来源：http://mz.haigaiapp.cn

Py:   "ab" * 3
来源：http://ul.hahajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ba.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://vp.newstarts.cn

TS:   "ab".repeat(3)
来源：http://qm.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://sj.huixiangedu.cn

Go:   strings.Repeat("ab", 3)
来源：http://nv.bjjhwx.cn

Ruby: "ab" * 3
来源：http://nf.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ia.huanxung.cn

[E03] 截取子串
来源：http://xa.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wk.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ho.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nc.nicolike.cn

TS:   s.slice(1, 4)
来源：http://em.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://rm.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://my.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yz.colortex.cn

C#:   s.Substring(1, 3)
来源：http://cr.haigaiapp.cn

[E04] 查找子串位置
来源：http://gv.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://nf.521024.cn

PHP:  strpos($s, "x");
来源：http://lv.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gv.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://xv.huanxung.cn

Java: s.indexOf("x")
来源：http://ay.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://on.haigaiapp.cn

Ruby: s.index("x")
来源：http://gy.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://ep.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://za.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ji.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ty.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bj.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nf.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ky.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gx.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://af.yuntaijiaju.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jt.wgjwhj.cn

[E06] 替换子串
来源：http://wn.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rx.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://dy.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fo.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://dj.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ng.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lb.szsharing.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kr.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://uh.nszjky.cn

[E07] 按分隔符拆分
来源：http://hq.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rc.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://na.colortex.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fu.521024.cn

TS:   s.split(",")
来源：http://fu.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ig.lnxyls.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://at.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://dz.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bz.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://pl.wgjwhj.cn

Py:   ",".join(items)
来源：http://tl.shxzskj.cn

PHP:  implode(",", $items);
来源：http://dt.haigaiapp.cn

JS:   items.join(",")
来源：http://gz.shxzukj.cn

TS:   items.join(",")
来源：http://xc.bjjhwx.cn

Java: String.join(",", items)
来源：http://vu.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://jq.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://lt.nicolike.cn

C#:   string.Join(",", items)
来源：http://by.gzmigu.cn

[E09] 去除所有空白字符
来源：http://oo.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fp.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wh.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://cy.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://yq.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://xd.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ba.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ic.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zv.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://sv.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dk.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lp.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://di.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://sx.asd995.cn

Java: String.format("%03d", 7)
来源：http://jf.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vz.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cf.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ex.shxzskj.cn

[E11] 反转字符串
来源：http://ka.hahajie.cn

Py:   s[::-1]
来源：http://qt.nszjky.cn

PHP:  strrev($s);
来源：http://jd.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://td.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://sp.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yr.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hr.huanxung.cn

Ruby: s.reverse
来源：http://xd.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ab.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://ii.jctech888.com.cn

Py:   s.count("a")
来源：http://zp.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://wz.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://zk.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://ty.bjjhwx.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ey.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://dg.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://jf.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://jy.haigaiapp.cn

[E13] 逐字符遍历
来源：http://zc.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://at.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jc.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lh.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://po.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fi.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uu.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bv.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yg.jctech888.com.cn

[E14] URL 编码与 Base64
来源：http://ev.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xe.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zx.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ar.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oz.shtwfgs.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bj.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vv.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fs.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ft.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://fc.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jf.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kt.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nk.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wj.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qk.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cv.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://it.521024.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://on.bookmarksfly.cn

[E16] 数字千分位
来源：http://oi.nszjky.cn

Py:   f"{1234567:,}"
来源：http://qo.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://sz.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vq.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ff.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wo.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qo.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ol.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://eu.panjiajie.cn

[E17] 首字母大写
来源：http://ge.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pg.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sk.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tu.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hs.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://op.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ne.yuexingan06.cn

Ruby: s.capitalize
来源：http://yr.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ye.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://rx.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pv.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pd.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cb.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://na.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pg.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://us.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mn.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gu.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://lp.asd995.cn

Py:   s.splitlines()
来源：http://mg.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tr.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://fp.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://ri.nicolike.cn

Java: s.lines().toList()
来源：http://yw.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://rz.haigaiapp.cn

Ruby: s.lines
来源：http://uq.shtwfgs.cn

C#:   s.Split('\n')
来源：http://nb.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://xf.yuexingan06.cn

Py:   if not s:
来源：http://fh.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kt.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fb.nszjky.cn

TS:   if (s === "") {}
来源：http://ci.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://kk.panjiajie.cn

Go:   if s == "" {}
来源：http://hp.shxzukj.cn

Ruby: if s.empty?
来源：http://zf.nicolike.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ut.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://fn.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ax.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://av.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mz.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cy.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nz.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://yo.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qr.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://df.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://js.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://va.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ua.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dt.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jv.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gz.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bi.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://pc.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sa.nszjky.cn

================================================================================
来源：http://lo.jianghongdianzi.cn

F. 文件与目录
来源：http://hg.panjiajie.cn

================================================================================
来源：http://wa.chemitech.net.cn

[F01] 读取整个文件
来源：http://ea.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oe.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://pz.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vo.chemitech.net.cn


<!-- 参考信息 -->