代发 wailian999

Java: new ArrayList<>(list);
来源：http://ko.yuexingan06.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gw.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://pn.newstarts.cn

C#:   new List<int>(list);
来源：http://kg.shxzukj.cn

[D23] reduce 累积计算
来源：http://qh.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tc.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mu.gzmigu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sq.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cb.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tf.colortex.cn

Go:   // 手写循环
来源：http://gg.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oq.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sf.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://kh.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xh.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://di.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lz.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zj.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qc.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vj.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zl.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mv.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://sn.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nk.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rr.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ag.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://al.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vh.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hr.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pa.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kc.521024.cn

[D26] 数组转字符串
来源：http://mv.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://jp.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://cv.9csxet.cn

JS:   arr.join(", ")
来源：http://xl.hahajie.cn

TS:   arr.join(", ")
来源：http://hd.szsharing.cn

Java: String.join(", ", list)
来源：http://en.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://ot.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://lb.szxytkj.cn

C#:   string.Join(", ", list)
来源：http://de.chemitech.net.cn

================================================================================
来源：http://zv.muxihuayi.cn

E. 字符串处理
来源：http://dh.haigaiapp.cn

================================================================================
来源：http://lw.colortex.cn

[E01] 拼接字符串
来源：http://uy.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sv.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ag.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fy.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fn.yuntaijiaju.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mb.yuntaijiaju.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ee.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://to.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yu.gzmigu.cn

[E02] 重复字符串
来源：http://ji.chemitech.net.cn

Py:   "ab" * 3
来源：http://md.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://op.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://cg.9csxet.cn

TS:   "ab".repeat(3)
来源：http://pf.shxzskj.cn

Java: "ab".repeat(3)
来源：http://re.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://pq.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://ah.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gf.shtwfgs.cn

[E03] 截取子串
来源：http://ek.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uc.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ha.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pv.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://tm.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://zv.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fk.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ih.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://aj.gzmigu.cn

[E04] 查找子串位置
来源：http://gz.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://hh.bjjhwx.cn

PHP:  strpos($s, "x");
来源：http://eg.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bh.huanxung.cn

TS:   s.indexOf("x")
来源：http://gx.wgjwhj.cn

Java: s.indexOf("x")
来源：http://bu.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://dz.hahajie.cn

Ruby: s.index("x")
来源：http://de.9csxet.cn

C#:   s.IndexOf("x")
来源：http://go.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zw.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xn.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fb.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pt.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://al.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ig.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ac.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rc.shxzskj.cn

[E06] 替换子串
来源：http://ny.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rj.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://fa.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gz.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://mi.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ai.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qr.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eq.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://qt.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://lv.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gb.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tq.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lb.9csxet.cn

TS:   s.split(",")
来源：http://vo.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eq.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bd.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://ae.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fa.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://aw.bookmarksfly.cn

Py:   ",".join(items)
来源：http://vd.huanxung.cn

PHP:  implode(",", $items);
来源：http://tn.9csxet.cn

JS:   items.join(",")
来源：http://xf.huixiangedu.cn

TS:   items.join(",")
来源：http://ri.panjiajie.cn

Java: String.join(",", items)
来源：http://ch.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://ay.yuexingan06.cn

Ruby: items.join(",")
来源：http://hu.newstarts.cn

C#:   string.Join(",", items)
来源：http://aq.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://ie.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wz.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kp.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://hm.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://dp.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://xs.9csxet.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dj.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gn.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yo.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://nn.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cj.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eh.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://lx.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://li.521024.cn

Java: String.format("%03d", 7)
来源：http://lz.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://aj.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nv.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://al.shtwfgs.cn

[E11] 反转字符串
来源：http://ce.gzmigu.cn

Py:   s[::-1]
来源：http://xg.asd995.cn

PHP:  strrev($s);
来源：http://xi.shxzskj.cn

JS:   [...s].reverse().join("")
来源：http://zq.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://gs.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bt.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://li.gzmigu.cn

Ruby: s.reverse
来源：http://qh.shxzukj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ob.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://bl.asd995.cn

Py:   s.count("a")
来源：http://id.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ar.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://qu.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://ps.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xg.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://yg.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://po.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://rp.gzmigu.cn

[E13] 逐字符遍历
来源：http://gt.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://ap.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://be.bookmarksfly.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://or.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hs.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tm.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ix.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tf.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oa.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://zt.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eo.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rq.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bu.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tz.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qd.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ng.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fx.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ty.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://ux.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pp.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jw.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kp.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xk.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ec.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dn.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ow.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lb.muxihuayi.cn

[E16] 数字千分位
来源：http://pv.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://xi.shxzskj.cn

PHP:  number_format(1234567);
来源：http://xc.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zq.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hq.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rr.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zw.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sg.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://jk.gzmigu.cn

[E17] 首字母大写
来源：http://rn.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yy.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iq.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sh.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cp.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kx.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gx.hnjuh.cn

Ruby: s.capitalize
来源：http://jr.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fe.shtwfgs.cn

[E18] 模板占位符替换
来源：http://cy.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mg.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rs.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hw.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://az.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gh.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yr.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zw.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vh.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://ww.panjiajie.cn

Py:   s.splitlines()
来源：http://aw.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ys.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://bk.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://tf.521024.cn

Java: s.lines().toList()
来源：http://wo.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://bn.yuntaijiaju.cn

Ruby: s.lines
来源：http://rn.shtwfgs.cn

C#:   s.Split('\n')
来源：http://pj.hahajie.cn

[E20] 判断字符串是否为空
来源：http://ut.newstarts.cn

Py:   if not s:
来源：http://wj.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mt.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ne.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ve.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://xj.shxzukj.cn

Go:   if s == "" {}
来源：http://zi.huanxung.cn

Ruby: if s.empty?
来源：http://tj.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ma.shxzskj.cn

[E21] 超长截断加省略号
来源：http://it.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kn.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dv.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xj.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://db.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ej.shxzukj.cn

Go:   // 按 rune 判断长度后截断
来源：http://jz.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kr.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uw.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://hv.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://it.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rk.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tq.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ti.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://in.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tq.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://tw.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cc.9csxet.cn

================================================================================
来源：http://fd.szxytkj.cn

F. 文件与目录
来源：http://gu.gzmigu.cn

================================================================================
来源：http://pe.hnjuh.cn

[F01] 读取整个文件
来源：http://nm.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mc.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://iw.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wq.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ip.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vs.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kl.asd995.cn

Ruby: File.read("a.txt")
来源：http://eh.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://yz.9csxet.cn

[F02] 逐行读取文件
来源：http://th.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kg.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yw.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uh.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lz.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rf.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fk.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yz.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fv.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://xt.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rq.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dk.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vl.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vq.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://el.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sj.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ei.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pe.jctech888.com.cn

[F04] 追加写入文件
来源：http://zk.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xd.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wr.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mh.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lq.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pw.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qd.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cz.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gk.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://dx.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xu.asd995.cn

PHP:  file_exists("a.txt");
来源：http://xn.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://xu.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://ih.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pq.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://si.521024.cn

Ruby: File.exist?("a.txt")
来源：http://dk.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://nh.jctech888.com.cn

[F06] 删除文件
来源：http://iq.521024.cn

Py:   os.remove("a.txt")
来源：http://pz.newstarts.cn

PHP:  unlink("a.txt");
来源：http://bi.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xa.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ms.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ju.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://eg.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://ik.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://ur.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://my.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ke.yuntaijiaju.cn


<!-- 参考信息 -->