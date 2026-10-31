代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jm.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://ub.asd995.cn

Ruby: nested.flatten
来源：http://ng.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ph.panjiajie.cn

[D19] 按字段分组
来源：http://bd.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dr.bookmarksfly.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ut.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eq.haigaiapp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yc.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fg.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://cx.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ju.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kk.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://ed.521024.cn

Py:   Counter(arr)
来源：http://wf.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://jr.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sm.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nf.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gn.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://ir.gzmigu.cn

Ruby: arr.tally
来源：http://sp.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://at.hnjuh.cn

[D21] 判断是否包含某元素
来源：http://sc.asd995.cn

Py:   x in arr
来源：http://pd.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://qq.huixiangedu.cn

JS:   arr.includes(x)
来源：http://vc.nszjky.cn

TS:   arr.includes(x)
来源：http://lr.yuexingan06.cn

Java: list.contains(x)
来源：http://sk.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://on.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://cm.wgjwhj.cn

C#:   list.Contains(x)
来源：http://rd.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://oj.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ik.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qh.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lr.jctech888.com.cn

TS:   [...arr];
来源：http://lf.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://ke.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dj.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://gn.huanxung.cn

C#:   new List<int>(list);
来源：http://of.shtwfgs.cn

[D23] reduce 累积计算
来源：http://cx.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ea.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mz.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mj.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hj.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ic.huanxung.cn

Go:   // 手写循环
来源：http://ch.haigaiapp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zk.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ua.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://oy.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gy.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rq.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uj.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yt.yuntaijiaju.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fs.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qy.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mr.jianghongdianzi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wp.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://xg.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ee.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oc.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ir.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ic.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ul.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://un.huixiangedu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ey.newstarts.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gb.chemitech.net.cn

[D26] 数组转字符串
来源：http://qf.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://ht.lnxyls.cn

PHP:  implode(", ", $arr);
来源：http://cf.bjjhwx.cn

JS:   arr.join(", ")
来源：http://ih.lnxyls.cn

TS:   arr.join(", ")
来源：http://av.wgjwhj.cn

Java: String.join(", ", list)
来源：http://pf.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://zz.huanxung.cn

Ruby: arr.join(", ")
来源：http://dh.521024.cn

C#:   string.Join(", ", list)
来源：http://cl.chemitech.net.cn

================================================================================
来源：http://ud.szsharing.cn

E. 字符串处理
来源：http://ig.newstarts.cn

================================================================================
来源：http://ia.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://fc.jianghongdianzi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://po.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zz.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://di.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hm.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uq.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tp.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yq.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://og.muxihuayi.cn

[E02] 重复字符串
来源：http://gk.gzmigu.cn

Py:   "ab" * 3
来源：http://re.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://hr.hahajie.cn

JS:   "ab".repeat(3)
来源：http://gg.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://fb.shxzskj.cn

Java: "ab".repeat(3)
来源：http://zw.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://jf.shxzukj.cn

Ruby: "ab" * 3
来源：http://mq.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ki.gzmigu.cn

[E03] 截取子串
来源：http://rs.colortex.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ri.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fc.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gz.asd995.cn

TS:   s.slice(1, 4)
来源：http://qy.panjiajie.cn

Java: s.substring(1, 4)
来源：http://hn.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yi.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yn.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://mf.szxytkj.cn

[E04] 查找子串位置
来源：http://zt.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://kc.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://lj.hahajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ll.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://dd.huixiangedu.cn

Java: s.indexOf("x")
来源：http://mn.521024.cn

Go:   strings.Index(s, "x")
来源：http://dz.yuexingan06.cn

Ruby: s.index("x")
来源：http://qk.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://rl.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sx.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mp.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sc.wgjwhj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tm.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yp.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zu.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sb.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ms.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ks.hnjuh.cn

[E06] 替换子串
来源：http://cx.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lu.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ys.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ew.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://xc.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zf.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ik.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yh.nszjky.cn

C#:   s.Replace("a", "b")
来源：http://mv.gzmigu.cn

[E07] 按分隔符拆分
来源：http://nu.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://an.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yl.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rx.asd995.cn

TS:   s.split(",")
来源：http://ak.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xq.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://de.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://vp.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zz.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://vc.hnjuh.cn

Py:   ",".join(items)
来源：http://qk.hnjuh.cn

PHP:  implode(",", $items);
来源：http://gq.panjiajie.cn

JS:   items.join(",")
来源：http://ra.9csxet.cn

TS:   items.join(",")
来源：http://ri.colortex.cn

Java: String.join(",", items)
来源：http://of.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://eq.colortex.cn

Ruby: items.join(",")
来源：http://ep.hnjuh.cn

C#:   string.Join(",", items)
来源：http://pp.newstarts.cn

[E09] 去除所有空白字符
来源：http://uy.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bl.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lz.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://mo.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://yf.huixiangedu.cn

Java: s.replaceAll("\\s+", "")
来源：http://yo.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vv.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cj.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zn.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://qk.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uz.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://se.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://dc.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://wc.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://si.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tt.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ny.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xa.lnxyls.cn

[E11] 反转字符串
来源：http://hj.huixiangedu.cn

Py:   s[::-1]
来源：http://rr.nszjky.cn

PHP:  strrev($s);
来源：http://dd.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://rp.colortex.cn

TS:   [...s].reverse().join("")
来源：http://wc.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ir.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://si.shtwfgs.cn

Ruby: s.reverse
来源：http://to.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ep.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://mz.hahajie.cn

Py:   s.count("a")
来源：http://ol.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://dm.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://rz.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://hi.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pz.yuexingan06.cn

Go:   strings.Count(s, "a")
来源：http://fm.huixiangedu.cn

Ruby: s.count("a")
来源：http://hn.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://iw.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://yt.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://ze.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ps.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fw.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wn.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://px.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lt.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ye.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pb.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://aq.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oj.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vw.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jq.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fa.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://on.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ui.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aq.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jv.521024.cn

[E15] HTML 转义 / 反转义
来源：http://zx.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zg.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xf.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ai.bookmarksfly.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qn.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eu.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ih.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aj.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nw.hnjuh.cn

[E16] 数字千分位
来源：http://pk.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://fu.gzmigu.cn

PHP:  number_format(1234567);
来源：http://oa.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uf.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bz.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fh.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ps.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ug.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://lv.asd995.cn

[E17] 首字母大写
来源：http://bx.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rd.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wy.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lm.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wt.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nc.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cd.szsharing.cn

Ruby: s.capitalize
来源：http://po.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bj.colortex.cn

[E18] 模板占位符替换
来源：http://iy.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ak.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ce.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qu.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ad.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iw.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ic.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ul.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vr.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://sa.szsharing.cn

Py:   s.splitlines()
来源：http://th.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ah.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://sx.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://ol.shtwfgs.cn

Java: s.lines().toList()
来源：http://ck.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://ek.newstarts.cn

Ruby: s.lines
来源：http://ut.szsharing.cn

C#:   s.Split('\n')
来源：http://xd.colortex.cn

[E20] 判断字符串是否为空
来源：http://ql.huanxung.cn

Py:   if not s:
来源：http://xf.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zk.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oe.lnxyls.cn

TS:   if (s === "") {}
来源：http://jz.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://dg.shxzukj.cn

Go:   if s == "" {}
来源：http://la.muxihuayi.cn

Ruby: if s.empty?
来源：http://cj.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lx.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://im.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mw.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ov.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://au.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fq.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lh.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://wi.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dm.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mn.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://hy.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://so.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ue.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ea.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eu.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bw.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hb.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://ka.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ew.panjiajie.cn

================================================================================
来源：http://qn.chemitech.net.cn

F. 文件与目录
来源：http://mi.shxzukj.cn

================================================================================
来源：http://ff.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://uw.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sh.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://sa.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wm.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://os.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bo.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ku.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://mq.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://oe.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://gc.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jv.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kn.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cm.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://po.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nv.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xy.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://es.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ar.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ur.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ba.hnjuh.cn


<!-- 参考信息 -->