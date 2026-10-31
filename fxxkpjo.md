代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://io.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gc.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ab.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zg.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fu.shxzskj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gx.huixinmuqiang.cn

[D25] Set 集合去重与交并差
来源：http://bk.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://km.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pz.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pn.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hq.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bb.jctech888.com.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gh.wgjwhj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yc.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ge.szsharing.cn

[D26] 数组转字符串
来源：http://tl.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://xz.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://gy.9csxet.cn

JS:   arr.join(", ")
来源：http://pm.gzmigu.cn

TS:   arr.join(", ")
来源：http://yq.wgjwhj.cn

Java: String.join(", ", list)
来源：http://vc.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://is.gzmigu.cn

Ruby: arr.join(", ")
来源：http://ra.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://iq.haigaiapp.cn

================================================================================
来源：http://lo.nicolike.cn

E. 字符串处理
来源：http://vt.shxzskj.cn

================================================================================
来源：http://hr.hahajie.cn

[E01] 拼接字符串
来源：http://ew.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oa.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gr.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wg.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eu.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xg.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ex.shtwfgs.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hg.nszjky.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vk.hnjuh.cn

[E02] 重复字符串
来源：http://ta.huixiangedu.cn

Py:   "ab" * 3
来源：http://dk.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://bd.nszjky.cn

JS:   "ab".repeat(3)
来源：http://tk.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://cg.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://mx.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://xe.nicolike.cn

Ruby: "ab" * 3
来源：http://hy.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nf.asd995.cn

[E03] 截取子串
来源：http://hj.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bd.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bf.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rs.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://cn.colortex.cn

Java: s.substring(1, 4)
来源：http://ew.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mu.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fp.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://ez.gzmigu.cn

[E04] 查找子串位置
来源：http://dm.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://yt.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://hx.jianghongdianzi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jm.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://ek.9csxet.cn

Java: s.indexOf("x")
来源：http://iw.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://zl.shtwfgs.cn

Ruby: s.index("x")
来源：http://dz.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://wq.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rw.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kn.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qg.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ba.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hg.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ye.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gd.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yk.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uz.huixiangedu.cn

[E06] 替换子串
来源：http://yu.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wm.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://qa.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uo.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://as.colortex.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lv.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hs.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wm.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://df.hahajie.cn

[E07] 按分隔符拆分
来源：http://tc.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cd.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rk.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tx.haigaiapp.cn

TS:   s.split(",")
来源：http://ol.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wm.hahajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kw.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://cb.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bl.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://oz.yuexingan06.cn

Py:   ",".join(items)
来源：http://cv.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://hy.hahajie.cn

JS:   items.join(",")
来源：http://xj.huixiangedu.cn

TS:   items.join(",")
来源：http://tp.szsharing.cn

Java: String.join(",", items)
来源：http://ah.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://fu.muxihuayi.cn

Ruby: items.join(",")
来源：http://if.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://he.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://wt.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dv.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ua.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://oy.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://ao.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ec.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://aj.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tl.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xj.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://xb.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ya.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oj.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://by.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://rm.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://no.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gz.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rj.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://da.szxytkj.cn

[E11] 反转字符串
来源：http://ng.lnxyls.cn

Py:   s[::-1]
来源：http://pa.hahajie.cn

PHP:  strrev($s);
来源：http://ad.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://qg.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://ym.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://un.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cf.521024.cn

Ruby: s.reverse
来源：http://ko.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://io.asd995.cn

[E12] 统计某字符出现次数
来源：http://ec.shxzskj.cn

Py:   s.count("a")
来源：http://pp.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://hg.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://bt.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://os.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cd.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://jz.hnjuh.cn

Ruby: s.count("a")
来源：http://vx.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://dz.bjjhwx.cn

[E13] 逐字符遍历
来源：http://vx.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://mh.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qw.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://su.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yu.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wa.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uv.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iv.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pf.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://iw.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ti.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ut.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oi.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://su.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lb.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lb.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wy.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bv.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://nz.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wd.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wk.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qy.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tk.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dz.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qe.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ks.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qj.wgjwhj.cn

[E16] 数字千分位
来源：http://ox.hahajie.cn

Py:   f"{1234567:,}"
来源：http://hj.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://gu.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://md.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cv.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ky.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lr.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gd.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://ev.huanxung.cn

[E17] 首字母大写
来源：http://iw.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ae.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hm.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://de.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tr.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xx.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tg.huixiangedu.cn

Ruby: s.capitalize
来源：http://xf.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ox.9csxet.cn

[E18] 模板占位符替换
来源：http://ld.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oq.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://et.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yw.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jd.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hl.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hm.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xc.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lu.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://vt.haigaiapp.cn

Py:   s.splitlines()
来源：http://st.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jc.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://ns.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://rm.wgjwhj.cn

Java: s.lines().toList()
来源：http://mj.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://mt.lnxyls.cn

Ruby: s.lines
来源：http://fb.huixiangedu.cn

C#:   s.Split('\n')
来源：http://gv.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://xq.colortex.cn

Py:   if not s:
来源：http://gm.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hs.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eo.nszjky.cn

TS:   if (s === "") {}
来源：http://bo.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://bf.9csxet.cn

Go:   if s == "" {}
来源：http://fv.gzmigu.cn

Ruby: if s.empty?
来源：http://ci.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vh.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://hg.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zp.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mq.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eu.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bg.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ia.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://vn.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cd.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hf.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://qp.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lk.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ya.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nt.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lu.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sz.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ki.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://bn.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ix.panjiajie.cn

================================================================================
来源：http://vh.yuntaijiaju.cn

F. 文件与目录
来源：http://es.521024.cn

================================================================================
来源：http://xx.shxzukj.cn

[F01] 读取整个文件
来源：http://fa.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://me.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://ni.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zn.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nl.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bt.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ry.szsharing.cn

Ruby: File.read("a.txt")
来源：http://lo.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://nr.nicolike.cn

[F02] 逐行读取文件
来源：http://js.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fo.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xi.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pq.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cr.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ld.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xf.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lj.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://fv.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ue.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mx.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zh.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xl.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ki.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://br.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://zj.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xv.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://ao.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tk.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xe.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xw.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://em.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dc.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kb.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qz.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bh.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://hy.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bb.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://tk.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://wr.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://xh.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rf.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tb.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://er.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://wp.huixinmuqiang.cn

[F06] 删除文件
来源：http://fv.nicolike.cn

Py:   os.remove("a.txt")
来源：http://ee.9csxet.cn

PHP:  unlink("a.txt");
来源：http://pt.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yp.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ip.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nb.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://xu.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://ra.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ub.huanxung.cn

[F07] 创建目录（含多级）
来源：http://mt.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yq.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ke.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ih.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oz.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zq.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ni.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rw.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zd.shxzukj.cn

[F08] 遍历目录
来源：http://iy.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nq.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uc.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://fr.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://cx.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jf.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gq.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ct.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://jo.huixiangedu.cn


<!-- 参考信息 -->