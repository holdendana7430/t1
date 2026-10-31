代发 wailian999

TS:   "ab".repeat(3)
来源：http://kh.asd995.cn

Java: "ab".repeat(3)
来源：http://ul.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://rd.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://ys.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://we.gzmigu.cn

[E03] 截取子串
来源：http://kg.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zp.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ga.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yk.colortex.cn

TS:   s.slice(1, 4)
来源：http://nz.huanxung.cn

Java: s.substring(1, 4)
来源：http://hq.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sj.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pk.521024.cn

C#:   s.Substring(1, 3)
来源：http://ci.hnjuh.cn

[E04] 查找子串位置
来源：http://ds.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://rd.9csxet.cn

PHP:  strpos($s, "x");
来源：http://jv.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nd.521024.cn

TS:   s.indexOf("x")
来源：http://lx.521024.cn

Java: s.indexOf("x")
来源：http://vp.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://zp.hahajie.cn

Ruby: s.index("x")
来源：http://fw.newstarts.cn

C#:   s.IndexOf("x")
来源：http://zj.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://or.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ov.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dk.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ak.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jo.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hw.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bx.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qa.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ra.asd995.cn

[E06] 替换子串
来源：http://ge.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mk.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://pb.nicolike.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nf.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://ii.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rm.newstarts.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wt.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cl.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://uw.hnjuh.cn

[E07] 按分隔符拆分
来源：http://zq.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ot.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://co.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cx.wgjwhj.cn

TS:   s.split(",")
来源：http://bj.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xi.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tn.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://ja.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sf.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://ff.521024.cn

Py:   ",".join(items)
来源：http://zn.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://ix.colortex.cn

JS:   items.join(",")
来源：http://wl.huanxung.cn

TS:   items.join(",")
来源：http://ic.haigaiapp.cn

Java: String.join(",", items)
来源：http://kg.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://bu.gzmigu.cn

Ruby: items.join(",")
来源：http://mw.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://ik.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://ve.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wv.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ki.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://zk.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://qu.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://ie.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ma.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lf.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lv.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://cz.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ul.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sx.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://ae.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://fg.nicolike.cn

Java: String.format("%03d", 7)
来源：http://dc.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fa.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pe.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ls.hahajie.cn

[E11] 反转字符串
来源：http://md.huixiangedu.cn

Py:   s[::-1]
来源：http://ee.shxzskj.cn

PHP:  strrev($s);
来源：http://um.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://qk.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://al.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rm.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ez.muxihuayi.cn

Ruby: s.reverse
来源：http://wh.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qf.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://vd.lnxyls.cn

Py:   s.count("a")
来源：http://xy.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://im.huanxung.cn

JS:   s.split("a").length - 1
来源：http://pz.nicolike.cn

TS:   s.split("a").length - 1
来源：http://jx.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wh.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://lh.newstarts.cn

Ruby: s.count("a")
来源：http://wl.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://cb.hnjuh.cn

[E13] 逐字符遍历
来源：http://rb.521024.cn

Py:   for ch in s: print(ch)
来源：http://jf.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xb.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rj.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wu.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xn.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mf.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://px.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xm.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://pb.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wa.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ay.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dn.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nv.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ni.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ig.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rd.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mk.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://jf.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wa.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://do.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sx.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ui.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ke.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yp.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bs.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rr.bookmarksfly.cn

[E16] 数字千分位
来源：http://fg.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://nd.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://qf.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ty.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hg.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vl.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hp.panjiajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xr.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://sn.jctech888.com.cn

[E17] 首字母大写
来源：http://xw.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sc.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ty.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cz.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jz.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jh.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wt.huixiangedu.cn

Ruby: s.capitalize
来源：http://gh.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ah.jctech888.com.cn

[E18] 模板占位符替换
来源：http://ia.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qr.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qf.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rq.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qq.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ri.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mm.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wh.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oc.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://mq.shxzukj.cn

Py:   s.splitlines()
来源：http://uk.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hq.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://jb.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://us.shtwfgs.cn

Java: s.lines().toList()
来源：http://my.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://rh.bjjhwx.cn

Ruby: s.lines
来源：http://zo.chemitech.net.cn

C#:   s.Split('\n')
来源：http://rx.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://ve.muxihuayi.cn

Py:   if not s:
来源：http://hl.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jk.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ta.jctech888.com.cn

TS:   if (s === "") {}
来源：http://kp.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://jv.lnxyls.cn

Go:   if s == "" {}
来源：http://bc.hahajie.cn

Ruby: if s.empty?
来源：http://bi.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bv.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://pn.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tv.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pj.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ji.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qa.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uy.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://tz.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://by.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ls.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://bw.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ed.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://un.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vu.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nw.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bc.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jq.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://xb.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zk.huixinmuqiang.cn

================================================================================
来源：http://pt.shtwfgs.cn

F. 文件与目录
来源：http://km.bjjhwx.cn

================================================================================
来源：http://co.panjiajie.cn

[F01] 读取整个文件
来源：http://nn.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sj.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://jn.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ff.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kp.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uy.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://it.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://di.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://gd.haigaiapp.cn

[F02] 逐行读取文件
来源：http://uh.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vx.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gh.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nl.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vr.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pd.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lw.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rf.yuntaijiaju.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ey.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://ee.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zm.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tv.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gc.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ps.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sw.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iw.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://mw.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fw.hahajie.cn

[F04] 追加写入文件
来源：http://qy.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hb.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bw.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aq.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zi.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ns.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ny.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://om.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zu.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://cq.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gx.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://qo.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://fu.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://oq.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zn.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lq.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://wd.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://rg.hnjuh.cn

[F06] 删除文件
来源：http://kt.asd995.cn

Py:   os.remove("a.txt")
来源：http://fv.huanxung.cn

PHP:  unlink("a.txt");
来源：http://im.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uj.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://el.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ti.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://oj.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://rr.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://ci.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://qd.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wm.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ik.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jx.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wl.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pv.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mw.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ne.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nu.nszjky.cn

[F08] 遍历目录
来源：http://lk.lnxyls.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hb.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://li.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://ao.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://no.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gg.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://db.newstarts.cn

Ruby: Dir.children("dir")
来源：http://qm.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://ql.szxytkj.cn

[F09] 获取文件大小
来源：http://qw.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://xa.hahajie.cn

PHP:  filesize("a.txt");
来源：http://is.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://mz.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://uu.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wi.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vg.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://li.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://fp.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://gx.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vs.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lh.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qq.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://gy.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ri.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ih.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ov.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sl.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://eg.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zx.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gv.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vr.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dh.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ie.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rc.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nn.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qa.colortex.cn

[F12] CSV 读写
来源：http://hq.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fj.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bt.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hq.hahajie.cn

TS:   // 同上
来源：http://zl.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wk.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xr.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mg.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rh.bookmarksfly.cn

================================================================================
来源：http://jq.huixiangedu.cn

G. 面向对象
来源：http://pt.colortex.cn

================================================================================
来源：http://ox.521024.cn

[G01] 定义类
来源：http://pn.shxzukj.cn


<!-- 参考信息 -->