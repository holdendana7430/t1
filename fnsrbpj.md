代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ad.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://we.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://di.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ul.shxzskj.cn

[E10] 左侧补零 / 定长填充
来源：http://nj.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lb.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://so.521024.cn

JS:   "7".padStart(3, "0")
来源：http://oc.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://zt.szsharing.cn

Java: String.format("%03d", 7)
来源：http://sx.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mw.asd995.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xp.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cs.chemitech.net.cn

[E11] 反转字符串
来源：http://yb.bookmarksfly.cn

Py:   s[::-1]
来源：http://ob.521024.cn

PHP:  strrev($s);
来源：http://hg.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://mz.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://hd.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fx.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zk.haigaiapp.cn

Ruby: s.reverse
来源：http://dd.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fj.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://fz.szxytkj.cn

Py:   s.count("a")
来源：http://hy.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://df.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://tc.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://vw.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yx.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://zk.panjiajie.cn

Ruby: s.count("a")
来源：http://qq.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://sq.shxzukj.cn

[E13] 逐字符遍历
来源：http://xp.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://bm.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://as.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qe.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wc.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ll.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fw.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qf.9csxet.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ue.huanxung.cn

[E14] URL 编码与 Base64
来源：http://jo.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iw.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ip.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nh.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bp.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://du.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vu.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uy.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jc.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://pk.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uy.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dw.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://va.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kt.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://na.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cf.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wu.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jb.muxihuayi.cn

[E16] 数字千分位
来源：http://nc.asd995.cn

Py:   f"{1234567:,}"
来源：http://my.newstarts.cn

PHP:  number_format(1234567);
来源：http://qj.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://os.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rp.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uc.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://li.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mw.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://rv.shxzskj.cn

[E17] 首字母大写
来源：http://rt.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vl.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://be.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://le.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tl.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://my.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://og.bookmarksfly.cn

Ruby: s.capitalize
来源：http://we.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dc.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://in.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pb.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dg.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sn.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jm.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fa.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ml.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fw.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uw.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://pq.chemitech.net.cn

Py:   s.splitlines()
来源：http://sm.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sj.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://zu.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://hz.shxzukj.cn

Java: s.lines().toList()
来源：http://cm.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://eg.newstarts.cn

Ruby: s.lines
来源：http://cw.hnjuh.cn

C#:   s.Split('\n')
来源：http://jk.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://eh.chemitech.net.cn

Py:   if not s:
来源：http://kp.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yb.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pi.shxzskj.cn

TS:   if (s === "") {}
来源：http://fd.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://kt.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://iz.bjjhwx.cn

Ruby: if s.empty?
来源：http://dc.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cs.shxzukj.cn

[E21] 超长截断加省略号
来源：http://sg.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qf.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jw.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xq.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rn.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rd.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://nf.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oo.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://we.huanxung.cn

[E22] 字节长度与字符长度
来源：http://pi.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ek.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ih.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lq.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vg.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oy.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yk.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://vt.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zw.newstarts.cn

================================================================================
来源：http://tv.lnxyls.cn

F. 文件与目录
来源：http://uv.hahajie.cn

================================================================================
来源：http://ss.hahajie.cn

[F01] 读取整个文件
来源：http://rw.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xp.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://qs.wgjwhj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zj.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://co.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jk.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ch.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://cu.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://ms.asd995.cn

[F02] 逐行读取文件
来源：http://in.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://da.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bw.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ih.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iw.muxihuayi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tw.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cn.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ai.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vj.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://te.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://at.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jp.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://je.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lx.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vk.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ez.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://lp.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mu.lnxyls.cn

[F04] 追加写入文件
来源：http://kt.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qr.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xh.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pa.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mi.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jx.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kk.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uz.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ui.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://ld.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hr.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://dz.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://lw.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://zv.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dc.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hy.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://bq.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://vo.huixinmuqiang.cn

[F06] 删除文件
来源：http://fo.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ni.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://bh.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xe.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dg.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lm.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://vl.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://xb.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://ta.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://uq.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wk.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://go.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yx.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wo.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zb.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hc.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://go.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ab.yuntaijiaju.cn

[F08] 遍历目录
来源：http://uc.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rv.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nw.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://ap.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://gm.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zy.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vd.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://bj.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://dg.muxihuayi.cn

[F09] 获取文件大小
来源：http://hh.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://bp.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://ek.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://oi.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://ar.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zy.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fl.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://ez.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://tp.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://yk.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rm.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://px.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qr.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://ly.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sv.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jt.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://on.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qi.asd995.cn

[F11] 复制与移动文件
来源：http://jv.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pg.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sr.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iz.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dx.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aa.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ln.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qj.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jv.yuexingan06.cn

[F12] CSV 读写
来源：http://eb.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://op.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lj.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ra.nicolike.cn

TS:   // 同上
来源：http://oi.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ld.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://el.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://at.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ic.jianghongdianzi.cn

================================================================================
来源：http://sq.yuexingan06.cn

G. 面向对象
来源：http://yj.shtwfgs.cn

================================================================================
来源：http://et.bjjhwx.cn

[G01] 定义类
来源：http://gy.colortex.cn

Py:   class User: pass
来源：http://ac.huanxung.cn

PHP:  class User {}
来源：http://kp.wgjwhj.cn

JS:   class User {}
来源：http://uc.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://dk.shxzukj.cn

Java: class User {}
来源：http://iz.huanxung.cn

Go:   type User struct { Name string }
来源：http://ay.hnjuh.cn

Ruby: class User; end
来源：http://oi.hnjuh.cn

C#:   class User {}
来源：http://zp.bookmarksfly.cn

[G02] 构造函数
来源：http://uj.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://dn.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://kj.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://sa.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://fb.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://as.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hp.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://lh.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://ld.yuntaijiaju.cn

[G03] 实例属性
来源：http://zy.wgjwhj.cn

Py:   self.name = "x"
来源：http://wp.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://lo.nicolike.cn

JS:   this.name = "x";
来源：http://dr.huanxung.cn

TS:   name: string = "x";
来源：http://lm.nszjky.cn

Java: private String name;
来源：http://sj.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wi.nicolike.cn

Ruby: @name = "x"
来源：http://zz.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://hb.chemitech.net.cn

[G04] 定义方法
来源：http://qg.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://fp.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zr.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://lg.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://nq.hahajie.cn

Java: String greet() { return name; }
来源：http://mv.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ur.lnxyls.cn

Ruby: def greet; @name; end
来源：http://iz.asd995.cn

C#:   public string Greet() => Name;
来源：http://fj.chemitech.net.cn

[G05] 继承
来源：http://xp.nicolike.cn

Py:   class Admin(User): pass
来源：http://pl.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://bb.shxzukj.cn

JS:   class Admin extends User {}
来源：http://oc.colortex.cn

TS:   class Admin extends User {}
来源：http://ts.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://oy.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bg.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://bq.shxzukj.cn

C#:   class Admin : User {}
来源：http://ay.wgjwhj.cn

[G06] 重写方法
来源：http://cu.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://mu.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oj.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://js.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://ep.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://ai.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cm.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://bm.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://oh.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://ur.9csxet.cn

Py:   super().greet()
来源：http://up.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://ar.asd995.cn

JS:   super.greet();
来源：http://lm.gzmigu.cn

TS:   super.greet();
来源：http://qb.yuexingan06.cn

Java: super.greet();
来源：http://ha.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mg.panjiajie.cn

Ruby: super
来源：http://na.bjjhwx.cn

C#:   base.Greet();
来源：http://rx.colortex.cn

[G08] 静态方法与属性
来源：http://bu.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lb.jianghongdianzi.cn


<!-- 参考信息 -->