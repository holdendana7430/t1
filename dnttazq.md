代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tj.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ed.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kg.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://me.yuexingan06.cn

[E02] 重复字符串
来源：http://cu.9csxet.cn

Py:   "ab" * 3
来源：http://fb.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://ck.szsharing.cn

JS:   "ab".repeat(3)
来源：http://zf.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://wb.haigaiapp.cn

Java: "ab".repeat(3)
来源：http://bu.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://mb.jctech888.com.cn

Ruby: "ab" * 3
来源：http://tz.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oz.jianghongdianzi.cn

[E03] 截取子串
来源：http://kq.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zm.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://er.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xc.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ol.panjiajie.cn

Java: s.substring(1, 4)
来源：http://ap.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uf.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mm.colortex.cn

C#:   s.Substring(1, 3)
来源：http://hg.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://oj.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://tr.asd995.cn

PHP:  strpos($s, "x");
来源：http://hx.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fs.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://jg.521024.cn

Java: s.indexOf("x")
来源：http://vt.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://ss.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ef.colortex.cn

C#:   s.IndexOf("x")
来源：http://lt.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nv.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://on.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vv.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iw.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ja.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rg.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qy.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cf.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bz.bjjhwx.cn

[E06] 替换子串
来源：http://vp.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dd.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://nv.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ju.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://zt.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wv.huanxung.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://in.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aq.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://ig.asd995.cn

[E07] 按分隔符拆分
来源：http://es.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yj.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bs.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cf.jctech888.com.cn

TS:   s.split(",")
来源：http://rr.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gr.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uy.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://ig.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://au.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://lo.chemitech.net.cn

Py:   ",".join(items)
来源：http://zp.huanxung.cn

PHP:  implode(",", $items);
来源：http://qo.huixiangedu.cn

JS:   items.join(",")
来源：http://in.newstarts.cn

TS:   items.join(",")
来源：http://aj.colortex.cn

Java: String.join(",", items)
来源：http://ok.asd995.cn

Go:   strings.Join(items, ",")
来源：http://sj.wgjwhj.cn

Ruby: items.join(",")
来源：http://so.szxytkj.cn

C#:   string.Join(",", items)
来源：http://wz.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://tk.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pt.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cv.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://tp.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://pi.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://hk.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yr.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wa.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lj.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://qx.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pa.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vo.521024.cn

JS:   "7".padStart(3, "0")
来源：http://ah.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://ot.hahajie.cn

Java: String.format("%03d", 7)
来源：http://um.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fg.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gs.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kr.asd995.cn

[E11] 反转字符串
来源：http://jo.huixinmuqiang.cn

Py:   s[::-1]
来源：http://rx.panjiajie.cn

PHP:  strrev($s);
来源：http://vz.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://le.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://pk.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ls.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://av.nicolike.cn

Ruby: s.reverse
来源：http://fp.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lm.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://pf.shxzukj.cn

Py:   s.count("a")
来源：http://og.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://zq.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://ga.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://gh.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tf.asd995.cn

Go:   strings.Count(s, "a")
来源：http://ey.chemitech.net.cn

Ruby: s.count("a")
来源：http://pq.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://yj.hahajie.cn

[E13] 逐字符遍历
来源：http://zm.521024.cn

Py:   for ch in s: print(ch)
来源：http://ty.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uz.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rc.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://js.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://af.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wl.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aj.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ho.colortex.cn

[E14] URL 编码与 Base64
来源：http://yg.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xs.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qx.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dj.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lp.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gs.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gx.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ya.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uz.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://zk.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://it.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hu.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sz.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ir.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vq.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kj.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fu.yuntaijiaju.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ej.szsharing.cn

[E16] 数字千分位
来源：http://va.huanxung.cn

Py:   f"{1234567:,}"
来源：http://ul.hahajie.cn

PHP:  number_format(1234567);
来源：http://gq.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://su.panjiajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wb.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ut.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lf.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lo.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://eb.muxihuayi.cn

[E17] 首字母大写
来源：http://fx.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uk.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://br.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://do.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://so.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wm.lnxyls.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://il.gzmigu.cn

Ruby: s.capitalize
来源：http://yv.521024.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nf.521024.cn

[E18] 模板占位符替换
来源：http://oe.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wk.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ol.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zi.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rz.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kd.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ib.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zq.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sr.newstarts.cn

[E19] 多行文本按行拆分
来源：http://rf.nszjky.cn

Py:   s.splitlines()
来源：http://kb.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ay.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://zu.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://rb.nicolike.cn

Java: s.lines().toList()
来源：http://pq.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://jm.hahajie.cn

Ruby: s.lines
来源：http://wz.panjiajie.cn

C#:   s.Split('\n')
来源：http://pm.9csxet.cn

[E20] 判断字符串是否为空
来源：http://pb.hahajie.cn

Py:   if not s:
来源：http://ix.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pp.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jo.haigaiapp.cn

TS:   if (s === "") {}
来源：http://wu.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://gd.nszjky.cn

Go:   if s == "" {}
来源：http://zs.wgjwhj.cn

Ruby: if s.empty?
来源：http://th.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ky.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://ja.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ag.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jh.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yz.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://km.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xm.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://cg.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rr.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tc.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://gk.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yp.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ic.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wq.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://as.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ex.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://nc.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pw.lnxyls.cn

================================================================================
来源：http://hb.huixinmuqiang.cn

F. 文件与目录
来源：http://xq.shxzskj.cn

================================================================================
来源：http://sw.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://py.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ig.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://jd.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lj.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mj.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vo.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gq.huanxung.cn

Ruby: File.read("a.txt")
来源：http://sl.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://hy.shtwfgs.cn

[F02] 逐行读取文件
来源：http://dv.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xh.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vg.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bo.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://el.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ox.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sy.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://po.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pq.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://ow.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yl.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tp.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cm.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yn.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hq.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oy.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://dv.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zx.shxzukj.cn

[F04] 追加写入文件
来源：http://wz.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cn.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zc.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qe.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://by.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://on.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://st.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://be.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qh.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://mo.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hh.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://po.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://hx.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://rf.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://th.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ah.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://uh.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://jr.huixinmuqiang.cn

[F06] 删除文件
来源：http://ab.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://kg.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://qs.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mo.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wl.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xs.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://ob.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://jh.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://ct.newstarts.cn

[F07] 创建目录（含多级）
来源：http://rq.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yp.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sk.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ve.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uo.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yf.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kq.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vm.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oc.newstarts.cn

[F08] 遍历目录
来源：http://ez.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sj.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ln.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://ga.521024.cn

TS:   fs.readdirSync("dir")
来源：http://qn.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wi.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xb.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://gw.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://kw.szxytkj.cn

[F09] 获取文件大小
来源：http://pg.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://fp.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://li.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://ls.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://uc.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://km.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ar.huanxung.cn

Ruby: File.size("a.txt")
来源：http://eo.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://ef.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://bt.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kr.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://as.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rt.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://hh.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qu.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pz.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zc.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://df.muxihuayi.cn

[F11] 复制与移动文件
来源：http://wv.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fk.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dm.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ay.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://al.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qx.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ne.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qo.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zu.asd995.cn

[F12] CSV 读写
来源：http://mg.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ak.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cr.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://te.shxzskj.cn

TS:   // 同上
来源：http://rn.haigaiapp.cn


<!-- 参考信息 -->