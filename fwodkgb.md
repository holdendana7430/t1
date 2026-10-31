代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ud.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://eg.nicolike.cn

Java: s.substring(1, 4)
来源：http://jr.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ij.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tl.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://nl.wgjwhj.cn

[E04] 查找子串位置
来源：http://mp.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://yo.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://li.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kz.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ra.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://za.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://ia.shtwfgs.cn

Ruby: s.index("x")
来源：http://hq.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://uh.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uw.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gj.huixinmuqiang.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zn.huixinmuqiang.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://co.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ha.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xj.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ph.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cf.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://on.szsharing.cn

[E06] 替换子串
来源：http://hq.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ry.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://ab.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ut.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://bs.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yi.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pb.haigaiapp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xq.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://uy.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://ic.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cy.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dv.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://es.muxihuayi.cn

TS:   s.split(",")
来源：http://jn.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://he.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qw.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://bo.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://um.huixiangedu.cn

Py:   ",".join(items)
来源：http://cf.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://no.shxzukj.cn

JS:   items.join(",")
来源：http://xe.hnjuh.cn

TS:   items.join(",")
来源：http://zp.asd995.cn

Java: String.join(",", items)
来源：http://bx.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://ze.chemitech.net.cn

Ruby: items.join(",")
来源：http://ou.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://ad.nszjky.cn

[E09] 去除所有空白字符
来源：http://dx.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dm.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zx.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://jt.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://lx.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://qo.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ox.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jv.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ri.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://bl.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pv.521024.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eg.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://hf.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://rk.szsharing.cn

Java: String.format("%03d", 7)
来源：http://id.shxzukj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hj.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cl.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bd.nszjky.cn

[E11] 反转字符串
来源：http://ql.haigaiapp.cn

Py:   s[::-1]
来源：http://km.chemitech.net.cn

PHP:  strrev($s);
来源：http://gt.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://ye.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://eq.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ho.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lt.huixiangedu.cn

Ruby: s.reverse
来源：http://qu.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wn.nicolike.cn

[E12] 统计某字符出现次数
来源：http://cn.gzmigu.cn

Py:   s.count("a")
来源：http://nc.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://oz.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://nh.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://fb.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mq.521024.cn

Go:   strings.Count(s, "a")
来源：http://ch.gzmigu.cn

Ruby: s.count("a")
来源：http://eo.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://uc.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://bz.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://uk.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cc.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kj.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ac.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xq.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ka.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ki.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uj.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://re.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pq.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zl.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bb.9csxet.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gd.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vu.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vl.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://no.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ok.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://zp.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nu.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ym.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jg.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qm.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jn.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tz.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cz.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lp.huixinmuqiang.cn

[E16] 数字千分位
来源：http://cq.colortex.cn

Py:   f"{1234567:,}"
来源：http://ni.hnjuh.cn

PHP:  number_format(1234567);
来源：http://xw.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fm.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bw.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cl.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ui.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lg.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://rn.colortex.cn

[E17] 首字母大写
来源：http://ae.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kf.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gq.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qr.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gh.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hg.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oh.hnjuh.cn

Ruby: s.capitalize
来源：http://xa.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://df.521024.cn

[E18] 模板占位符替换
来源：http://hr.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ah.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hx.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sd.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fl.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tr.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bi.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zr.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ds.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://az.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://jf.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://on.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ou.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://sn.nszjky.cn

Java: s.lines().toList()
来源：http://wh.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://qe.yuexingan06.cn

Ruby: s.lines
来源：http://ep.bjjhwx.cn

C#:   s.Split('\n')
来源：http://cg.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://zm.nicolike.cn

Py:   if not s:
来源：http://cg.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zi.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zy.shtwfgs.cn

TS:   if (s === "") {}
来源：http://bh.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://rn.lnxyls.cn

Go:   if s == "" {}
来源：http://en.bookmarksfly.cn

Ruby: if s.empty?
来源：http://bo.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wb.colortex.cn

[E21] 超长截断加省略号
来源：http://ju.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hw.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yl.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ts.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ll.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qa.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nt.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dj.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pw.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://ia.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xy.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yf.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bq.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mh.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zk.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ex.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://fk.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bk.huixinmuqiang.cn

================================================================================
来源：http://zs.newstarts.cn

F. 文件与目录
来源：http://wk.szsharing.cn

================================================================================
来源：http://xc.jctech888.com.cn

[F01] 读取整个文件
来源：http://mm.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uv.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://iq.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zx.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wo.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bj.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://po.hahajie.cn

Ruby: File.read("a.txt")
来源：http://be.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://jb.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://aa.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dw.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://le.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ed.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bs.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gs.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ax.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kv.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xg.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://sf.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cg.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xo.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pt.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://js.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://el.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nj.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://tp.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uo.nszjky.cn

[F04] 追加写入文件
来源：http://xo.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fy.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kh.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ib.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nr.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://es.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oa.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cp.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qa.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://gy.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://us.521024.cn

PHP:  file_exists("a.txt");
来源：http://zk.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://az.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://rb.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://by.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://he.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://jf.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://vy.bookmarksfly.cn

[F06] 删除文件
来源：http://xe.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://fw.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://wo.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cz.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xr.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://do.asd995.cn

Go:   os.Remove("a.txt")
来源：http://ny.asd995.cn

Ruby: File.delete("a.txt")
来源：http://ts.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://ge.nicolike.cn

[F07] 创建目录（含多级）
来源：http://cj.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ee.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pv.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pj.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sg.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://js.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tr.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ek.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xd.colortex.cn

[F08] 遍历目录
来源：http://qj.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oi.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jc.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://ji.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://hh.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fe.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ce.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://to.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://ie.huanxung.cn

[F09] 获取文件大小
来源：http://dj.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://tg.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://sz.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://ue.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://wp.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ni.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qt.9csxet.cn

Ruby: File.size("a.txt")
来源：http://hn.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://oz.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ha.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://af.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gv.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uu.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://wd.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zo.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zl.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://la.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vg.panjiajie.cn

[F11] 复制与移动文件
来源：http://rj.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rm.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vb.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kh.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ns.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bw.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zf.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jg.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sw.shxzukj.cn

[F12] CSV 读写
来源：http://et.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jv.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zq.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kd.huanxung.cn

TS:   // 同上
来源：http://dj.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cm.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wi.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oh.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hj.szxytkj.cn

================================================================================
来源：http://yl.hahajie.cn

G. 面向对象
来源：http://gh.yuntaijiaju.cn

================================================================================
来源：http://at.yuntaijiaju.cn

[G01] 定义类
来源：http://fq.lnxyls.cn

Py:   class User: pass
来源：http://nr.lnxyls.cn

PHP:  class User {}
来源：http://yn.yuexingan06.cn

JS:   class User {}
来源：http://bw.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ls.gzmigu.cn

Java: class User {}
来源：http://tw.hahajie.cn

Go:   type User struct { Name string }
来源：http://uo.huixinmuqiang.cn

Ruby: class User; end
来源：http://sv.shxzskj.cn

C#:   class User {}
来源：http://sn.jianghongdianzi.cn


<!-- 参考信息 -->