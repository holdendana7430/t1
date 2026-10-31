代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://sp.huixiangedu.cn

PHP:  implode(", ", $arr);
来源：http://zr.521024.cn

JS:   arr.join(", ")
来源：http://kq.nicolike.cn

TS:   arr.join(", ")
来源：http://cm.hahajie.cn

Java: String.join(", ", list)
来源：http://dn.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://yz.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://do.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://ny.shxzskj.cn

================================================================================
来源：http://js.haigaiapp.cn

E. 字符串处理
来源：http://at.huixiangedu.cn

================================================================================
来源：http://jq.haigaiapp.cn

[E01] 拼接字符串
来源：http://kr.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zu.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ht.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bc.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jw.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hv.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iw.wgjwhj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wn.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rl.521024.cn

[E02] 重复字符串
来源：http://xx.gzmigu.cn

Py:   "ab" * 3
来源：http://vw.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://in.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ml.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://pj.lnxyls.cn

Java: "ab".repeat(3)
来源：http://bd.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://um.gzmigu.cn

Ruby: "ab" * 3
来源：http://dw.szsharing.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gv.shxzukj.cn

[E03] 截取子串
来源：http://ys.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ge.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lp.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qi.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://bd.colortex.cn

Java: s.substring(1, 4)
来源：http://pp.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kj.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jr.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://lf.asd995.cn

[E04] 查找子串位置
来源：http://bt.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://tj.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://wg.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ty.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://ub.hahajie.cn

Java: s.indexOf("x")
来源：http://fw.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://tn.bjjhwx.cn

Ruby: s.index("x")
来源：http://hw.huanxung.cn

C#:   s.IndexOf("x")
来源：http://do.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jr.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tz.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tz.asd995.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sa.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kg.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pn.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xd.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wo.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yr.chemitech.net.cn

[E06] 替换子串
来源：http://jk.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xo.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://vf.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iz.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://vb.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ms.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://up.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dm.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://fx.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://fp.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gn.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oa.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ck.nszjky.cn

TS:   s.split(",")
来源：http://xd.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xg.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xc.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://gh.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ez.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://dc.asd995.cn

Py:   ",".join(items)
来源：http://as.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://ln.shxzskj.cn

JS:   items.join(",")
来源：http://mn.shtwfgs.cn

TS:   items.join(",")
来源：http://rx.muxihuayi.cn

Java: String.join(",", items)
来源：http://vr.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://cw.9csxet.cn

Ruby: items.join(",")
来源：http://kt.huanxung.cn

C#:   string.Join(",", items)
来源：http://bp.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://rh.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cj.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qx.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://jo.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://tq.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://ui.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qw.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kr.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fm.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://ug.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fr.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mv.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://sd.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://pf.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://iw.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yp.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wa.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vy.hahajie.cn

[E11] 反转字符串
来源：http://we.bjjhwx.cn

Py:   s[::-1]
来源：http://qn.nszjky.cn

PHP:  strrev($s);
来源：http://eh.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://vg.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://te.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ar.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yw.asd995.cn

Ruby: s.reverse
来源：http://ow.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bn.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://ss.colortex.cn

Py:   s.count("a")
来源：http://ln.521024.cn

PHP:  substr_count($s, "a");
来源：http://ku.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://ch.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://ij.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iw.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://gr.gzmigu.cn

Ruby: s.count("a")
来源：http://qz.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://wl.huixiangedu.cn

[E13] 逐字符遍历
来源：http://ys.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://gl.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nl.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kw.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hk.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yx.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jd.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jh.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zy.nicolike.cn

[E14] URL 编码与 Base64
来源：http://of.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kc.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jp.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nq.nicolike.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vl.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qh.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ic.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ng.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xy.521024.cn

[E15] HTML 转义 / 反转义
来源：http://hd.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sj.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xh.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zt.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kj.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qc.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vc.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gy.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qi.bookmarksfly.cn

[E16] 数字千分位
来源：http://qr.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://fi.newstarts.cn

PHP:  number_format(1234567);
来源：http://qp.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lw.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lm.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xu.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ud.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xk.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://sw.jianghongdianzi.cn

[E17] 首字母大写
来源：http://gz.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yw.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pe.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kl.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tr.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zv.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mq.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://mm.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ch.lnxyls.cn

[E18] 模板占位符替换
来源：http://dg.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bn.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zs.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bg.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cd.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://it.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jm.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hs.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ec.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://ia.jctech888.com.cn

Py:   s.splitlines()
来源：http://bd.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zr.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://px.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://em.panjiajie.cn

Java: s.lines().toList()
来源：http://fr.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://xo.huanxung.cn

Ruby: s.lines
来源：http://ts.9csxet.cn

C#:   s.Split('\n')
来源：http://lv.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://lg.jianghongdianzi.cn

Py:   if not s:
来源：http://lv.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sz.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mm.asd995.cn

TS:   if (s === "") {}
来源：http://gp.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://eh.bjjhwx.cn

Go:   if s == "" {}
来源：http://ml.bjjhwx.cn

Ruby: if s.empty?
来源：http://sv.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mz.newstarts.cn

[E21] 超长截断加省略号
来源：http://rs.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lm.bookmarksfly.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gf.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kr.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://px.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://np.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://pt.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gj.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://um.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://ok.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tz.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uh.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yu.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ey.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ag.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://af.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://ov.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://me.lnxyls.cn

================================================================================
来源：http://lb.colortex.cn

F. 文件与目录
来源：http://zf.hnjuh.cn

================================================================================
来源：http://wa.bookmarksfly.cn

[F01] 读取整个文件
来源：http://cu.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ca.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://al.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sq.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://km.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fn.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fd.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://bc.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://be.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://zi.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pv.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oy.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ax.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ri.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://us.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ne.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://io.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qj.colortex.cn

[F03] 写入文件（覆盖）
来源：http://et.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eu.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qi.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mn.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fu.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jt.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fr.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://hq.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kj.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://kh.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qo.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mn.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jd.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dw.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ts.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://um.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ju.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ig.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://dp.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mc.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://uf.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://la.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://yx.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lr.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cj.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://rm.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://cr.9csxet.cn

[F06] 删除文件
来源：http://ym.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://uj.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://zq.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dl.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wu.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pv.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://cx.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://lg.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://cv.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://jm.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://us.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wv.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pe.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xk.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nl.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mo.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zw.szxytkj.cn

[F08] 遍历目录
来源：http://fl.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uy.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pt.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://qa.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://li.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yb.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ec.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://lx.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://kk.9csxet.cn

[F09] 获取文件大小
来源：http://ms.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://wa.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://qq.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://vo.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://dt.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gj.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kg.nszjky.cn

Ruby: File.size("a.txt")
来源：http://xr.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://gf.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://sg.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ir.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hl.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pz.szsharing.cn

TS:   path.extname("a.txt")
来源：http://mk.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nh.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nd.wgjwhj.cn


<!-- 参考信息 -->