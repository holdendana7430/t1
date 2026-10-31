代发 wailian999

Go:   strings.Index(s, "x")
来源：http://zo.newstarts.cn

Ruby: s.index("x")
来源：http://yf.asd995.cn

C#:   s.IndexOf("x")
来源：http://ow.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oo.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bv.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://da.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tx.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ik.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yp.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rj.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yl.bookmarksfly.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jz.521024.cn

[E06] 替换子串
来源：http://fl.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pg.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://xq.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tj.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://fg.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pu.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yp.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mz.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://bi.szsharing.cn

[E07] 按分隔符拆分
来源：http://ng.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nd.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nv.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yi.muxihuayi.cn

TS:   s.split(",")
来源：http://um.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://it.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vp.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://mf.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dl.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://zg.bookmarksfly.cn

Py:   ",".join(items)
来源：http://tb.shxzukj.cn

PHP:  implode(",", $items);
来源：http://fr.jianghongdianzi.cn

JS:   items.join(",")
来源：http://fc.newstarts.cn

TS:   items.join(",")
来源：http://gj.szsharing.cn

Java: String.join(",", items)
来源：http://gt.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://yh.hnjuh.cn

Ruby: items.join(",")
来源：http://sz.nszjky.cn

C#:   string.Join(",", items)
来源：http://tn.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://zr.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fj.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gl.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://wu.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://tp.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://vs.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cx.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qd.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mr.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://sz.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vh.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yd.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://ts.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://fv.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://tv.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rs.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mm.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lg.yuexingan06.cn

[E11] 反转字符串
来源：http://nc.asd995.cn

Py:   s[::-1]
来源：http://sh.521024.cn

PHP:  strrev($s);
来源：http://fb.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://ks.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://dw.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xs.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qo.lnxyls.cn

Ruby: s.reverse
来源：http://lh.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nq.asd995.cn

[E12] 统计某字符出现次数
来源：http://xc.nszjky.cn

Py:   s.count("a")
来源：http://wm.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://mp.asd995.cn

JS:   s.split("a").length - 1
来源：http://tj.521024.cn

TS:   s.split("a").length - 1
来源：http://sa.newstarts.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rg.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://gn.szsharing.cn

Ruby: s.count("a")
来源：http://xm.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://dq.jctech888.com.cn

[E13] 逐字符遍历
来源：http://nq.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://ad.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pt.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ro.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wq.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ir.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mr.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uz.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yg.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://jb.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mc.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vy.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wj.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yu.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ii.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hf.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ch.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://ud.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uj.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://au.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gw.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qb.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fv.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ht.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oy.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ux.szxytkj.cn

[E16] 数字千分位
来源：http://fq.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://tc.shxzskj.cn

PHP:  number_format(1234567);
来源：http://du.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zt.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yj.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rb.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ae.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tv.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://gi.bookmarksfly.cn

[E17] 首字母大写
来源：http://fe.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://px.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tg.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cr.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yz.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nh.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cb.wgjwhj.cn

Ruby: s.capitalize
来源：http://da.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dc.shxzskj.cn

[E18] 模板占位符替换
来源：http://ck.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ax.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nd.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ki.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ph.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ti.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iv.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ho.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fn.newstarts.cn

[E19] 多行文本按行拆分
来源：http://zx.521024.cn

Py:   s.splitlines()
来源：http://qt.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://id.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://cq.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://wy.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://jx.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://of.huixiangedu.cn

Ruby: s.lines
来源：http://pl.nszjky.cn

C#:   s.Split('\n')
来源：http://lv.nicolike.cn

[E20] 判断字符串是否为空
来源：http://sl.huixiangedu.cn

Py:   if not s:
来源：http://uo.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qw.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kl.shtwfgs.cn

TS:   if (s === "") {}
来源：http://ag.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://hg.asd995.cn

Go:   if s == "" {}
来源：http://ur.chemitech.net.cn

Ruby: if s.empty?
来源：http://vc.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ri.gzmigu.cn

[E21] 超长截断加省略号
来源：http://cx.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wj.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ks.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vo.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ot.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ta.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://nh.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ch.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cz.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://tf.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ul.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://be.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lj.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ni.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ci.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kr.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://mo.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jj.szsharing.cn

================================================================================
来源：http://gv.wgjwhj.cn

F. 文件与目录
来源：http://ho.bjjhwx.cn

================================================================================
来源：http://ji.lnxyls.cn

[F01] 读取整个文件
来源：http://er.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gf.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://yz.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eq.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hu.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lj.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nd.colortex.cn

Ruby: File.read("a.txt")
来源：http://bo.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://kh.chemitech.net.cn

[F02] 逐行读取文件
来源：http://jw.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nm.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eb.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://na.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://as.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pf.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wj.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mh.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wo.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://vk.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cz.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xm.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ih.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wh.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ij.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ys.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://gr.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rj.szxytkj.cn

[F04] 追加写入文件
来源：http://tc.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lz.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sc.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tz.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dt.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jg.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ba.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ce.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lg.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://ym.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ea.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://xq.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://qs.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://xx.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ia.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://av.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://uj.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://xt.chemitech.net.cn

[F06] 删除文件
来源：http://on.szsharing.cn

Py:   os.remove("a.txt")
来源：http://ks.9csxet.cn

PHP:  unlink("a.txt");
来源：http://dx.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xw.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wd.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://un.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://pp.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://kn.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://yy.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://rv.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://re.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bv.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eq.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tu.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hs.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mt.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tw.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eo.huanxung.cn

[F08] 遍历目录
来源：http://tr.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vs.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cd.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://ba.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://sg.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kc.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ye.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://vq.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://pn.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://ye.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://eq.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://rh.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://qf.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://ld.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cr.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yo.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://mr.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://lz.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://tu.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bh.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dr.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gr.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://dk.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ps.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jr.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xc.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rr.hahajie.cn

[F11] 复制与移动文件
来源：http://ox.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://of.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xo.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hy.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zq.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ly.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rs.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cz.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ts.hahajie.cn

[F12] CSV 读写
来源：http://ll.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://au.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://je.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bg.shtwfgs.cn

TS:   // 同上
来源：http://bb.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vm.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oz.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zd.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nk.shxzukj.cn

================================================================================
来源：http://de.lnxyls.cn

G. 面向对象
来源：http://sq.haigaiapp.cn

================================================================================
来源：http://no.haigaiapp.cn

[G01] 定义类
来源：http://gb.jctech888.com.cn

Py:   class User: pass
来源：http://xq.bjjhwx.cn

PHP:  class User {}
来源：http://pg.hnjuh.cn

JS:   class User {}
来源：http://rn.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://qs.shxzukj.cn

Java: class User {}
来源：http://mv.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://ls.nicolike.cn

Ruby: class User; end
来源：http://te.jianghongdianzi.cn

C#:   class User {}
来源：http://il.muxihuayi.cn

[G02] 构造函数
来源：http://io.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://cf.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://gl.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ky.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://jo.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://va.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jk.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://lb.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://si.shtwfgs.cn

[G03] 实例属性
来源：http://uc.szsharing.cn

Py:   self.name = "x"
来源：http://tx.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://xw.hnjuh.cn


<!-- 参考信息 -->