代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ls.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rz.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lf.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zm.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://wa.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://se.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://za.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://jx.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://na.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://rt.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wf.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wh.asd995.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oy.szxytkj.cn

[E11] 反转字符串
来源：http://kc.chemitech.net.cn

Py:   s[::-1]
来源：http://mu.asd995.cn

PHP:  strrev($s);
来源：http://ph.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://tx.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://mt.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bw.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fq.jctech888.com.cn

Ruby: s.reverse
来源：http://rb.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yc.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://jh.shxzukj.cn

Py:   s.count("a")
来源：http://ba.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://sw.hahajie.cn

JS:   s.split("a").length - 1
来源：http://nz.hahajie.cn

TS:   s.split("a").length - 1
来源：http://zr.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ks.colortex.cn

Go:   strings.Count(s, "a")
来源：http://gx.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://rw.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://wb.lnxyls.cn

[E13] 逐字符遍历
来源：http://sp.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ud.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fq.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xs.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xb.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uh.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fz.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wh.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pn.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://dp.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rv.huixiangedu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nu.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fl.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wt.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mb.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cv.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uz.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xs.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://hu.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cv.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cx.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://in.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hn.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nr.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://br.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://np.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mq.newstarts.cn

[E16] 数字千分位
来源：http://qi.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://ri.hnjuh.cn

PHP:  number_format(1234567);
来源：http://op.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tg.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mu.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ir.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cu.muxihuayi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fo.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://pw.9csxet.cn

[E17] 首字母大写
来源：http://nz.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fq.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://km.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ee.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pf.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gf.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://to.shxzskj.cn

Ruby: s.capitalize
来源：http://yx.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vp.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://fi.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lc.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nl.521024.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gr.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jz.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mx.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mz.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fj.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xe.wgjwhj.cn

[E19] 多行文本按行拆分
来源：http://qs.nszjky.cn

Py:   s.splitlines()
来源：http://nb.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hy.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://tp.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://jx.huanxung.cn

Java: s.lines().toList()
来源：http://kf.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://gu.asd995.cn

Ruby: s.lines
来源：http://aw.shxzukj.cn

C#:   s.Split('\n')
来源：http://xo.szsharing.cn

[E20] 判断字符串是否为空
来源：http://ov.huanxung.cn

Py:   if not s:
来源：http://hb.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qu.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bj.lnxyls.cn

TS:   if (s === "") {}
来源：http://yr.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ae.hahajie.cn

Go:   if s == "" {}
来源：http://vi.huixiangedu.cn

Ruby: if s.empty?
来源：http://jo.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qp.szxytkj.cn

[E21] 超长截断加省略号
来源：http://ys.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cq.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hm.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ce.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://by.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cb.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://th.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fc.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yx.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://xw.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zr.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://no.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://re.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hp.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ee.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yv.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://ue.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kd.hahajie.cn

================================================================================
来源：http://ry.wgjwhj.cn

F. 文件与目录
来源：http://zk.shxzukj.cn

================================================================================
来源：http://mq.hahajie.cn

[F01] 读取整个文件
来源：http://sm.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://az.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://kh.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://an.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fo.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://de.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wf.nicolike.cn

Ruby: File.read("a.txt")
来源：http://fq.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://nc.newstarts.cn

[F02] 逐行读取文件
来源：http://sb.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rw.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tm.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ho.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nk.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ff.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://km.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://az.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ae.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://wc.nszjky.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cx.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://up.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xr.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bm.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://th.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ih.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://oe.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wk.yuexingan06.cn

[F04] 追加写入文件
来源：http://wm.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vk.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uv.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sc.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zt.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ns.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lt.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gy.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://et.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://xw.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mq.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://cp.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://pc.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://vh.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ta.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nf.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://oo.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://df.9csxet.cn

[F06] 删除文件
来源：http://qz.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://wp.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://nz.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tl.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ag.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ac.colortex.cn

Go:   os.Remove("a.txt")
来源：http://gw.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://lh.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://fp.asd995.cn

[F07] 创建目录（含多级）
来源：http://xm.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ng.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ao.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nz.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oq.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bo.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://by.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://il.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qw.wgjwhj.cn

[F08] 遍历目录
来源：http://iz.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dh.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ao.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://vp.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://yf.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jm.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ls.asd995.cn

Ruby: Dir.children("dir")
来源：http://lr.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://ra.nszjky.cn

[F09] 获取文件大小
来源：http://lc.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://yg.521024.cn

PHP:  filesize("a.txt");
来源：http://ua.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://gt.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://ij.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yo.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ki.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://lr.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://mu.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://xc.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bf.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xh.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ys.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://ha.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rd.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kk.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ev.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cg.muxihuayi.cn

[F11] 复制与移动文件
来源：http://qr.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ov.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mh.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uy.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nq.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sp.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://da.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ql.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pr.bookmarksfly.cn

[F12] CSV 读写
来源：http://nt.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ov.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sk.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yb.jctech888.com.cn

TS:   // 同上
来源：http://ao.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oy.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://od.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ch.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://py.jctech888.com.cn

================================================================================
来源：http://bn.asd995.cn

G. 面向对象
来源：http://fg.chemitech.net.cn

================================================================================
来源：http://ny.wgjwhj.cn

[G01] 定义类
来源：http://tc.huanxung.cn

Py:   class User: pass
来源：http://ae.huanxung.cn

PHP:  class User {}
来源：http://ns.hahajie.cn

JS:   class User {}
来源：http://ne.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://pa.shxzukj.cn

Java: class User {}
来源：http://ep.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://mw.szsharing.cn

Ruby: class User; end
来源：http://nf.lnxyls.cn

C#:   class User {}
来源：http://sn.szsharing.cn

[G02] 构造函数
来源：http://sd.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://hm.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://az.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://aq.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://qt.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://wg.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dt.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ol.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://pi.yuexingan06.cn

[G03] 实例属性
来源：http://zn.gzmigu.cn

Py:   self.name = "x"
来源：http://mn.9csxet.cn

PHP:  public string $name = "x";
来源：http://go.lnxyls.cn

JS:   this.name = "x";
来源：http://ez.asd995.cn

TS:   name: string = "x";
来源：http://uh.yuexingan06.cn

Java: private String name;
来源：http://vd.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bb.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://iu.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://fh.yuntaijiaju.cn

[G04] 定义方法
来源：http://jt.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://bf.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lo.newstarts.cn

JS:   greet() { return this.name; }
来源：http://ou.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://ap.szsharing.cn

Java: String greet() { return name; }
来源：http://uz.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://en.szxytkj.cn

Ruby: def greet; @name; end
来源：http://xb.asd995.cn

C#:   public string Greet() => Name;
来源：http://ky.shtwfgs.cn

[G05] 继承
来源：http://ho.9csxet.cn

Py:   class Admin(User): pass
来源：http://jc.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://ug.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://go.panjiajie.cn

TS:   class Admin extends User {}
来源：http://bg.nicolike.cn

Java: class Admin extends User {}
来源：http://rw.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://do.shxzskj.cn

Ruby: class Admin < User; end
来源：http://kj.huanxung.cn

C#:   class Admin : User {}
来源：http://sd.asd995.cn

[G06] 重写方法
来源：http://qw.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://to.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uk.colortex.cn

JS:   greet() { return "admin"; }
来源：http://cy.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://yf.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://bx.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jp.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://hv.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://xq.bookmarksfly.cn

[G07] 调用父类方法
来源：http://tw.panjiajie.cn

Py:   super().greet()
来源：http://ka.newstarts.cn

PHP:  parent::greet();
来源：http://ob.panjiajie.cn

JS:   super.greet();
来源：http://qq.muxihuayi.cn

TS:   super.greet();
来源：http://lz.lnxyls.cn

Java: super.greet();
来源：http://rr.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://no.huixiangedu.cn

Ruby: super
来源：http://wu.nicolike.cn

C#:   base.Greet();
来源：http://yh.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://qq.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hj.wgjwhj.cn


<!-- 参考信息 -->