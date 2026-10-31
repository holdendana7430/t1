代发 wailian999

PHP:  strpos($s, "x");
来源：http://rp.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yx.521024.cn

TS:   s.indexOf("x")
来源：http://mh.szsharing.cn

Java: s.indexOf("x")
来源：http://bu.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://ld.hnjuh.cn

Ruby: s.index("x")
来源：http://ke.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ao.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://we.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ez.9csxet.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ye.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wv.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dz.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fc.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xk.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nf.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ox.shxzukj.cn

[E06] 替换子串
来源：http://bt.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cm.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://rv.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ea.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://bo.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cw.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bx.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vf.colortex.cn

C#:   s.Replace("a", "b")
来源：http://qm.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://qu.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nv.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://to.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vs.jianghongdianzi.cn

TS:   s.split(",")
来源：http://fa.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://my.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wf.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://ih.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zg.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://pp.shxzukj.cn

Py:   ",".join(items)
来源：http://gj.lnxyls.cn

PHP:  implode(",", $items);
来源：http://yg.jianghongdianzi.cn

JS:   items.join(",")
来源：http://yq.bjjhwx.cn

TS:   items.join(",")
来源：http://vg.huixiangedu.cn

Java: String.join(",", items)
来源：http://tf.yuntaijiaju.cn

Go:   strings.Join(items, ",")
来源：http://rb.shtwfgs.cn

Ruby: items.join(",")
来源：http://mo.hahajie.cn

C#:   string.Join(",", items)
来源：http://qd.gzmigu.cn

[E09] 去除所有空白字符
来源：http://tt.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jt.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yd.jctech888.com.cn

JS:   s.replace(/\s+/g, "")
来源：http://ov.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://mh.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://jh.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eh.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kf.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://on.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://bq.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fe.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oc.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://mh.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://jw.521024.cn

Java: String.format("%03d", 7)
来源：http://fx.chemitech.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hh.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://im.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ct.lnxyls.cn

[E11] 反转字符串
来源：http://ew.nszjky.cn

Py:   s[::-1]
来源：http://zd.hnjuh.cn

PHP:  strrev($s);
来源：http://dn.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://ew.panjiajie.cn

TS:   [...s].reverse().join("")
来源：http://xi.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wx.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pf.huanxung.cn

Ruby: s.reverse
来源：http://vf.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cb.hahajie.cn

[E12] 统计某字符出现次数
来源：http://yz.asd995.cn

Py:   s.count("a")
来源：http://rq.521024.cn

PHP:  substr_count($s, "a");
来源：http://vv.hahajie.cn

JS:   s.split("a").length - 1
来源：http://zi.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://hx.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qd.521024.cn

Go:   strings.Count(s, "a")
来源：http://gx.shxzukj.cn

Ruby: s.count("a")
来源：http://zp.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://va.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://od.colortex.cn

Py:   for ch in s: print(ch)
来源：http://tc.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eh.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yb.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cg.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xm.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cn.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vk.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hj.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://gx.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://se.jctech888.com.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ms.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eb.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://um.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dn.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dn.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ob.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hb.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://gl.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://en.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ak.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kc.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nu.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zd.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tw.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ts.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ac.gzmigu.cn

[E16] 数字千分位
来源：http://dk.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://ol.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://to.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ea.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oa.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pc.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://on.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gr.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://rp.asd995.cn

[E17] 首字母大写
来源：http://cx.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://za.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lg.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ki.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qv.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://op.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ny.jctech888.com.cn

Ruby: s.capitalize
来源：http://cd.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ea.szsharing.cn

[E18] 模板占位符替换
来源：http://gm.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bw.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bp.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ya.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ud.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cb.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://le.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ej.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ye.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://th.hnjuh.cn

Py:   s.splitlines()
来源：http://gz.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zf.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ga.521024.cn

TS:   s.split(/\r?\n/)
来源：http://ip.haigaiapp.cn

Java: s.lines().toList()
来源：http://mc.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://vd.colortex.cn

Ruby: s.lines
来源：http://xy.haigaiapp.cn

C#:   s.Split('\n')
来源：http://er.colortex.cn

[E20] 判断字符串是否为空
来源：http://xw.huixinmuqiang.cn

Py:   if not s:
来源：http://ke.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lm.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://al.hahajie.cn

TS:   if (s === "") {}
来源：http://jp.521024.cn

Java: if (s.isEmpty()) {}
来源：http://lx.gzmigu.cn

Go:   if s == "" {}
来源：http://cy.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://no.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hp.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://ua.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lt.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dg.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://er.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://un.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ip.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://hp.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hr.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wy.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://li.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yn.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kv.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xg.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jv.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nk.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ac.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://sr.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dk.yuexingan06.cn

================================================================================
来源：http://vw.yuntaijiaju.cn

F. 文件与目录
来源：http://dh.jctech888.com.cn

================================================================================
来源：http://fb.9csxet.cn

[F01] 读取整个文件
来源：http://yc.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cy.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://nr.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://im.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nu.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ae.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nh.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://ml.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://st.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://qq.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xo.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yl.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kj.shxzukj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dp.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jo.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lg.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vb.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://al.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://eq.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fi.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xg.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nc.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dh.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aq.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mf.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://kf.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ya.hahajie.cn

[F04] 追加写入文件
来源：http://og.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kq.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hh.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rt.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ry.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gq.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xz.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dp.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yw.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://po.szxytkj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://li.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://bi.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ki.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://cg.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xb.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://di.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://jg.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://xl.gzmigu.cn

[F06] 删除文件
来源：http://hw.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://pz.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://zw.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dh.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ru.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fb.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://yv.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://bl.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://gt.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ds.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zb.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cz.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ag.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mj.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gs.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sw.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zc.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hn.yuexingan06.cn

[F08] 遍历目录
来源：http://oi.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pu.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xu.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://rj.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://hr.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ch.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sw.asd995.cn

Ruby: Dir.children("dir")
来源：http://sc.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://fp.gzmigu.cn

[F09] 获取文件大小
来源：http://hc.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://hi.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://le.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://el.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://fv.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iq.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bi.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://al.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://wd.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://yp.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://al.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sd.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qn.nszjky.cn

TS:   path.extname("a.txt")
来源：http://zo.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rn.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vl.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bw.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://or.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://om.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mu.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cm.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zb.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dv.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zl.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uo.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zj.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zo.panjiajie.cn

[F12] CSV 读写
来源：http://yy.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ef.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sa.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qp.huixiangedu.cn

TS:   // 同上
来源：http://oi.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ja.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ut.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jk.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ln.nicolike.cn

================================================================================
来源：http://rz.bjjhwx.cn

G. 面向对象
来源：http://dm.bookmarksfly.cn

================================================================================
来源：http://dc.yuexingan06.cn

[G01] 定义类
来源：http://nr.huanxung.cn

Py:   class User: pass
来源：http://dd.jianghongdianzi.cn

PHP:  class User {}
来源：http://sa.newstarts.cn

JS:   class User {}
来源：http://nt.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://qh.bookmarksfly.cn

Java: class User {}
来源：http://de.newstarts.cn

Go:   type User struct { Name string }
来源：http://hu.shtwfgs.cn

Ruby: class User; end
来源：http://gp.jctech888.com.cn

C#:   class User {}
来源：http://jc.newstarts.cn

[G02] 构造函数
来源：http://ee.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://nb.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://go.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://pk.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://dr.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://sq.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ym.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://an.newstarts.cn


<!-- 参考信息 -->