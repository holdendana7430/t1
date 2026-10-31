代发 wailian999

================================================================================
来源：http://qq.hahajie.cn

E. 字符串处理
来源：http://mj.szxytkj.cn

================================================================================
来源：http://vj.huixiangedu.cn

[E01] 拼接字符串
来源：http://zy.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bk.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://og.huanxung.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tp.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kl.szxytkj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sq.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ql.hahajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gz.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xu.haigaiapp.cn

[E02] 重复字符串
来源：http://zc.wgjwhj.cn

Py:   "ab" * 3
来源：http://xj.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://uz.muxihuayi.cn

JS:   "ab".repeat(3)
来源：http://xh.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://ov.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://tz.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://kd.huanxung.cn

Ruby: "ab" * 3
来源：http://ad.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vm.huixiangedu.cn

[E03] 截取子串
来源：http://pj.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qx.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kl.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ax.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://kd.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://xm.nicolike.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aw.shxzukj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mj.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://fo.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://ln.9csxet.cn

Py:   s.find("x");  s.index("x")
来源：http://sl.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://no.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pw.szsharing.cn

TS:   s.indexOf("x")
来源：http://ip.jctech888.com.cn

Java: s.indexOf("x")
来源：http://uf.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://gq.huanxung.cn

Ruby: s.index("x")
来源：http://by.szsharing.cn

C#:   s.IndexOf("x")
来源：http://dv.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cr.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gq.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eq.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dl.hnjuh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zk.colortex.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ge.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jt.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://la.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pp.huixinmuqiang.cn

[E06] 替换子串
来源：http://vs.colortex.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kq.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://uv.yuexingan06.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cb.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://yv.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://id.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ai.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wz.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://qf.hahajie.cn

[E07] 按分隔符拆分
来源：http://zw.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xg.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://og.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jm.bookmarksfly.cn

TS:   s.split(",")
来源：http://ba.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ph.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://db.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://lg.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pk.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://zz.asd995.cn

Py:   ",".join(items)
来源：http://hq.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://vs.hnjuh.cn

JS:   items.join(",")
来源：http://kv.gzmigu.cn

TS:   items.join(",")
来源：http://mr.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://vs.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://hh.shxzukj.cn

Ruby: items.join(",")
来源：http://xh.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://vz.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://sf.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qo.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ld.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://xc.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://bs.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://qi.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tu.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ca.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xn.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://af.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bn.huixiangedu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ig.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://is.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://ef.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://sz.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fz.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rf.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ng.szxytkj.cn

[E11] 反转字符串
来源：http://pe.9csxet.cn

Py:   s[::-1]
来源：http://vu.hahajie.cn

PHP:  strrev($s);
来源：http://jy.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://pe.colortex.cn

TS:   [...s].reverse().join("")
来源：http://tm.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ua.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ov.huixiangedu.cn

Ruby: s.reverse
来源：http://fo.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zs.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://tm.jctech888.com.cn

Py:   s.count("a")
来源：http://la.asd995.cn

PHP:  substr_count($s, "a");
来源：http://mm.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://df.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://qa.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://po.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://jr.shtwfgs.cn

Ruby: s.count("a")
来源：http://xl.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://fq.muxihuayi.cn

[E13] 逐字符遍历
来源：http://fc.huixiangedu.cn

Py:   for ch in s: print(ch)
来源：http://mk.hahajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dw.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qn.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sc.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ly.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gp.newstarts.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ij.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mr.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://ow.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zs.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lt.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hm.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ol.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tv.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iv.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tq.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ah.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://rc.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://or.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ku.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ph.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wm.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ee.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lj.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ov.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://px.colortex.cn

[E16] 数字千分位
来源：http://wr.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://rv.szsharing.cn

PHP:  number_format(1234567);
来源：http://fu.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ct.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rk.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fj.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dx.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://se.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://aq.shxzskj.cn

[E17] 首字母大写
来源：http://xy.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cg.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fo.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ea.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ri.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ms.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sn.gzmigu.cn

Ruby: s.capitalize
来源：http://df.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rp.nszjky.cn

[E18] 模板占位符替换
来源：http://dw.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ab.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zz.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ve.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wh.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nf.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ye.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ed.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cz.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://sv.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://bo.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kl.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://ng.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://im.jianghongdianzi.cn

Java: s.lines().toList()
来源：http://ca.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://cc.haigaiapp.cn

Ruby: s.lines
来源：http://vk.nicolike.cn

C#:   s.Split('\n')
来源：http://yu.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://wq.huixinmuqiang.cn

Py:   if not s:
来源：http://td.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bl.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vw.asd995.cn

TS:   if (s === "") {}
来源：http://wg.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://hy.chemitech.net.cn

Go:   if s == "" {}
来源：http://ri.huixiangedu.cn

Ruby: if s.empty?
来源：http://ur.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zh.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://pa.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wa.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fe.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yp.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lj.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ev.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://ka.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cy.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vy.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://yg.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tg.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rx.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ta.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zm.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hw.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ys.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://xs.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ro.jianghongdianzi.cn

================================================================================
来源：http://jj.hahajie.cn

F. 文件与目录
来源：http://ju.haigaiapp.cn

================================================================================
来源：http://ks.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://hw.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ns.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://vj.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ds.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://et.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ow.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bs.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://ar.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://bp.huanxung.cn

[F02] 逐行读取文件
来源：http://nh.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://of.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ft.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wq.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kh.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jf.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jt.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pb.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://em.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://jh.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hf.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oh.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dl.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eg.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://by.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hy.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://zv.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zd.chemitech.net.cn

[F04] 追加写入文件
来源：http://gr.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ln.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ik.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fq.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pk.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mk.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zl.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kb.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hr.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://ca.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://st.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://cy.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://dn.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://nr.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kz.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fk.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://dv.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://nx.jctech888.com.cn

[F06] 删除文件
来源：http://gu.asd995.cn

Py:   os.remove("a.txt")
来源：http://cy.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://ts.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vw.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gc.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ol.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://os.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://oh.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://bb.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://nu.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mz.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://db.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kh.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fw.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rt.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://az.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rl.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wc.muxihuayi.cn

[F08] 遍历目录
来源：http://fa.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fn.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cc.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://fw.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://sz.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ka.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ea.szsharing.cn

Ruby: Dir.children("dir")
来源：http://xg.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://sk.bookmarksfly.cn

[F09] 获取文件大小
来源：http://ry.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://gg.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://bk.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://vc.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://wc.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wo.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yh.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://nf.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://lv.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://gg.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qh.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ny.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vi.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://yv.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xz.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nk.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jo.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kk.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://rb.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iz.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ge.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ui.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iz.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shxzukj.cn


<!-- 参考信息 -->