代发 wailian999

Ruby: s.reverse
来源：http://bo.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bq.szsharing.cn

[E12] 统计某字符出现次数
来源：http://nb.muxihuayi.cn

Py:   s.count("a")
来源：http://yb.szxytkj.cn

PHP:  substr_count($s, "a");
来源：http://kg.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://xy.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://ul.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://os.521024.cn

Go:   strings.Count(s, "a")
来源：http://mf.newstarts.cn

Ruby: s.count("a")
来源：http://ze.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://wi.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ll.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://ep.shtwfgs.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hp.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ie.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ql.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wi.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uz.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rk.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mp.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://ye.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ir.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sy.yuntaijiaju.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vd.haigaiapp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mz.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sa.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wc.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zp.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ct.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://hy.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ip.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rh.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dh.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wq.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gx.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ph.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yw.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gu.hahajie.cn

[E16] 数字千分位
来源：http://ph.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://pp.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://eb.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vq.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hh.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qv.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tf.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fp.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://ye.nszjky.cn

[E17] 首字母大写
来源：http://wv.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bz.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ho.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wt.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://al.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://et.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ix.bookmarksfly.cn

Ruby: s.capitalize
来源：http://xm.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gl.szsharing.cn

[E18] 模板占位符替换
来源：http://rz.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kd.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wd.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://um.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bw.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mw.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ww.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zd.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mh.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://df.huixiangedu.cn

Py:   s.splitlines()
来源：http://vt.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yr.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://li.gzmigu.cn

TS:   s.split(/\r?\n/)
来源：http://kl.521024.cn

Java: s.lines().toList()
来源：http://wi.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://nv.nszjky.cn

Ruby: s.lines
来源：http://tv.muxihuayi.cn

C#:   s.Split('\n')
来源：http://gb.jctech888.com.cn

[E20] 判断字符串是否为空
来源：http://dz.wgjwhj.cn

Py:   if not s:
来源：http://dg.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kd.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://om.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://bn.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://gj.hnjuh.cn

Go:   if s == "" {}
来源：http://ua.9csxet.cn

Ruby: if s.empty?
来源：http://gq.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tw.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://ll.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ol.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yh.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sm.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iw.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pl.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://tb.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ai.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cg.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://bq.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cm.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rj.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ry.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wm.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pd.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xl.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://zn.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fs.muxihuayi.cn

================================================================================
来源：http://ig.521024.cn

F. 文件与目录
来源：http://si.chemitech.net.cn

================================================================================
来源：http://yr.bookmarksfly.cn

[F01] 读取整个文件
来源：http://dg.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cg.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://bf.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pw.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ld.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rc.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ib.huanxung.cn

Ruby: File.read("a.txt")
来源：http://hk.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://et.asd995.cn

[F02] 逐行读取文件
来源：http://kn.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wh.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kk.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lb.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xx.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yj.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ey.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sg.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xa.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://si.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cu.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cc.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ut.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xm.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jx.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oa.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://ku.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kj.asd995.cn

[F04] 追加写入文件
来源：http://ep.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dq.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kc.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://is.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wr.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zr.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oo.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wm.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lm.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://qk.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bh.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://st.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://tb.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://bs.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ee.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pq.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://nb.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://ei.asd995.cn

[F06] 删除文件
来源：http://nt.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://rl.9csxet.cn

PHP:  unlink("a.txt");
来源：http://nr.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ue.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wm.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bh.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://wq.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://ra.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://bm.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://pd.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://of.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wo.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eg.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tx.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qt.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zo.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qv.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ds.jianghongdianzi.cn

[F08] 遍历目录
来源：http://di.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://db.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zz.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://np.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://wx.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ng.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sl.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://ry.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://rb.hnjuh.cn

[F09] 获取文件大小
来源：http://hh.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://xi.asd995.cn

PHP:  filesize("a.txt");
来源：http://vu.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://jt.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://bh.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iz.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fu.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://ol.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://kc.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://aj.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nb.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ux.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bs.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://cm.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bx.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gh.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ep.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cm.9csxet.cn

[F11] 复制与移动文件
来源：http://nz.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wp.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ji.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gr.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gy.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ov.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hp.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ul.nicolike.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tu.szxytkj.cn

[F12] CSV 读写
来源：http://qx.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jz.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gl.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://im.chemitech.net.cn

TS:   // 同上
来源：http://mw.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vf.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://at.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xo.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yn.yuexingan06.cn

================================================================================
来源：http://jv.yuntaijiaju.cn

G. 面向对象
来源：http://rl.asd995.cn

================================================================================
来源：http://di.huanxung.cn

[G01] 定义类
来源：http://dz.bjjhwx.cn

Py:   class User: pass
来源：http://ik.chemitech.net.cn

PHP:  class User {}
来源：http://fo.yuexingan06.cn

JS:   class User {}
来源：http://gf.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://yg.shxzukj.cn

Java: class User {}
来源：http://wk.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://ej.huixinmuqiang.cn

Ruby: class User; end
来源：http://dm.panjiajie.cn

C#:   class User {}
来源：http://dw.wgjwhj.cn

[G02] 构造函数
来源：http://bm.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://qy.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://fc.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://cj.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://wi.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://vj.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hw.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://ug.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://cp.nszjky.cn

[G03] 实例属性
来源：http://qc.hnjuh.cn

Py:   self.name = "x"
来源：http://mn.shxzukj.cn

PHP:  public string $name = "x";
来源：http://yk.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://bp.hnjuh.cn

TS:   name: string = "x";
来源：http://eu.nszjky.cn

Java: private String name;
来源：http://vm.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wz.lnxyls.cn

Ruby: @name = "x"
来源：http://in.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://xo.newstarts.cn

[G04] 定义方法
来源：http://ww.nicolike.cn

Py:   def greet(self): return self.name
来源：http://lv.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ij.nicolike.cn

JS:   greet() { return this.name; }
来源：http://uu.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://cd.9csxet.cn

Java: String greet() { return name; }
来源：http://cx.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lu.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://np.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://xo.hnjuh.cn

[G05] 继承
来源：http://ql.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://sl.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://vy.asd995.cn

JS:   class Admin extends User {}
来源：http://ay.newstarts.cn

TS:   class Admin extends User {}
来源：http://gr.jctech888.com.cn

Java: class Admin extends User {}
来源：http://xd.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ke.hahajie.cn

Ruby: class Admin < User; end
来源：http://qw.huanxung.cn

C#:   class Admin : User {}
来源：http://xu.lnxyls.cn

[G06] 重写方法
来源：http://zo.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ox.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hh.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://lu.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://hx.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ef.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ki.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://zb.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://lc.haigaiapp.cn

[G07] 调用父类方法
来源：http://zl.colortex.cn

Py:   super().greet()
来源：http://bo.bjjhwx.cn

PHP:  parent::greet();
来源：http://rc.newstarts.cn

JS:   super.greet();
来源：http://jf.9csxet.cn

TS:   super.greet();
来源：http://sy.huanxung.cn

Java: super.greet();
来源：http://gt.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mp.asd995.cn

Ruby: super
来源：http://tz.yuntaijiaju.cn

C#:   base.Greet();
来源：http://yk.gzmigu.cn

[G08] 静态方法与属性
来源：http://pk.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zw.haigaiapp.cn

PHP:  public static function f() {}
来源：http://az.yuexingan06.cn

JS:   static f() {}
来源：http://ig.szsharing.cn

TS:   static f(): void {}
来源：http://gj.huixiangedu.cn

Java: static void f() {}
来源：http://cd.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://df.bookmarksfly.cn

Ruby: def self.f; end
来源：http://rn.bjjhwx.cn

C#:   public static void F() {}
来源：http://fk.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://gn.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://gh.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://up.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xk.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://va.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://eq.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://zp.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ry.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://kr.chemitech.net.cn

[G10] 访问控制
来源：http://rd.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://pb.szxytkj.cn

PHP:  public / protected / private
来源：http://bs.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://sc.haigaiapp.cn


<!-- 参考信息 -->