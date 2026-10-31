代发 wailian999

================================================================================
来源：http://wn.nszjky.cn

E. 字符串处理
来源：http://rc.bookmarksfly.cn

================================================================================
来源：http://ny.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://lv.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ie.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fx.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oz.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ri.colortex.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rd.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wy.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vg.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qn.jianghongdianzi.cn

[E02] 重复字符串
来源：http://rg.colortex.cn

Py:   "ab" * 3
来源：http://rb.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://ey.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://tn.newstarts.cn

TS:   "ab".repeat(3)
来源：http://rd.colortex.cn

Java: "ab".repeat(3)
来源：http://vd.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://ad.huanxung.cn

Ruby: "ab" * 3
来源：http://gz.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sk.521024.cn

[E03] 截取子串
来源：http://yj.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ys.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jn.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nh.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://pe.yuntaijiaju.cn

Java: s.substring(1, 4)
来源：http://xo.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nk.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gz.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://tm.muxihuayi.cn

[E04] 查找子串位置
来源：http://ea.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://nj.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://lc.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oq.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://hz.shxzskj.cn

Java: s.indexOf("x")
来源：http://kx.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://lk.lnxyls.cn

Ruby: s.index("x")
来源：http://li.9csxet.cn

C#:   s.IndexOf("x")
来源：http://jz.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qh.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kr.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wb.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mn.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mn.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uy.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://br.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://as.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ex.bjjhwx.cn

[E06] 替换子串
来源：http://yh.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://on.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://nb.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iv.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://wl.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xn.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xc.muxihuayi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://my.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://ze.9csxet.cn

[E07] 按分隔符拆分
来源：http://de.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://np.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xz.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aq.lnxyls.cn

TS:   s.split(",")
来源：http://pj.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zp.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cr.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://ta.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jz.szsharing.cn

[E08] 数组按分隔符合并
来源：http://wu.huixiangedu.cn

Py:   ",".join(items)
来源：http://ed.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://ie.szsharing.cn

JS:   items.join(",")
来源：http://bg.wgjwhj.cn

TS:   items.join(",")
来源：http://hk.521024.cn

Java: String.join(",", items)
来源：http://fw.521024.cn

Go:   strings.Join(items, ",")
来源：http://mg.gzmigu.cn

Ruby: items.join(",")
来源：http://mj.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://hk.panjiajie.cn

[E09] 去除所有空白字符
来源：http://mh.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vb.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://il.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://lx.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://ws.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://fz.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qd.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cy.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nf.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://nz.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wu.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gd.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://sx.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://pp.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ad.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://az.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tr.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mz.jianghongdianzi.cn

[E11] 反转字符串
来源：http://vw.lnxyls.cn

Py:   s[::-1]
来源：http://ev.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://eq.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://pm.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://hy.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ww.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bn.colortex.cn

Ruby: s.reverse
来源：http://aa.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mg.szsharing.cn

[E12] 统计某字符出现次数
来源：http://pq.521024.cn

Py:   s.count("a")
来源：http://sv.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://jq.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://hk.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://db.colortex.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ma.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://bt.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://cp.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://fi.newstarts.cn

[E13] 逐字符遍历
来源：http://cn.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://pn.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ge.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mt.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qg.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jp.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ms.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pj.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yk.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://nl.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hj.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eh.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fx.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wv.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ef.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zz.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ib.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xi.nszjky.cn

[E15] HTML 转义 / 反转义
来源：http://te.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wf.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qw.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vi.panjiajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bg.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tq.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yq.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mr.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ux.huixinmuqiang.cn

[E16] 数字千分位
来源：http://of.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://un.521024.cn

PHP:  number_format(1234567);
来源：http://ua.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://by.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sc.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fr.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xz.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://si.asd995.cn

C#:   1234567.ToString("N0")
来源：http://ng.shxzskj.cn

[E17] 首字母大写
来源：http://xj.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pg.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ec.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kk.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xu.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qr.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cs.shtwfgs.cn

Ruby: s.capitalize
来源：http://zp.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tj.nicolike.cn

[E18] 模板占位符替换
来源：http://ey.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fq.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mf.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wi.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ef.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oq.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fj.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gp.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rs.9csxet.cn

[E19] 多行文本按行拆分
来源：http://cy.huanxung.cn

Py:   s.splitlines()
来源：http://oi.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xv.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://zd.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://ko.wgjwhj.cn

Java: s.lines().toList()
来源：http://ny.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://wh.huanxung.cn

Ruby: s.lines
来源：http://fu.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://mm.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://uk.panjiajie.cn

Py:   if not s:
来源：http://on.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://df.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lm.nicolike.cn

TS:   if (s === "") {}
来源：http://yo.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://mg.nicolike.cn

Go:   if s == "" {}
来源：http://qk.yuexingan06.cn

Ruby: if s.empty?
来源：http://cx.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ic.shxzukj.cn

[E21] 超长截断加省略号
来源：http://ue.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jd.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cf.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jv.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hx.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kd.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://ht.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sy.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xk.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://eo.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pw.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sc.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wc.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rk.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ye.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jy.521024.cn

Ruby: s.bytesize;  s.length
来源：http://uj.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://um.panjiajie.cn

================================================================================
来源：http://sp.hnjuh.cn

F. 文件与目录
来源：http://nw.9csxet.cn

================================================================================
来源：http://dm.haigaiapp.cn

[F01] 读取整个文件
来源：http://rq.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uc.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://uz.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kr.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://il.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jk.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hf.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://ev.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://dh.hnjuh.cn

[F02] 逐行读取文件
来源：http://zk.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kj.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sh.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://za.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vt.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rm.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bj.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sq.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vo.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://py.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ri.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ey.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gj.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bz.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://br.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qe.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://td.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pm.9csxet.cn

[F04] 追加写入文件
来源：http://qu.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hs.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://do.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ov.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://js.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://go.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xh.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kk.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nb.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://vl.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ej.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://dr.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://jw.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://rs.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ee.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ki.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://ui.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://by.huixinmuqiang.cn

[F06] 删除文件
来源：http://cn.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://vr.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://bh.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mb.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://er.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://td.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://oo.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://yg.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://zt.colortex.cn

[F07] 创建目录（含多级）
来源：http://om.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mr.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bo.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vl.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cj.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ly.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ag.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mi.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xr.yuntaijiaju.cn

[F08] 遍历目录
来源：http://me.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fo.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ax.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://de.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://ix.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wd.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mc.colortex.cn

Ruby: Dir.children("dir")
来源：http://jq.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://gb.jctech888.com.cn

[F09] 获取文件大小
来源：http://qc.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://xg.newstarts.cn

PHP:  filesize("a.txt");
来源：http://mx.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://cp.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://vf.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wg.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hj.asd995.cn

Ruby: File.size("a.txt")
来源：http://ma.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://mb.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://md.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ia.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://so.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eg.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://nx.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nx.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bf.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zc.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nf.colortex.cn

[F11] 复制与移动文件
来源：http://vl.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qz.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ma.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ub.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lt.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ug.hnjuh.cn


<!-- 参考信息 -->