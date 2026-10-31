代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://nh.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://ps.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ke.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oi.muxihuayi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xq.nicolike.cn

[E11] 反转字符串
来源：http://jv.huixiangedu.cn

Py:   s[::-1]
来源：http://es.panjiajie.cn

PHP:  strrev($s);
来源：http://to.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://oq.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://yk.lnxyls.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pz.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://im.yuntaijiaju.cn

Ruby: s.reverse
来源：http://fn.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zv.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://vo.lnxyls.cn

Py:   s.count("a")
来源：http://rz.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://iv.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://jp.nszjky.cn

TS:   s.split("a").length - 1
来源：http://ip.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cn.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://xx.gzmigu.cn

Ruby: s.count("a")
来源：http://mg.muxihuayi.cn

C#:   s.Count(c => c == 'a')
来源：http://zi.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://ws.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://se.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qd.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iv.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cc.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xw.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://my.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dx.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mk.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://fk.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yg.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pg.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pl.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://or.asd995.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bc.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oz.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pd.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ef.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://be.muxihuayi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tu.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qj.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yn.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://eu.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cl.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dg.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oa.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ql.jianghongdianzi.cn

[E16] 数字千分位
来源：http://by.huanxung.cn

Py:   f"{1234567:,}"
来源：http://ar.newstarts.cn

PHP:  number_format(1234567);
来源：http://xk.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ea.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oy.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ct.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ci.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lh.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://ek.muxihuayi.cn

[E17] 首字母大写
来源：http://ys.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fq.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pj.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tt.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rq.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bw.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xd.hahajie.cn

Ruby: s.capitalize
来源：http://ej.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fs.colortex.cn

[E18] 模板占位符替换
来源：http://ep.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ev.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pq.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sm.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dg.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ip.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://km.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dq.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qj.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://jy.hnjuh.cn

Py:   s.splitlines()
来源：http://so.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ux.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://ej.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://ph.bookmarksfly.cn

Java: s.lines().toList()
来源：http://fm.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ru.jctech888.com.cn

Ruby: s.lines
来源：http://mx.shxzukj.cn

C#:   s.Split('\n')
来源：http://jz.asd995.cn

[E20] 判断字符串是否为空
来源：http://ad.hahajie.cn

Py:   if not s:
来源：http://yj.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kk.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vb.shxzukj.cn

TS:   if (s === "") {}
来源：http://dz.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://xs.shxzskj.cn

Go:   if s == "" {}
来源：http://uc.huixiangedu.cn

Ruby: if s.empty?
来源：http://hm.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wn.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://ub.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ny.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qg.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rb.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ob.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bn.bjjhwx.cn

Go:   // 按 rune 判断长度后截断
来源：http://up.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rz.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gv.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://jr.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sd.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wz.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ng.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cp.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wq.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vp.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://lm.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zk.wgjwhj.cn

================================================================================
来源：http://mo.asd995.cn

F. 文件与目录
来源：http://zg.shxzskj.cn

================================================================================
来源：http://cn.lnxyls.cn

[F01] 读取整个文件
来源：http://df.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kg.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://ju.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fp.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lt.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://we.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jr.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://xg.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://ln.muxihuayi.cn

[F02] 逐行读取文件
来源：http://ce.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ek.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vx.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pt.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cn.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://li.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ca.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://km.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tw.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://iq.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ez.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ae.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jn.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xq.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ic.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uj.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://uf.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qo.wgjwhj.cn

[F04] 追加写入文件
来源：http://lq.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rm.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ho.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xd.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mx.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://um.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jk.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wp.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fm.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://db.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vt.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://bw.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://qb.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://zk.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fg.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://am.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://wh.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://hf.jctech888.com.cn

[F06] 删除文件
来源：http://fw.hahajie.cn

Py:   os.remove("a.txt")
来源：http://yv.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://um.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qg.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xx.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ce.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://yd.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://tt.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://gu.9csxet.cn

[F07] 创建目录（含多级）
来源：http://eq.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ar.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://su.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lr.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pm.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nt.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cs.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nj.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://al.shxzskj.cn

[F08] 遍历目录
来源：http://jf.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gn.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ct.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://jc.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ej.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xx.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ne.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://dg.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://ds.colortex.cn

[F09] 获取文件大小
来源：http://zu.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://vu.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://fv.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://ty.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://jv.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ti.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://de.colortex.cn

Ruby: File.size("a.txt")
来源：http://ji.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://mt.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://pe.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kx.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bf.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ki.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://mo.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sy.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hl.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ph.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://th.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://yk.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ef.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xr.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://og.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hq.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sj.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ui.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rt.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iq.nicolike.cn

[F12] CSV 读写
来源：http://vx.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ld.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pc.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wh.bjjhwx.cn

TS:   // 同上
来源：http://ux.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ge.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dr.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bk.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sc.huixiangedu.cn

================================================================================
来源：http://ia.shxzukj.cn

G. 面向对象
来源：http://ff.nicolike.cn

================================================================================
来源：http://qj.newstarts.cn

[G01] 定义类
来源：http://pv.newstarts.cn

Py:   class User: pass
来源：http://qh.hahajie.cn

PHP:  class User {}
来源：http://jw.huixinmuqiang.cn

JS:   class User {}
来源：http://or.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://ag.hahajie.cn

Java: class User {}
来源：http://yk.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://uk.szsharing.cn

Ruby: class User; end
来源：http://uc.jianghongdianzi.cn

C#:   class User {}
来源：http://mz.yuntaijiaju.cn

[G02] 构造函数
来源：http://zl.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://rt.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://cl.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://as.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://pj.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://yt.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hg.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://kq.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://tw.bjjhwx.cn

[G03] 实例属性
来源：http://lu.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://rx.newstarts.cn

PHP:  public string $name = "x";
来源：http://vr.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://dd.huixiangedu.cn

TS:   name: string = "x";
来源：http://ul.nicolike.cn

Java: private String name;
来源：http://wg.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gy.wgjwhj.cn

Ruby: @name = "x"
来源：http://xb.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://te.shtwfgs.cn

[G04] 定义方法
来源：http://qw.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://sg.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ey.huanxung.cn

JS:   greet() { return this.name; }
来源：http://jw.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://eh.shxzskj.cn

Java: String greet() { return name; }
来源：http://hq.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xr.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://vc.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://fz.newstarts.cn

[G05] 继承
来源：http://fd.nszjky.cn

Py:   class Admin(User): pass
来源：http://rk.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://bs.hahajie.cn

JS:   class Admin extends User {}
来源：http://ld.shxzskj.cn

TS:   class Admin extends User {}
来源：http://ss.huanxung.cn

Java: class Admin extends User {}
来源：http://uk.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gn.szsharing.cn

Ruby: class Admin < User; end
来源：http://rn.shxzskj.cn

C#:   class Admin : User {}
来源：http://sz.huixinmuqiang.cn

[G06] 重写方法
来源：http://wm.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://gl.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://td.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://sa.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://eb.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://gq.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eq.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://of.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://ns.521024.cn

[G07] 调用父类方法
来源：http://gq.gzmigu.cn

Py:   super().greet()
来源：http://ct.shtwfgs.cn

PHP:  parent::greet();
来源：http://ho.jctech888.com.cn

JS:   super.greet();
来源：http://cz.jianghongdianzi.cn

TS:   super.greet();
来源：http://zb.bookmarksfly.cn

Java: super.greet();
来源：http://vq.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pp.lnxyls.cn

Ruby: super
来源：http://qp.hnjuh.cn

C#:   base.Greet();
来源：http://ff.shxzukj.cn

[G08] 静态方法与属性
来源：http://sl.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lp.shxzukj.cn

PHP:  public static function f() {}
来源：http://nh.huanxung.cn

JS:   static f() {}
来源：http://ld.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://ax.haigaiapp.cn

Java: static void f() {}
来源：http://op.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pr.panjiajie.cn

Ruby: def self.f; end
来源：http://mv.nicolike.cn

C#:   public static void F() {}
来源：http://ly.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://yp.panjiajie.cn


<!-- 参考信息 -->