代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mg.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://hd.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nf.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fu.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ra.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hf.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bj.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eo.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vn.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zi.huanxung.cn

[E16] 数字千分位
来源：http://lb.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://iv.gzmigu.cn

PHP:  number_format(1234567);
来源：http://ue.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://db.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xs.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ln.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mv.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aa.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://bo.jianghongdianzi.cn

[E17] 首字母大写
来源：http://ls.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sb.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hv.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mq.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://he.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ia.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hi.colortex.cn

Ruby: s.capitalize
来源：http://pd.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eu.wgjwhj.cn

[E18] 模板占位符替换
来源：http://aq.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yh.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fg.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kk.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lb.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jt.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rw.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mh.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wi.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://tk.panjiajie.cn

Py:   s.splitlines()
来源：http://mr.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sl.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://zp.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://nu.lnxyls.cn

Java: s.lines().toList()
来源：http://in.521024.cn

Go:   strings.Split(s, "\n")
来源：http://sb.hahajie.cn

Ruby: s.lines
来源：http://nv.asd995.cn

C#:   s.Split('\n')
来源：http://xv.nicolike.cn

[E20] 判断字符串是否为空
来源：http://dm.shxzukj.cn

Py:   if not s:
来源：http://ul.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ti.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xx.asd995.cn

TS:   if (s === "") {}
来源：http://au.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://au.hnjuh.cn

Go:   if s == "" {}
来源：http://ji.lnxyls.cn

Ruby: if s.empty?
来源：http://bi.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yy.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://ay.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mt.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wj.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kk.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dr.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ag.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://bu.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vn.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xw.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://yj.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lt.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ti.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://li.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yq.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hw.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wx.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://rr.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fu.huixinmuqiang.cn

================================================================================
来源：http://yr.szxytkj.cn

F. 文件与目录
来源：http://qy.shtwfgs.cn

================================================================================
来源：http://ix.shxzukj.cn

[F01] 读取整个文件
来源：http://pv.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xp.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://xg.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qf.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jj.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vq.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ik.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://za.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://pe.muxihuayi.cn

[F02] 逐行读取文件
来源：http://ot.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sy.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lu.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pt.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oi.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bc.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wu.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wp.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zg.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://jy.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vv.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://do.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://je.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rf.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ri.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dp.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://en.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mg.szxytkj.cn

[F04] 追加写入文件
来源：http://by.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xh.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lg.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uk.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ev.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cs.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vq.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ee.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zm.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://wy.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tb.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://dk.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://va.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://wz.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vq.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ye.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://na.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://iz.huixinmuqiang.cn

[F06] 删除文件
来源：http://hg.asd995.cn

Py:   os.remove("a.txt")
来源：http://ij.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://zc.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lq.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uo.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hu.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://ga.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://fc.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://lr.9csxet.cn

[F07] 创建目录（含多级）
来源：http://xo.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xp.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ho.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://co.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ta.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ez.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jh.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zw.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xr.huixinmuqiang.cn

[F08] 遍历目录
来源：http://zv.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ib.9csxet.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zn.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://or.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://it.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ay.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xf.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://zn.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://jt.asd995.cn

[F09] 获取文件大小
来源：http://hv.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://ig.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://tw.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://db.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://kq.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ls.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://db.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://lo.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://sm.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://jc.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://va.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://si.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vd.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://ni.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ll.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rw.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yd.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vc.nicolike.cn

[F11] 复制与移动文件
来源：http://di.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://us.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ci.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ti.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jt.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xr.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fo.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fo.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xt.hahajie.cn

[F12] CSV 读写
来源：http://gt.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kr.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fn.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zm.haigaiapp.cn

TS:   // 同上
来源：http://uw.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://or.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zx.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ft.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zv.jctech888.com.cn

================================================================================
来源：http://yq.huixinmuqiang.cn

G. 面向对象
来源：http://gi.colortex.cn

================================================================================
来源：http://mx.shxzskj.cn

[G01] 定义类
来源：http://ig.hnjuh.cn

Py:   class User: pass
来源：http://ns.9csxet.cn

PHP:  class User {}
来源：http://ws.shxzskj.cn

JS:   class User {}
来源：http://hw.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://vm.asd995.cn

Java: class User {}
来源：http://ml.gzmigu.cn

Go:   type User struct { Name string }
来源：http://dd.hnjuh.cn

Ruby: class User; end
来源：http://uw.wgjwhj.cn

C#:   class User {}
来源：http://kw.shxzskj.cn

[G02] 构造函数
来源：http://ss.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://ei.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://ba.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://ne.asd995.cn

TS:   constructor(public name: string) {}
来源：http://eg.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://qo.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sw.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://gn.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://tu.bjjhwx.cn

[G03] 实例属性
来源：http://yk.szsharing.cn

Py:   self.name = "x"
来源：http://qf.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://kq.nicolike.cn

JS:   this.name = "x";
来源：http://xn.panjiajie.cn

TS:   name: string = "x";
来源：http://el.huixinmuqiang.cn

Java: private String name;
来源：http://qv.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zq.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://ep.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://yz.shtwfgs.cn

[G04] 定义方法
来源：http://ql.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://xg.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ij.nicolike.cn

JS:   greet() { return this.name; }
来源：http://zl.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://bp.hahajie.cn

Java: String greet() { return name; }
来源：http://ey.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qy.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://zt.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://up.jianghongdianzi.cn

[G05] 继承
来源：http://va.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://fr.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://jj.szxytkj.cn

JS:   class Admin extends User {}
来源：http://tk.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://xv.gzmigu.cn

Java: class Admin extends User {}
来源：http://pp.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sh.colortex.cn

Ruby: class Admin < User; end
来源：http://bn.chemitech.net.cn

C#:   class Admin : User {}
来源：http://tn.muxihuayi.cn

[G06] 重写方法
来源：http://eq.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://lv.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ol.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://nc.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://ph.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://vn.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://di.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://ku.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://wv.bookmarksfly.cn

[G07] 调用父类方法
来源：http://ag.muxihuayi.cn

Py:   super().greet()
来源：http://st.521024.cn

PHP:  parent::greet();
来源：http://vz.panjiajie.cn

JS:   super.greet();
来源：http://sg.newstarts.cn

TS:   super.greet();
来源：http://qe.jianghongdianzi.cn

Java: super.greet();
来源：http://ko.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jz.jianghongdianzi.cn

Ruby: super
来源：http://pb.9csxet.cn

C#:   base.Greet();
来源：http://fz.gzmigu.cn

[G08] 静态方法与属性
来源：http://tw.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wc.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://ev.lnxyls.cn

JS:   static f() {}
来源：http://ox.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://fn.9csxet.cn

Java: static void f() {}
来源：http://vz.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yu.panjiajie.cn

Ruby: def self.f; end
来源：http://tg.huanxung.cn

C#:   public static void F() {}
来源：http://bo.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://qk.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://om.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://se.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xx.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://rr.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://np.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://kl.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sf.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://vu.shxzskj.cn

[G10] 访问控制
来源：http://ju.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://xl.521024.cn

PHP:  public / protected / private
来源：http://rw.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://wx.shxzskj.cn

TS:   public / protected / private
来源：http://cp.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://kh.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://on.muxihuayi.cn

Ruby: public / protected / private
来源：http://vy.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://uy.bjjhwx.cn

[G11] getter / setter
来源：http://vy.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://qc.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aj.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://zb.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ac.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://yc.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://br.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://ld.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://rc.nicolike.cn

[G12] 对象转字符串
来源：http://ul.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://wa.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yu.colortex.cn

JS:   toString() { return this.name; }
来源：http://ap.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://zi.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://lm.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rh.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://qg.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://xa.muxihuayi.cn

[G13] 判断对象类型
来源：http://oq.panjiajie.cn

Py:   isinstance(u, User)
来源：http://uf.panjiajie.cn

PHP:  $u instanceof User
来源：http://cf.huanxung.cn

JS:   u instanceof User
来源：http://xj.shxzskj.cn

TS:   u instanceof User
来源：http://ux.bjjhwx.cn


<!-- 参考信息 -->