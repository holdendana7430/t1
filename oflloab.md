代发 wailian999

Go:   strings.Index(s, "x")
来源：http://aw.521024.cn

Ruby: s.index("x")
来源：http://wu.521024.cn

C#:   s.IndexOf("x")
来源：http://lu.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ms.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bm.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hf.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ki.szsharing.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cl.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sv.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rj.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eh.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bc.huixiangedu.cn

[E06] 替换子串
来源：http://vv.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://im.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://mp.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iz.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://cz.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mt.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eb.hahajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sd.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://ny.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://gq.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xp.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wz.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lr.haigaiapp.cn

TS:   s.split(",")
来源：http://pp.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zw.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iz.nicolike.cn

Ruby: s.split(",");  s.split
来源：http://vu.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dj.hahajie.cn

[E08] 数组按分隔符合并
来源：http://vc.jctech888.com.cn

Py:   ",".join(items)
来源：http://in.521024.cn

PHP:  implode(",", $items);
来源：http://qw.chemitech.net.cn

JS:   items.join(",")
来源：http://yf.yuntaijiaju.cn

TS:   items.join(",")
来源：http://mn.szxytkj.cn

Java: String.join(",", items)
来源：http://wt.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://ux.bookmarksfly.cn

Ruby: items.join(",")
来源：http://ti.hahajie.cn

C#:   string.Join(",", items)
来源：http://yd.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://sb.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hc.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xm.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://wt.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://sf.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://cg.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yq.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ig.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ze.shtwfgs.cn

[E10] 左侧补零 / 定长填充
来源：http://ap.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vp.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pi.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://lj.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://ab.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://fe.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bc.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xm.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eh.jianghongdianzi.cn

[E11] 反转字符串
来源：http://qn.huixiangedu.cn

Py:   s[::-1]
来源：http://vv.wgjwhj.cn

PHP:  strrev($s);
来源：http://nh.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://ly.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://xn.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pw.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://se.nszjky.cn

Ruby: s.reverse
来源：http://pf.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pv.nszjky.cn

[E12] 统计某字符出现次数
来源：http://nk.szxytkj.cn

Py:   s.count("a")
来源：http://og.asd995.cn

PHP:  substr_count($s, "a");
来源：http://ge.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://ap.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://fi.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dd.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://wg.hnjuh.cn

Ruby: s.count("a")
来源：http://zw.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://su.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://qh.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://nw.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uz.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ti.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mo.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ud.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vn.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://im.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yl.asd995.cn

[E14] URL 编码与 Base64
来源：http://qf.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gy.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qf.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ue.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jz.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uc.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tn.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vu.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jr.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://ne.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ui.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dy.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cd.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ka.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ry.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xn.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vl.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dm.jianghongdianzi.cn

[E16] 数字千分位
来源：http://yw.colortex.cn

Py:   f"{1234567:,}"
来源：http://fu.colortex.cn

PHP:  number_format(1234567);
来源：http://ju.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://db.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vk.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ay.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://au.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oy.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://su.jctech888.com.cn

[E17] 首字母大写
来源：http://dv.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sq.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ak.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dy.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pz.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qo.asd995.cn

Ruby: s.capitalize
来源：http://pp.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fa.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://px.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oq.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gh.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yh.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://do.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ck.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kk.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bn.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ph.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://cg.yuexingan06.cn

Py:   s.splitlines()
来源：http://pg.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fz.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ay.bjjhwx.cn

TS:   s.split(/\r?\n/)
来源：http://ou.521024.cn

Java: s.lines().toList()
来源：http://tf.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://qi.hnjuh.cn

Ruby: s.lines
来源：http://ft.jctech888.com.cn

C#:   s.Split('\n')
来源：http://xk.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://pr.colortex.cn

Py:   if not s:
来源：http://ax.nszjky.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ff.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sd.panjiajie.cn

TS:   if (s === "") {}
来源：http://ul.newstarts.cn

Java: if (s.isEmpty()) {}
来源：http://hl.nszjky.cn

Go:   if s == "" {}
来源：http://bs.lnxyls.cn

Ruby: if s.empty?
来源：http://rb.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hh.lnxyls.cn

[E21] 超长截断加省略号
来源：http://fo.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ys.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yv.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sk.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ht.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uo.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://fc.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cj.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vh.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://eq.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ky.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ch.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cz.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ba.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://um.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yo.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://cr.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kf.shtwfgs.cn

================================================================================
来源：http://lc.9csxet.cn

F. 文件与目录
来源：http://qn.szsharing.cn

================================================================================
来源：http://wq.chemitech.net.cn

[F01] 读取整个文件
来源：http://kn.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ko.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://ay.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bh.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wb.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bw.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ig.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://oo.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ze.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ip.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fh.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qy.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nv.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gd.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dv.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ht.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hp.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ua.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://ji.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nm.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ld.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ed.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bq.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mn.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vo.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://zx.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kd.nicolike.cn

[F04] 追加写入文件
来源：http://gj.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xx.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wb.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aw.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oe.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uk.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bl.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hn.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qo.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://rz.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dd.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://pi.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://zk.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://vn.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xk.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wl.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://ke.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://cf.shtwfgs.cn

[F06] 删除文件
来源：http://wd.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://zv.colortex.cn

PHP:  unlink("a.txt");
来源：http://zp.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://du.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rl.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ek.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://qv.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://xl.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://sx.nszjky.cn

[F07] 创建目录（含多级）
来源：http://yb.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jb.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bb.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jx.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eh.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ot.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tm.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wl.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wt.shxzukj.cn

[F08] 遍历目录
来源：http://zc.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://po.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nj.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://zu.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://fx.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://el.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pa.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://jy.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://sy.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://wk.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://jl.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://tk.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://bs.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://gf.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iq.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lk.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://rl.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://fi.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://ak.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nt.szsharing.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tg.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hg.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://bd.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yi.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fq.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mn.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tc.huixiangedu.cn

[F11] 复制与移动文件
来源：http://wv.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ka.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oz.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vd.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ot.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rf.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://me.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qe.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://is.jianghongdianzi.cn

[F12] CSV 读写
来源：http://mm.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://py.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ap.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bo.521024.cn

TS:   // 同上
来源：http://to.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cx.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rj.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fo.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lr.chemitech.net.cn

================================================================================
来源：http://ne.huixinmuqiang.cn

G. 面向对象
来源：http://rh.bookmarksfly.cn

================================================================================
来源：http://nw.hahajie.cn

[G01] 定义类
来源：http://ok.colortex.cn

Py:   class User: pass
来源：http://rv.gzmigu.cn

PHP:  class User {}
来源：http://hz.muxihuayi.cn

JS:   class User {}
来源：http://fy.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://jb.bjjhwx.cn

Java: class User {}
来源：http://ug.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://mc.nicolike.cn

Ruby: class User; end
来源：http://fe.wgjwhj.cn

C#:   class User {}
来源：http://pp.jianghongdianzi.cn

[G02] 构造函数
来源：http://fz.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://xe.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://dy.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://gl.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://gs.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://pi.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gc.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://iq.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://uu.nszjky.cn

[G03] 实例属性
来源：http://ld.haigaiapp.cn

Py:   self.name = "x"
来源：http://no.hahajie.cn

PHP:  public string $name = "x";
来源：http://fa.yuexingan06.cn


<!-- 参考信息 -->