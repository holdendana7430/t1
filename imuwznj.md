代发 wailian999

================================================================================
来源：http://us.shtwfgs.cn

E. 字符串处理
来源：http://kz.shtwfgs.cn

================================================================================
来源：http://oh.shtwfgs.cn

[E01] 拼接字符串
来源：http://wo.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gg.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zy.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ev.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zo.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dl.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jq.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qw.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ec.colortex.cn

[E02] 重复字符串
来源：http://km.panjiajie.cn

Py:   "ab" * 3
来源：http://ey.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://wj.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://iw.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://rf.nicolike.cn

Java: "ab".repeat(3)
来源：http://ek.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://lo.wgjwhj.cn

Ruby: "ab" * 3
来源：http://ks.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ml.hahajie.cn

[E03] 截取子串
来源：http://fh.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hr.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://et.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://st.9csxet.cn

TS:   s.slice(1, 4)
来源：http://sa.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://xn.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zt.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ip.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://ya.asd995.cn

[E04] 查找子串位置
来源：http://hc.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://dt.muxihuayi.cn

PHP:  strpos($s, "x");
来源：http://un.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jm.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://lc.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://os.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://xn.nicolike.cn

Ruby: s.index("x")
来源：http://eq.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://ad.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nh.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mx.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ej.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fc.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ar.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yj.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dv.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hw.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qg.szsharing.cn

[E06] 替换子串
来源：http://tt.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ji.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://qo.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iv.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://sd.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cr.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ac.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sh.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://ya.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://vx.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ee.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kp.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qn.9csxet.cn

TS:   s.split(",")
来源：http://ze.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tc.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://em.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://dw.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://we.yuexingan06.cn

[E08] 数组按分隔符合并
来源：http://dj.9csxet.cn

Py:   ",".join(items)
来源：http://ma.lnxyls.cn

PHP:  implode(",", $items);
来源：http://pb.colortex.cn

JS:   items.join(",")
来源：http://it.nicolike.cn

TS:   items.join(",")
来源：http://ug.muxihuayi.cn

Java: String.join(",", items)
来源：http://vx.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://gb.nicolike.cn

Ruby: items.join(",")
来源：http://xo.szxytkj.cn

C#:   string.Join(",", items)
来源：http://hh.newstarts.cn

[E09] 去除所有空白字符
来源：http://lk.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ko.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qc.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://hu.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://ri.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://ol.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://us.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zx.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vb.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://qv.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ak.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sc.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://mn.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://ga.9csxet.cn

Java: String.format("%03d", 7)
来源：http://ud.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://eq.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ro.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://md.gzmigu.cn

[E11] 反转字符串
来源：http://dn.wgjwhj.cn

Py:   s[::-1]
来源：http://at.shxzskj.cn

PHP:  strrev($s);
来源：http://wg.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://yw.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://qm.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zl.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dl.asd995.cn

Ruby: s.reverse
来源：http://sp.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tx.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://gx.szsharing.cn

Py:   s.count("a")
来源：http://uo.colortex.cn

PHP:  substr_count($s, "a");
来源：http://go.colortex.cn

JS:   s.split("a").length - 1
来源：http://rq.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://zu.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tc.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://bq.huixiangedu.cn

Ruby: s.count("a")
来源：http://in.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://on.shxzukj.cn

[E13] 逐字符遍历
来源：http://bl.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://qd.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ar.jctech888.com.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rm.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qa.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gw.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ul.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ec.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xi.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ca.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://af.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yt.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sc.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://og.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cl.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xn.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sr.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zy.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://zm.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uo.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vd.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ji.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ck.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yk.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wc.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bd.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ko.nicolike.cn

[E16] 数字千分位
来源：http://uz.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://kc.shxzskj.cn

PHP:  number_format(1234567);
来源：http://kx.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ww.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fh.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gk.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://su.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pc.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://au.yuexingan06.cn

[E17] 首字母大写
来源：http://bx.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oo.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hm.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wo.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://no.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tg.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.huixiangedu.cn

Ruby: s.capitalize
来源：http://wm.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ch.nszjky.cn

[E18] 模板占位符替换
来源：http://sq.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kq.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://js.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vq.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rb.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vz.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dt.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oq.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gu.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://pd.yuexingan06.cn

Py:   s.splitlines()
来源：http://ss.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kj.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://zd.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://xq.shxzskj.cn

Java: s.lines().toList()
来源：http://dr.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://eh.yuntaijiaju.cn

Ruby: s.lines
来源：http://mt.wgjwhj.cn

C#:   s.Split('\n')
来源：http://xd.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://mv.lnxyls.cn

Py:   if not s:
来源：http://hq.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tc.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vj.haigaiapp.cn

TS:   if (s === "") {}
来源：http://fz.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://fh.chemitech.net.cn

Go:   if s == "" {}
来源：http://kk.lnxyls.cn

Ruby: if s.empty?
来源：http://wm.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dd.huanxung.cn

[E21] 超长截断加省略号
来源：http://ae.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wa.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gz.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ub.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jr.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lo.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://nm.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://op.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hw.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://gh.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uc.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iz.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xg.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cb.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ed.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ai.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://xm.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qv.muxihuayi.cn

================================================================================
来源：http://xj.huixiangedu.cn

F. 文件与目录
来源：http://nr.colortex.cn

================================================================================
来源：http://ai.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://rw.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pi.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://uj.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vx.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ee.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://em.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://na.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://vq.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://zs.jctech888.com.cn

[F02] 逐行读取文件
来源：http://bn.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yy.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tu.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fz.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gd.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eg.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kq.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bg.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lb.colortex.cn

[F03] 写入文件（覆盖）
来源：http://hq.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wq.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vj.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ho.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mo.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fk.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ty.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://xx.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xj.jctech888.com.cn

[F04] 追加写入文件
来源：http://pv.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qu.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zk.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cc.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xq.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pv.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yf.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://se.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gn.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://ma.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hp.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://fy.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://qh.yuntaijiaju.cn

TS:   fs.existsSync("a.txt")
来源：http://hu.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qa.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://db.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://nz.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://hk.shxzskj.cn

[F06] 删除文件
来源：http://lp.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://re.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://jq.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vg.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cj.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lg.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://hp.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://of.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://sb.colortex.cn

[F07] 创建目录（含多级）
来源：http://mu.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tw.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wr.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ey.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hd.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://so.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cp.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rq.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cc.colortex.cn

[F08] 遍历目录
来源：http://uk.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xf.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qg.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://ge.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://wa.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yg.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ed.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://lu.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://fq.nicolike.cn

[F09] 获取文件大小
来源：http://ht.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://nt.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://el.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://yv.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://sk.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ku.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://od.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://fs.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://gf.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://az.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xt.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sc.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qm.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://vr.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kl.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bj.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dx.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bq.521024.cn

[F11] 复制与移动文件
来源：http://xd.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zm.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kz.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wp.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lz.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://em.huixinmuqiang.cn


<!-- 参考信息 -->