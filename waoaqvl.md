代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sx.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dh.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vr.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jn.panjiajie.cn

[E06] 替换子串
来源：http://nr.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kq.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://fy.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wn.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://vj.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sl.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ak.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://no.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://in.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://rk.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qn.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dl.bookmarksfly.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wv.shxzukj.cn

TS:   s.split(",")
来源：http://ik.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sj.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://og.shxzskj.cn

Ruby: s.split(",");  s.split
来源：http://yr.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://io.9csxet.cn

[E08] 数组按分隔符合并
来源：http://bh.jctech888.com.cn

Py:   ",".join(items)
来源：http://qi.shxzskj.cn

PHP:  implode(",", $items);
来源：http://eg.lnxyls.cn

JS:   items.join(",")
来源：http://tt.shtwfgs.cn

TS:   items.join(",")
来源：http://ut.9csxet.cn

Java: String.join(",", items)
来源：http://fs.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://gv.jctech888.com.cn

Ruby: items.join(",")
来源：http://vo.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://td.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://fp.9csxet.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ic.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nk.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://la.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://aa.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://yd.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zi.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ft.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ri.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://lq.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uv.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ml.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://cx.yuntaijiaju.cn

TS:   "7".padStart(3, "0")
来源：http://ff.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://vh.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kk.lnxyls.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://en.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zx.shtwfgs.cn

[E11] 反转字符串
来源：http://ia.jianghongdianzi.cn

Py:   s[::-1]
来源：http://rc.haigaiapp.cn

PHP:  strrev($s);
来源：http://zr.bookmarksfly.cn

JS:   [...s].reverse().join("")
来源：http://xo.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://ms.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lb.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gi.bookmarksfly.cn

Ruby: s.reverse
来源：http://mt.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://st.nicolike.cn

[E12] 统计某字符出现次数
来源：http://ka.haigaiapp.cn

Py:   s.count("a")
来源：http://dd.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://sw.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://bf.szsharing.cn

TS:   s.split("a").length - 1
来源：http://xu.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ko.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://aq.asd995.cn

Ruby: s.count("a")
来源：http://cx.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://qw.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://bz.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ir.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nq.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ca.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bx.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wo.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fq.muxihuayi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eq.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oj.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://ql.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vj.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ey.9csxet.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bw.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qy.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fk.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://de.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tr.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yn.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://fr.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iu.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zd.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xi.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rg.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ns.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bl.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ta.huanxung.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://es.gzmigu.cn

[E16] 数字千分位
来源：http://ro.9csxet.cn

Py:   f"{1234567:,}"
来源：http://dv.lnxyls.cn

PHP:  number_format(1234567);
来源：http://sp.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://in.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kk.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ll.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fx.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wp.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://yt.shtwfgs.cn

[E17] 首字母大写
来源：http://ys.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gv.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pk.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mc.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://je.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uz.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bp.szxytkj.cn

Ruby: s.capitalize
来源：http://yy.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ck.wgjwhj.cn

[E18] 模板占位符替换
来源：http://jg.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dc.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://up.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lg.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nj.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ft.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lt.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qp.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dy.521024.cn

[E19] 多行文本按行拆分
来源：http://bh.newstarts.cn

Py:   s.splitlines()
来源：http://tt.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ps.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://lr.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://qh.521024.cn

Java: s.lines().toList()
来源：http://rl.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://kq.wgjwhj.cn

Ruby: s.lines
来源：http://bd.9csxet.cn

C#:   s.Split('\n')
来源：http://wn.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://fi.shxzskj.cn

Py:   if not s:
来源：http://ae.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ok.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ry.wgjwhj.cn

TS:   if (s === "") {}
来源：http://ro.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://ys.nszjky.cn

Go:   if s == "" {}
来源：http://jb.gzmigu.cn

Ruby: if s.empty?
来源：http://vr.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fd.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://yb.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uj.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hn.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rj.szsharing.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nt.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://si.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://zx.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rm.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sa.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://va.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qb.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hb.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://za.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hr.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vz.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qr.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://bs.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jq.szxytkj.cn

================================================================================
来源：http://rm.shtwfgs.cn

F. 文件与目录
来源：http://ni.newstarts.cn

================================================================================
来源：http://lj.lnxyls.cn

[F01] 读取整个文件
来源：http://nk.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hy.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://bp.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yi.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qa.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qy.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vj.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://et.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://no.haigaiapp.cn

[F02] 逐行读取文件
来源：http://vz.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ev.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zf.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://et.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wh.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://im.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yk.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://we.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hi.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://ac.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gp.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pv.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bb.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mf.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tx.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zc.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://wd.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bv.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://ky.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kk.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dg.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sf.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ln.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fz.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ka.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kr.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yh.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://gm.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cm.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://bt.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://vh.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://wb.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vc.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ny.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://cw.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://cf.hnjuh.cn

[F06] 删除文件
来源：http://ay.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://xe.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://nl.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nc.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://am.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mn.521024.cn

Go:   os.Remove("a.txt")
来源：http://qp.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://mz.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://tj.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://kb.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dc.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cu.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qz.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eo.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qc.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://md.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://db.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vs.asd995.cn

[F08] 遍历目录
来源：http://mc.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ty.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mz.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://ea.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://mg.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zh.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ra.huanxung.cn

Ruby: Dir.children("dir")
来源：http://ar.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://to.colortex.cn

[F09] 获取文件大小
来源：http://un.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://cc.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://wg.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://vk.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://ca.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vd.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dh.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://wi.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ha.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://ny.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pi.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ff.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bq.huanxung.cn

TS:   path.extname("a.txt")
来源：http://fg.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dr.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oo.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://de.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xv.jctech888.com.cn

[F11] 复制与移动文件
来源：http://pc.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pc.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cz.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ll.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wv.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://un.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yx.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iz.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ra.gzmigu.cn

[F12] CSV 读写
来源：http://vp.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hr.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bi.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hl.panjiajie.cn

TS:   // 同上
来源：http://sq.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gj.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rt.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gt.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pj.huixinmuqiang.cn

================================================================================
来源：http://hj.yuntaijiaju.cn

G. 面向对象
来源：http://nv.bjjhwx.cn

================================================================================
来源：http://yk.szsharing.cn

[G01] 定义类
来源：http://zm.shxzskj.cn

Py:   class User: pass
来源：http://vp.shxzskj.cn

PHP:  class User {}
来源：http://ip.huixinmuqiang.cn

JS:   class User {}
来源：http://tr.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://we.huixinmuqiang.cn

Java: class User {}
来源：http://cl.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://wa.jianghongdianzi.cn

Ruby: class User; end
来源：http://wx.huanxung.cn

C#:   class User {}
来源：http://xo.newstarts.cn

[G02] 构造函数
来源：http://lf.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://sn.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://um.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://ip.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://us.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://gn.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xi.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://oz.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://ed.jctech888.com.cn

[G03] 实例属性
来源：http://cs.shtwfgs.cn

Py:   self.name = "x"
来源：http://fv.hnjuh.cn

PHP:  public string $name = "x";
来源：http://gt.chemitech.net.cn

JS:   this.name = "x";
来源：http://mn.asd995.cn

TS:   name: string = "x";
来源：http://lb.521024.cn

Java: private String name;
来源：http://ze.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lk.muxihuayi.cn

Ruby: @name = "x"
来源：http://qx.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://ad.colortex.cn

[G04] 定义方法
来源：http://yf.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://vk.nszjky.cn


<!-- 参考信息 -->