代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wz.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ix.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dx.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ob.szsharing.cn

[E02] 重复字符串
来源：http://aq.chemitech.net.cn

Py:   "ab" * 3
来源：http://vn.colortex.cn

PHP:  str_repeat("ab", 3);
来源：http://je.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://gw.nicolike.cn

TS:   "ab".repeat(3)
来源：http://hy.shxzskj.cn

Java: "ab".repeat(3)
来源：http://tf.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://ka.huanxung.cn

Ruby: "ab" * 3
来源：http://zk.huixiangedu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vd.shxzskj.cn

[E03] 截取子串
来源：http://mv.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://js.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pt.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yo.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://nk.panjiajie.cn

Java: s.substring(1, 4)
来源：http://qb.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xq.huixinmuqiang.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iz.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://ac.wgjwhj.cn

[E04] 查找子串位置
来源：http://jt.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://rx.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://gh.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dw.521024.cn

TS:   s.indexOf("x")
来源：http://vu.521024.cn

Java: s.indexOf("x")
来源：http://gn.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://oh.yuexingan06.cn

Ruby: s.index("x")
来源：http://hf.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://cx.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ve.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gh.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ti.chemitech.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uh.521024.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://er.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fm.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nj.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qg.asd995.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fs.gzmigu.cn

[E06] 替换子串
来源：http://xj.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wo.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://ft.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jt.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://yu.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sp.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://un.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gf.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://uv.huanxung.cn

[E07] 按分隔符拆分
来源：http://aa.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fe.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://de.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jo.jctech888.com.cn

TS:   s.split(",")
来源：http://is.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dq.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kd.jianghongdianzi.cn

Ruby: s.split(",");  s.split
来源：http://bh.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hn.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://da.shxzukj.cn

Py:   ",".join(items)
来源：http://zv.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://il.haigaiapp.cn

JS:   items.join(",")
来源：http://ui.lnxyls.cn

TS:   items.join(",")
来源：http://ut.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://qb.hnjuh.cn

Go:   strings.Join(items, ",")
来源：http://nz.huanxung.cn

Ruby: items.join(",")
来源：http://gk.hahajie.cn

C#:   string.Join(",", items)
来源：http://kp.newstarts.cn

[E09] 去除所有空白字符
来源：http://qc.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ba.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ma.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://sy.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://dl.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://ys.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wl.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lr.huanxung.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zi.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://zv.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kn.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ce.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://ey.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://ok.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://iq.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://js.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hj.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zo.lnxyls.cn

[E11] 反转字符串
来源：http://zb.bjjhwx.cn

Py:   s[::-1]
来源：http://oh.szsharing.cn

PHP:  strrev($s);
来源：http://um.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://ji.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://ul.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ee.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ug.szsharing.cn

Ruby: s.reverse
来源：http://tm.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mw.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://gx.newstarts.cn

Py:   s.count("a")
来源：http://ks.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://tj.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://ep.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://nh.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wd.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://ef.colortex.cn

Ruby: s.count("a")
来源：http://bn.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://oj.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://ai.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://cb.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jf.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://na.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fg.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ag.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ga.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://il.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nv.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://kr.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sy.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xr.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lj.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pz.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qd.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ov.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qk.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mt.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://ba.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zm.muxihuayi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xr.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qu.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fc.chemitech.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kr.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bc.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tu.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lh.yuexingan06.cn

[E16] 数字千分位
来源：http://lj.huanxung.cn

Py:   f"{1234567:,}"
来源：http://fj.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://bq.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mf.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jv.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mi.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vl.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://in.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://if.panjiajie.cn

[E17] 首字母大写
来源：http://aw.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yd.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xe.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sg.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://at.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yq.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xo.bjjhwx.cn

Ruby: s.capitalize
来源：http://lo.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xo.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://hj.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cg.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yd.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wf.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rc.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oz.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xp.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://px.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dk.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://bo.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://bm.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://os.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://ub.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://rd.shxzukj.cn

Java: s.lines().toList()
来源：http://ym.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://dr.lnxyls.cn

Ruby: s.lines
来源：http://qh.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://hy.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://zl.nicolike.cn

Py:   if not s:
来源：http://tx.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gg.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fw.haigaiapp.cn

TS:   if (s === "") {}
来源：http://uw.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://bp.bjjhwx.cn

Go:   if s == "" {}
来源：http://ky.hahajie.cn

Ruby: if s.empty?
来源：http://lf.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vn.9csxet.cn

[E21] 超长截断加省略号
来源：http://zx.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rw.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wi.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qg.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ij.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mh.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://yq.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sg.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bg.asd995.cn

[E22] 字节长度与字符长度
来源：http://te.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ih.nicolike.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mu.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vp.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gg.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ls.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mg.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://nt.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ix.asd995.cn

================================================================================
来源：http://ne.hahajie.cn

F. 文件与目录
来源：http://nz.521024.cn

================================================================================
来源：http://yq.bjjhwx.cn

[F01] 读取整个文件
来源：http://zk.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kv.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://xt.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://if.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qw.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rc.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oc.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://kl.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://vg.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://tf.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vm.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qi.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vb.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ps.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nq.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://il.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cm.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zx.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://ye.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ql.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vy.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nu.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://af.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zt.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wl.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://we.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sn.szsharing.cn

[F04] 追加写入文件
来源：http://bn.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ah.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cz.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iq.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qm.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://um.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mj.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://km.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rl.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://uj.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lj.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://my.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://bd.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://is.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gq.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jb.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://eu.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ae.huixiangedu.cn

[F06] 删除文件
来源：http://ta.hahajie.cn

Py:   os.remove("a.txt")
来源：http://in.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://yc.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nq.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dy.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gv.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://so.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://vg.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://dl.521024.cn

[F07] 创建目录（含多级）
来源：http://kg.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jx.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tx.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ld.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://if.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mq.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ox.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tm.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vn.bookmarksfly.cn

[F08] 遍历目录
来源：http://kf.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gn.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ey.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://uh.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://pw.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wn.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kq.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://iv.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://lp.asd995.cn

[F09] 获取文件大小
来源：http://uc.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://st.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://zv.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://zs.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://vc.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rz.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vd.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://oc.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://pf.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://rn.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xb.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ij.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ai.nicolike.cn

TS:   path.extname("a.txt")
来源：http://uf.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fl.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mi.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sg.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yl.muxihuayi.cn

[F11] 复制与移动文件
来源：http://kf.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dj.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zw.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wg.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mj.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://de.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lm.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://de.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ub.newstarts.cn

[F12] CSV 读写
来源：http://ui.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uf.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hx.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oa.yuexingan06.cn

TS:   // 同上
来源：http://hc.huixinmuqiang.cn


<!-- 参考信息 -->