代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://da.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://yk.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gr.shxzukj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ym.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ic.asd995.cn

C#:   list.Max();  list.Min()
来源：http://ma.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://om.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wy.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://hs.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qf.gzmigu.cn

TS:   nested.flat();
来源：http://kg.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xh.newstarts.cn

Go:   // 手写双层循环
来源：http://gc.bookmarksfly.cn

Ruby: nested.flatten
来源：http://nj.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jv.shxzukj.cn

[D19] 按字段分组
来源：http://wz.szsharing.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ap.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://li.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cm.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aq.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sl.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://vl.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zg.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://is.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://sn.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://md.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://oc.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://po.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://js.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yb.colortex.cn

Go:   // 手写 map[T]int
来源：http://yz.521024.cn

Ruby: arr.tally
来源：http://ew.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kz.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://ie.yuexingan06.cn

Py:   x in arr
来源：http://kl.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://sp.muxihuayi.cn

JS:   arr.includes(x)
来源：http://nv.huanxung.cn

TS:   arr.includes(x)
来源：http://xe.521024.cn

Java: list.contains(x)
来源：http://fv.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://wl.gzmigu.cn

Ruby: arr.include?(x)
来源：http://vo.haigaiapp.cn

C#:   list.Contains(x)
来源：http://cd.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://qw.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sb.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fn.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sq.nszjky.cn

TS:   [...arr];
来源：http://ar.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://ha.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qx.bookmarksfly.cn

Ruby: arr.dup;  arr.clone
来源：http://us.szxytkj.cn

C#:   new List<int>(list);
来源：http://ff.asd995.cn

[D23] reduce 累积计算
来源：http://ii.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wh.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sz.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gt.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ej.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fb.szsharing.cn

Go:   // 手写循环
来源：http://pt.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gw.shtwfgs.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hb.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://rc.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ih.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iu.chemitech.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zu.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mo.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://um.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://la.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eu.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eo.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://qq.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ox.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ts.chemitech.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uk.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yc.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ck.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eq.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vc.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bm.haigaiapp.cn

[D26] 数组转字符串
来源：http://zl.jianghongdianzi.cn

Py:   ", ".join(map(str, arr))
来源：http://yh.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://ug.hnjuh.cn

JS:   arr.join(", ")
来源：http://nn.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://uz.521024.cn

Java: String.join(", ", list)
来源：http://ws.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://zo.newstarts.cn

Ruby: arr.join(", ")
来源：http://dz.chemitech.net.cn

C#:   string.Join(", ", list)
来源：http://el.9csxet.cn

================================================================================
来源：http://cu.huixinmuqiang.cn

E. 字符串处理
来源：http://oi.yuexingan06.cn

================================================================================
来源：http://ld.wgjwhj.cn

[E01] 拼接字符串
来源：http://on.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://km.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kc.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ad.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://za.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dz.huixiangedu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nx.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://da.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fu.huanxung.cn

[E02] 重复字符串
来源：http://su.lnxyls.cn

Py:   "ab" * 3
来源：http://dc.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://ox.hnjuh.cn

JS:   "ab".repeat(3)
来源：http://qz.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://ws.nicolike.cn

Java: "ab".repeat(3)
来源：http://gj.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://qi.chemitech.net.cn

Ruby: "ab" * 3
来源：http://nu.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pz.huixinmuqiang.cn

[E03] 截取子串
来源：http://ku.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zm.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://su.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gz.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://bc.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://ae.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vs.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cb.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://fr.yuexingan06.cn

[E04] 查找子串位置
来源：http://ww.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://gf.szsharing.cn

PHP:  strpos($s, "x");
来源：http://qe.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tw.newstarts.cn

TS:   s.indexOf("x")
来源：http://ak.muxihuayi.cn

Java: s.indexOf("x")
来源：http://ku.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://hb.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://ni.9csxet.cn

C#:   s.IndexOf("x")
来源：http://dm.9csxet.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yz.huanxung.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://na.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://en.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://be.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xi.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dh.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sf.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lx.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kq.jianghongdianzi.cn

[E06] 替换子串
来源：http://qb.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xe.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://zd.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ik.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://gx.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zi.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oq.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gq.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://ew.newstarts.cn

[E07] 按分隔符拆分
来源：http://cq.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gq.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iz.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mt.shtwfgs.cn

TS:   s.split(",")
来源：http://fo.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ku.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ym.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://oz.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cf.9csxet.cn

[E08] 数组按分隔符合并
来源：http://em.521024.cn

Py:   ",".join(items)
来源：http://lr.asd995.cn

PHP:  implode(",", $items);
来源：http://ye.szxytkj.cn

JS:   items.join(",")
来源：http://qn.newstarts.cn

TS:   items.join(",")
来源：http://jm.chemitech.net.cn

Java: String.join(",", items)
来源：http://rx.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://pg.shtwfgs.cn

Ruby: items.join(",")
来源：http://et.colortex.cn

C#:   string.Join(",", items)
来源：http://df.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://ao.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vu.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pd.muxihuayi.cn

JS:   s.replace(/\s+/g, "")
来源：http://wb.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://vd.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://sp.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cn.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pv.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mj.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://eu.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zd.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pn.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://sd.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://bk.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://to.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ik.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ci.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cv.wgjwhj.cn

[E11] 反转字符串
来源：http://je.chemitech.net.cn

Py:   s[::-1]
来源：http://xd.wgjwhj.cn

PHP:  strrev($s);
来源：http://it.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://sg.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://mw.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://va.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dk.9csxet.cn

Ruby: s.reverse
来源：http://wr.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iu.colortex.cn

[E12] 统计某字符出现次数
来源：http://xd.nicolike.cn

Py:   s.count("a")
来源：http://fa.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://hv.nszjky.cn

JS:   s.split("a").length - 1
来源：http://bz.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://cu.521024.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rz.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://qr.521024.cn

Ruby: s.count("a")
来源：http://pg.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://by.huanxung.cn

[E13] 逐字符遍历
来源：http://bp.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://ab.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vv.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gr.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pl.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://an.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fk.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://of.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fw.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://wi.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gq.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://la.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ro.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dr.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oy.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sc.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ta.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sf.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://jt.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://br.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rv.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rm.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://an.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://um.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ua.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xu.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ln.521024.cn

[E16] 数字千分位
来源：http://ye.newstarts.cn

Py:   f"{1234567:,}"
来源：http://vs.szsharing.cn

PHP:  number_format(1234567);
来源：http://dp.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ed.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rs.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sg.gzmigu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wu.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ta.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://ou.shxzskj.cn

[E17] 首字母大写
来源：http://ki.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gx.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://za.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fh.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fh.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tb.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kn.521024.cn

Ruby: s.capitalize
来源：http://ea.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cg.colortex.cn

[E18] 模板占位符替换
来源：http://cr.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://no.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ac.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cr.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fn.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ge.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://px.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ij.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://od.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://nm.szsharing.cn

Py:   s.splitlines()
来源：http://vc.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xu.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ly.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://ag.huixiangedu.cn

Java: s.lines().toList()
来源：http://pm.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://cj.bookmarksfly.cn

Ruby: s.lines
来源：http://ca.wgjwhj.cn

C#:   s.Split('\n')
来源：http://gl.chemitech.net.cn

[E20] 判断字符串是否为空
来源：http://me.newstarts.cn

Py:   if not s:
来源：http://ua.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qq.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ux.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://yz.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://gj.huixiangedu.cn

Go:   if s == "" {}
来源：http://ry.newstarts.cn

Ruby: if s.empty?
来源：http://mm.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ml.newstarts.cn

[E21] 超长截断加省略号
来源：http://vj.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sm.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mp.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sr.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xy.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qs.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://ly.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ge.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cn.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://kb.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://br.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gi.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ew.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mg.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://js.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ke.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://bn.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kg.szsharing.cn

================================================================================
来源：http://du.muxihuayi.cn

F. 文件与目录
来源：http://xv.nicolike.cn

================================================================================
来源：http://zv.chemitech.net.cn

[F01] 读取整个文件
来源：http://zr.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dr.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://sx.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oz.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yw.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xg.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fb.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://ek.huanxung.cn


<!-- 参考信息 -->