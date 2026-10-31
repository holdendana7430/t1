代发 wailian999

Py:   for ch in s: print(ch)
来源：http://kr.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rw.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fa.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sl.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mz.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jz.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zr.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cl.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://lg.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qz.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://te.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dq.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tz.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tq.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ic.chemitech.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rr.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eu.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://pg.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lw.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rx.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pm.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://um.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ch.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://if.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pt.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ca.521024.cn

[E16] 数字千分位
来源：http://ex.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://hq.shxzukj.cn

PHP:  number_format(1234567);
来源：http://ss.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mx.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ez.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sj.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tv.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tw.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://te.szsharing.cn

[E17] 首字母大写
来源：http://sw.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ip.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pm.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hd.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hh.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://am.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kc.huixiangedu.cn

Ruby: s.capitalize
来源：http://vr.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ys.jctech888.com.cn

[E18] 模板占位符替换
来源：http://lt.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sd.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tx.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://te.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kb.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://td.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ub.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://im.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yv.jctech888.com.cn

[E19] 多行文本按行拆分
来源：http://by.shxzukj.cn

Py:   s.splitlines()
来源：http://xv.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://md.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://kr.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://zc.bookmarksfly.cn

Java: s.lines().toList()
来源：http://fe.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://lx.nicolike.cn

Ruby: s.lines
来源：http://jh.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://nl.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://gl.hnjuh.cn

Py:   if not s:
来源：http://pr.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kx.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fn.huixiangedu.cn

TS:   if (s === "") {}
来源：http://js.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://sb.huanxung.cn

Go:   if s == "" {}
来源：http://tg.newstarts.cn

Ruby: if s.empty?
来源：http://my.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cq.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://ls.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sz.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ca.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://df.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uu.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zr.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://pz.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wa.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jf.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://ni.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gg.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lm.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pj.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://na.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qv.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dd.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://dq.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ku.muxihuayi.cn

================================================================================
来源：http://pn.colortex.cn

F. 文件与目录
来源：http://mc.gzmigu.cn

================================================================================
来源：http://lk.asd995.cn

[F01] 读取整个文件
来源：http://md.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oz.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://ye.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lw.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mn.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://px.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qz.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://za.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://en.haigaiapp.cn

[F02] 逐行读取文件
来源：http://tb.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mm.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://er.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ea.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cw.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ox.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nu.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lk.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xm.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://nu.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pi.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ps.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://du.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rk.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gr.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zf.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://xr.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://le.asd995.cn

[F04] 追加写入文件
来源：http://nn.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ts.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vm.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cl.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ov.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lk.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pw.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bn.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ar.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://kn.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uc.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://tb.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://qb.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://wo.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mq.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tn.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ez.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://zm.chemitech.net.cn

[F06] 删除文件
来源：http://rr.9csxet.cn

Py:   os.remove("a.txt")
来源：http://pz.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://lq.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hx.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pv.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uh.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://ol.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://sn.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://nz.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://nv.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xl.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oq.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nf.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ye.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://th.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cm.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://os.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dk.jianghongdianzi.cn

[F08] 遍历目录
来源：http://ax.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xo.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rn.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://va.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://nn.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://te.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pz.huanxung.cn

Ruby: Dir.children("dir")
来源：http://jb.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://zn.9csxet.cn

[F09] 获取文件大小
来源：http://uf.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://rk.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://zd.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://ia.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://ke.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bv.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pa.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://we.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://su.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://cw.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://os.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mn.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nh.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ul.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xk.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://me.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://if.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ko.newstarts.cn

[F11] 复制与移动文件
来源：http://kp.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fb.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://er.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nt.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mc.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fy.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vr.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jh.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://js.muxihuayi.cn

[F12] CSV 读写
来源：http://og.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ac.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vu.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ou.szsharing.cn

TS:   // 同上
来源：http://lw.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ve.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ag.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jl.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yd.szxytkj.cn

================================================================================
来源：http://qp.chemitech.net.cn

G. 面向对象
来源：http://qv.9csxet.cn

================================================================================
来源：http://rl.szxytkj.cn

[G01] 定义类
来源：http://ml.yuntaijiaju.cn

Py:   class User: pass
来源：http://ed.newstarts.cn

PHP:  class User {}
来源：http://jg.shxzukj.cn

JS:   class User {}
来源：http://hf.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://ei.huanxung.cn

Java: class User {}
来源：http://sn.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://dh.chemitech.net.cn

Ruby: class User; end
来源：http://xz.chemitech.net.cn

C#:   class User {}
来源：http://bi.colortex.cn

[G02] 构造函数
来源：http://cy.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://xb.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://ou.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://qq.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://oj.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://wx.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sb.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://li.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://td.panjiajie.cn

[G03] 实例属性
来源：http://fk.521024.cn

Py:   self.name = "x"
来源：http://et.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://kb.yuexingan06.cn

JS:   this.name = "x";
来源：http://oa.szxytkj.cn

TS:   name: string = "x";
来源：http://kl.bjjhwx.cn

Java: private String name;
来源：http://kk.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ya.colortex.cn

Ruby: @name = "x"
来源：http://jb.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ba.panjiajie.cn

[G04] 定义方法
来源：http://jx.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://ej.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hs.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://gx.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://kb.521024.cn

Java: String greet() { return name; }
来源：http://wb.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ow.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://nh.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://hq.haigaiapp.cn

[G05] 继承
来源：http://jc.huanxung.cn

Py:   class Admin(User): pass
来源：http://lp.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://pe.huanxung.cn

JS:   class Admin extends User {}
来源：http://sk.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://hb.nicolike.cn

Java: class Admin extends User {}
来源：http://vh.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pn.gzmigu.cn

Ruby: class Admin < User; end
来源：http://qx.huanxung.cn

C#:   class Admin : User {}
来源：http://mz.yuntaijiaju.cn

[G06] 重写方法
来源：http://fe.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ep.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pp.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://ih.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://lg.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://en.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cm.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://qc.521024.cn

C#:   public override string Greet() => "admin";
来源：http://rp.jctech888.com.cn

[G07] 调用父类方法
来源：http://yq.yuntaijiaju.cn

Py:   super().greet()
来源：http://vi.shxzskj.cn

PHP:  parent::greet();
来源：http://yn.bjjhwx.cn

JS:   super.greet();
来源：http://yb.szsharing.cn

TS:   super.greet();
来源：http://zi.muxihuayi.cn

Java: super.greet();
来源：http://sd.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ky.chemitech.net.cn

Ruby: super
来源：http://jp.muxihuayi.cn

C#:   base.Greet();
来源：http://tf.newstarts.cn

[G08] 静态方法与属性
来源：http://gv.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oj.haigaiapp.cn

PHP:  public static function f() {}
来源：http://cl.nicolike.cn

JS:   static f() {}
来源：http://qw.szsharing.cn

TS:   static f(): void {}
来源：http://yj.muxihuayi.cn

Java: static void f() {}
来源：http://pl.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bt.lnxyls.cn

Ruby: def self.f; end
来源：http://oo.yuexingan06.cn

C#:   public static void F() {}
来源：http://qx.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://gz.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://tt.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qr.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yq.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://fi.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://jn.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://sl.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://en.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://ms.hnjuh.cn

[G10] 访问控制
来源：http://rg.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://fb.panjiajie.cn

PHP:  public / protected / private
来源：http://db.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://im.chemitech.net.cn

TS:   public / protected / private
来源：http://bn.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://qw.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xf.shxzukj.cn

Ruby: public / protected / private
来源：http://qt.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://aj.jctech888.com.cn

[G11] getter / setter
来源：http://ie.hahajie.cn

Py:   @property 与 @x.setter
来源：http://jx.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gk.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://pz.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://xa.szsharing.cn

Java: public String getName() { return name; }
来源：http://dx.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ta.shtwfgs.cn


<!-- 参考信息 -->