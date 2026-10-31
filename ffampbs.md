代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sg.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qx.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qo.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ee.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lp.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yk.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yq.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://or.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://gz.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://ez.shxzukj.cn

JS:   arr.join(", ")
来源：http://aj.hnjuh.cn

TS:   arr.join(", ")
来源：http://kb.nicolike.cn

Java: String.join(", ", list)
来源：http://ra.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://da.9csxet.cn

Ruby: arr.join(", ")
来源：http://ah.huanxung.cn

C#:   string.Join(", ", list)
来源：http://yx.szxytkj.cn

================================================================================
来源：http://cx.szxytkj.cn

E. 字符串处理
来源：http://ow.jctech888.com.cn

================================================================================
来源：http://bx.9csxet.cn

[E01] 拼接字符串
来源：http://nh.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://um.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://np.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iy.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://du.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rz.shxzukj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xg.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ez.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qe.wgjwhj.cn

[E02] 重复字符串
来源：http://nh.yuexingan06.cn

Py:   "ab" * 3
来源：http://he.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://xm.9csxet.cn

JS:   "ab".repeat(3)
来源：http://zw.521024.cn

TS:   "ab".repeat(3)
来源：http://ct.asd995.cn

Java: "ab".repeat(3)
来源：http://fi.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://yx.colortex.cn

Ruby: "ab" * 3
来源：http://yn.bjjhwx.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tz.haigaiapp.cn

[E03] 截取子串
来源：http://je.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://di.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tr.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dx.huanxung.cn

TS:   s.slice(1, 4)
来源：http://ai.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://rz.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iv.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xc.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://lt.shxzskj.cn

[E04] 查找子串位置
来源：http://jn.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://la.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://jd.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mh.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://ek.lnxyls.cn

Java: s.indexOf("x")
来源：http://yv.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://ra.shtwfgs.cn

Ruby: s.index("x")
来源：http://he.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://jt.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hp.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uo.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zn.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://su.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aq.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gp.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uo.gzmigu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pu.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xn.jianghongdianzi.cn

[E06] 替换子串
来源：http://eg.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ou.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://ac.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zm.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://at.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yc.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hd.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://re.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://vq.hahajie.cn

[E07] 按分隔符拆分
来源：http://db.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://to.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fc.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qm.asd995.cn

TS:   s.split(",")
来源：http://hs.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gr.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zu.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://jp.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ma.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://ln.bookmarksfly.cn

Py:   ",".join(items)
来源：http://vg.9csxet.cn

PHP:  implode(",", $items);
来源：http://sx.szsharing.cn

JS:   items.join(",")
来源：http://ud.wgjwhj.cn

TS:   items.join(",")
来源：http://hy.bjjhwx.cn

Java: String.join(",", items)
来源：http://qo.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://bl.shxzukj.cn

Ruby: items.join(",")
来源：http://ay.521024.cn

C#:   string.Join(",", items)
来源：http://pz.huanxung.cn

[E09] 去除所有空白字符
来源：http://ng.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cq.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bi.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://ao.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://ln.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://pd.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zo.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dj.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cb.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://ng.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://on.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vh.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://le.muxihuayi.cn

TS:   "7".padStart(3, "0")
来源：http://zo.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://mv.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://su.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eq.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vv.jctech888.com.cn

[E11] 反转字符串
来源：http://ax.haigaiapp.cn

Py:   s[::-1]
来源：http://bq.asd995.cn

PHP:  strrev($s);
来源：http://sh.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://nh.521024.cn

TS:   [...s].reverse().join("")
来源：http://bv.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xn.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ji.huanxung.cn

Ruby: s.reverse
来源：http://zz.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mw.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://lg.wgjwhj.cn

Py:   s.count("a")
来源：http://qd.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://fi.9csxet.cn

JS:   s.split("a").length - 1
来源：http://qt.asd995.cn

TS:   s.split("a").length - 1
来源：http://bt.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tx.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://uy.muxihuayi.cn

Ruby: s.count("a")
来源：http://rg.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://dd.shxzukj.cn

[E13] 逐字符遍历
来源：http://gv.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://jz.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zu.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vv.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://um.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aq.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vr.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hl.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uy.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://yb.newstarts.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nz.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pk.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ay.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dm.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://li.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gp.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ug.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cy.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://sc.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://in.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ey.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vp.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://as.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jy.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dv.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tx.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ha.521024.cn

[E16] 数字千分位
来源：http://pw.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://we.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://fn.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://os.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hl.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ia.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ni.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wk.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ad.shxzskj.cn

[E17] 首字母大写
来源：http://ly.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gu.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jp.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://po.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eq.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sf.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dt.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://fp.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vv.hahajie.cn

[E18] 模板占位符替换
来源：http://zt.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zs.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gw.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yd.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ix.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zk.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hp.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hn.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tf.nszjky.cn

[E19] 多行文本按行拆分
来源：http://lf.huanxung.cn

Py:   s.splitlines()
来源：http://yg.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rf.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://bh.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://po.bjjhwx.cn

Java: s.lines().toList()
来源：http://jy.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://hi.panjiajie.cn

Ruby: s.lines
来源：http://ho.hahajie.cn

C#:   s.Split('\n')
来源：http://ae.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://bj.panjiajie.cn

Py:   if not s:
来源：http://sf.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bo.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fp.panjiajie.cn

TS:   if (s === "") {}
来源：http://dy.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://if.shxzukj.cn

Go:   if s == "" {}
来源：http://rc.hahajie.cn

Ruby: if s.empty?
来源：http://uc.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ro.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://ef.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ax.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zw.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://he.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ar.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jl.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://fb.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wl.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ib.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://nd.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ee.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zv.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hv.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ih.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kb.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://de.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://yc.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wg.newstarts.cn

================================================================================
来源：http://ab.colortex.cn

F. 文件与目录
来源：http://ez.huanxung.cn

================================================================================
来源：http://ut.yuexingan06.cn

[F01] 读取整个文件
来源：http://yi.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ta.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://ou.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wx.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tw.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ah.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gl.9csxet.cn

Ruby: File.read("a.txt")
来源：http://yk.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://sr.panjiajie.cn

[F02] 逐行读取文件
来源：http://ua.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://az.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xi.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://np.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ax.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xq.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kc.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aj.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iq.hahajie.cn

[F03] 写入文件（覆盖）
来源：http://dr.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ab.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cq.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tf.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ij.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eo.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zd.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://ny.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wy.shxzukj.cn

[F04] 追加写入文件
来源：http://er.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kd.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cc.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tu.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vl.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zz.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wl.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mk.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cu.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://ko.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://io.521024.cn

PHP:  file_exists("a.txt");
来源：http://rl.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://qt.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://my.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kf.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wp.521024.cn

Ruby: File.exist?("a.txt")
来源：http://du.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://iy.521024.cn

[F06] 删除文件
来源：http://ru.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://qp.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://jq.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ee.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dx.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yu.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://yi.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://rr.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://vb.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://yk.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zt.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://au.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xg.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yj.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oy.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gu.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ot.huanxung.cn

[F08] 遍历目录
来源：http://ft.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hv.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bb.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://sv.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ad.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mg.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dg.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://xb.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://nc.szsharing.cn

[F09] 获取文件大小
来源：http://uo.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://xm.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://nl.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://li.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://ts.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://md.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jb.asd995.cn

Ruby: File.size("a.txt")
来源：http://ju.shxzskj.cn


<!-- 参考信息 -->