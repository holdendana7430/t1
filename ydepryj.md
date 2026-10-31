代发 wailian999

Go:   strings.Join(items, ",")
来源：http://qy.shtwfgs.cn

Ruby: items.join(",")
来源：http://pq.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://vy.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://op.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tq.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xe.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://zj.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://cx.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://wo.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yv.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yc.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kf.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://la.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ob.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://et.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://bz.521024.cn

TS:   "7".padStart(3, "0")
来源：http://yc.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://ad.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kl.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sy.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://km.shxzukj.cn

[E11] 反转字符串
来源：http://vc.shxzskj.cn

Py:   s[::-1]
来源：http://nl.bjjhwx.cn

PHP:  strrev($s);
来源：http://ea.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://ve.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://qm.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qj.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pc.asd995.cn

Ruby: s.reverse
来源：http://rr.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ka.521024.cn

[E12] 统计某字符出现次数
来源：http://sy.szsharing.cn

Py:   s.count("a")
来源：http://rk.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://lt.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://rb.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://vc.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jy.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://tb.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://le.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://my.colortex.cn

[E13] 逐字符遍历
来源：http://er.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://yy.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ih.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dv.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yv.newstarts.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cf.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://at.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cs.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eu.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://dn.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hg.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://aj.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kh.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cd.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lv.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xv.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://du.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ea.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://hg.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ev.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ww.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yt.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ga.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vj.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mt.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cz.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kh.shtwfgs.cn

[E16] 数字千分位
来源：http://fh.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://lj.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://yk.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ex.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hd.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lq.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ht.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ub.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://vi.wgjwhj.cn

[E17] 首字母大写
来源：http://xh.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ds.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jf.huixiangedu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kd.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cx.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qq.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rb.huanxung.cn

Ruby: s.capitalize
来源：http://hn.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wt.9csxet.cn

[E18] 模板占位符替换
来源：http://db.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xj.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xf.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ki.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dq.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ok.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sc.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cy.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nm.nszjky.cn

[E19] 多行文本按行拆分
来源：http://ct.newstarts.cn

Py:   s.splitlines()
来源：http://vd.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tb.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://oo.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://sn.haigaiapp.cn

Java: s.lines().toList()
来源：http://xq.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://ek.shxzukj.cn

Ruby: s.lines
来源：http://xq.szxytkj.cn

C#:   s.Split('\n')
来源：http://ot.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://rc.huixiangedu.cn

Py:   if not s:
来源：http://jn.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ct.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rp.colortex.cn

TS:   if (s === "") {}
来源：http://mx.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://wq.bjjhwx.cn

Go:   if s == "" {}
来源：http://cb.asd995.cn

Ruby: if s.empty?
来源：http://hv.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bt.nszjky.cn

[E21] 超长截断加省略号
来源：http://gp.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cj.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xs.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pc.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xk.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://of.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://pb.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cq.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vt.huanxung.cn

[E22] 字节长度与字符长度
来源：http://dj.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rp.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wm.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uy.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wp.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xb.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xk.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://kr.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cr.yuexingan06.cn

================================================================================
来源：http://dh.haigaiapp.cn

F. 文件与目录
来源：http://vb.wgjwhj.cn

================================================================================
来源：http://in.newstarts.cn

[F01] 读取整个文件
来源：http://ka.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nz.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://wh.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vn.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ly.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bq.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nh.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://it.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://ri.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://ey.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://li.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vl.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ah.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ru.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wc.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fj.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xh.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jr.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://rm.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iw.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bu.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tv.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zg.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://db.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xw.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://yo.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yo.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://zi.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dj.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lf.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xv.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://te.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://de.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pn.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lx.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cj.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://yc.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mk.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://fw.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://hd.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://vr.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bl.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sj.521024.cn

Ruby: File.exist?("a.txt")
来源：http://ff.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://gw.szsharing.cn

[F06] 删除文件
来源：http://hp.521024.cn

Py:   os.remove("a.txt")
来源：http://tk.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://kl.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kk.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tl.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qk.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://et.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://yf.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://ah.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://ku.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cy.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rg.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xl.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ar.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://th.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lc.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lq.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jl.bjjhwx.cn

[F08] 遍历目录
来源：http://vo.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://et.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yl.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://zj.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://ke.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mc.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yj.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://ns.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://fu.9csxet.cn

[F09] 获取文件大小
来源：http://sa.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://yq.asd995.cn

PHP:  filesize("a.txt");
来源：http://cz.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://gn.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://bn.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gj.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://he.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://ai.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://ig.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://ka.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bk.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ha.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hg.szsharing.cn

TS:   path.extname("a.txt")
来源：http://tl.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mt.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jt.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yu.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jz.nicolike.cn

[F11] 复制与移动文件
来源：http://wt.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uq.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ee.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uu.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xk.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fn.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rp.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fe.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rm.bookmarksfly.cn

[F12] CSV 读写
来源：http://gv.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rv.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ev.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://le.muxihuayi.cn

TS:   // 同上
来源：http://zf.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nu.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xx.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qe.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uz.szxytkj.cn

================================================================================
来源：http://mm.haigaiapp.cn

G. 面向对象
来源：http://wz.lnxyls.cn

================================================================================
来源：http://jl.asd995.cn

[G01] 定义类
来源：http://gt.jianghongdianzi.cn

Py:   class User: pass
来源：http://vu.nszjky.cn

PHP:  class User {}
来源：http://ab.colortex.cn

JS:   class User {}
来源：http://cm.wgjwhj.cn

TS:   class User { name: string = ""; }
来源：http://ii.szsharing.cn

Java: class User {}
来源：http://ma.nszjky.cn

Go:   type User struct { Name string }
来源：http://vm.huixiangedu.cn

Ruby: class User; end
来源：http://kc.shxzukj.cn

C#:   class User {}
来源：http://wf.shxzskj.cn

[G02] 构造函数
来源：http://wd.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://tz.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://gj.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://me.colortex.cn

TS:   constructor(public name: string) {}
来源：http://vt.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://hz.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nf.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://dl.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://yw.panjiajie.cn

[G03] 实例属性
来源：http://iv.hahajie.cn

Py:   self.name = "x"
来源：http://ye.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://ls.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://ow.9csxet.cn

TS:   name: string = "x";
来源：http://av.nszjky.cn

Java: private String name;
来源：http://qs.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ig.nszjky.cn

Ruby: @name = "x"
来源：http://el.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://ya.chemitech.net.cn

[G04] 定义方法
来源：http://gb.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://eb.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vv.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://yf.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://wl.shxzukj.cn

Java: String greet() { return name; }
来源：http://gs.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ry.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://jm.nszjky.cn

C#:   public string Greet() => Name;
来源：http://ty.nicolike.cn

[G05] 继承
来源：http://cr.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://pt.colortex.cn

PHP:  class Admin extends User {}
来源：http://nd.szxytkj.cn

JS:   class Admin extends User {}
来源：http://uj.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://rb.shxzskj.cn

Java: class Admin extends User {}
来源：http://kz.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fz.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://wb.yuexingan06.cn

C#:   class Admin : User {}
来源：http://yf.bookmarksfly.cn

[G06] 重写方法
来源：http://sr.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://bq.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xf.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://tz.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://wa.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://hr.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ln.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://ab.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://ze.bjjhwx.cn

[G07] 调用父类方法
来源：http://ye.nszjky.cn

Py:   super().greet()
来源：http://oi.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://po.nszjky.cn


<!-- 参考信息 -->