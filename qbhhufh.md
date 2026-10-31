代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ph.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pg.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://of.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cx.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ah.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ab.bookmarksfly.cn

[E16] 数字千分位
来源：http://yp.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://sq.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://cl.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nq.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vc.shtwfgs.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ov.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vz.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://to.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://mz.nszjky.cn

[E17] 首字母大写
来源：http://xy.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ro.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ai.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zv.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oq.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ms.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kd.szsharing.cn

Ruby: s.capitalize
来源：http://tt.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vr.nszjky.cn

[E18] 模板占位符替换
来源：http://pm.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wn.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zt.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eu.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fe.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yi.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://si.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jh.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jk.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://dv.yuexingan06.cn

Py:   s.splitlines()
来源：http://vt.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ts.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://pk.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://fm.bjjhwx.cn

Java: s.lines().toList()
来源：http://pp.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://xz.hnjuh.cn

Ruby: s.lines
来源：http://fq.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://wx.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://yc.yuntaijiaju.cn

Py:   if not s:
来源：http://ei.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sz.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nl.haigaiapp.cn

TS:   if (s === "") {}
来源：http://no.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://by.panjiajie.cn

Go:   if s == "" {}
来源：http://am.yuexingan06.cn

Ruby: if s.empty?
来源：http://ug.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vo.9csxet.cn

[E21] 超长截断加省略号
来源：http://rl.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ns.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pg.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mu.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fs.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ae.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://sk.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://as.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://im.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://hl.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eo.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qv.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lg.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lq.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xt.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yg.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://ig.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ul.shxzukj.cn

================================================================================
来源：http://nh.panjiajie.cn

F. 文件与目录
来源：http://gt.jctech888.com.cn

================================================================================
来源：http://hu.panjiajie.cn

[F01] 读取整个文件
来源：http://kb.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sx.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://nq.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ys.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://th.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ig.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://le.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://oh.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://fo.colortex.cn

[F02] 逐行读取文件
来源：http://rn.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aj.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fb.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xm.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ge.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://da.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jz.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mk.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hu.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://qo.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pi.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oe.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gs.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vq.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hy.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cn.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://yy.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://al.asd995.cn

[F04] 追加写入文件
来源：http://cq.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qy.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://me.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://om.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ii.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ph.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ok.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aa.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tj.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://sv.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://va.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://el.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://ld.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://zy.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://by.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tw.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://zr.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://hx.wgjwhj.cn

[F06] 删除文件
来源：http://gl.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://fg.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://od.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gl.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wl.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://za.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://lt.asd995.cn

Ruby: File.delete("a.txt")
来源：http://xc.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://ta.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://un.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://he.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jo.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zr.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xv.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://em.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lt.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kg.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gi.nszjky.cn

[F08] 遍历目录
来源：http://nt.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nb.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ar.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://yq.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://qx.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://az.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nt.hahajie.cn

Ruby: Dir.children("dir")
来源：http://ju.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://vm.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://dx.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://ee.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://nx.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://ub.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://cd.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ww.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dy.9csxet.cn

Ruby: File.size("a.txt")
来源：http://wx.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://ry.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://hz.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qf.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ok.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ui.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://gf.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vw.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yl.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ed.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ft.shxzukj.cn

[F11] 复制与移动文件
来源：http://nu.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ex.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fn.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hc.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nq.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yv.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ni.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jp.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yv.szsharing.cn

[F12] CSV 读写
来源：http://md.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sl.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rt.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cz.colortex.cn

TS:   // 同上
来源：http://tr.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pw.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fz.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://il.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ew.shtwfgs.cn

================================================================================
来源：http://gj.yuexingan06.cn

G. 面向对象
来源：http://yc.chemitech.net.cn

================================================================================
来源：http://ei.wgjwhj.cn

[G01] 定义类
来源：http://ne.gzmigu.cn

Py:   class User: pass
来源：http://nw.jctech888.com.cn

PHP:  class User {}
来源：http://qt.bookmarksfly.cn

JS:   class User {}
来源：http://pu.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://oo.bjjhwx.cn

Java: class User {}
来源：http://ig.shxzukj.cn

Go:   type User struct { Name string }
来源：http://nm.panjiajie.cn

Ruby: class User; end
来源：http://ek.shxzukj.cn

C#:   class User {}
来源：http://iv.huixinmuqiang.cn

[G02] 构造函数
来源：http://md.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://tn.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://kd.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://ri.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://xn.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://xr.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ex.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://gd.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://vm.huixiangedu.cn

[G03] 实例属性
来源：http://bo.nszjky.cn

Py:   self.name = "x"
来源：http://no.shxzukj.cn

PHP:  public string $name = "x";
来源：http://hj.asd995.cn

JS:   this.name = "x";
来源：http://yw.jctech888.com.cn

TS:   name: string = "x";
来源：http://tl.szxytkj.cn

Java: private String name;
来源：http://jk.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jh.lnxyls.cn

Ruby: @name = "x"
来源：http://fl.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://rl.gzmigu.cn

[G04] 定义方法
来源：http://cn.szsharing.cn

Py:   def greet(self): return self.name
来源：http://ji.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mq.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://gw.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://wa.panjiajie.cn

Java: String greet() { return name; }
来源：http://cr.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vz.newstarts.cn

Ruby: def greet; @name; end
来源：http://gq.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://yj.chemitech.net.cn

[G05] 继承
来源：http://ey.asd995.cn

Py:   class Admin(User): pass
来源：http://pl.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://mk.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://mp.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://rr.bjjhwx.cn

Java: class Admin extends User {}
来源：http://ty.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sf.nicolike.cn

Ruby: class Admin < User; end
来源：http://ae.bjjhwx.cn

C#:   class Admin : User {}
来源：http://rw.jianghongdianzi.cn

[G06] 重写方法
来源：http://ij.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://xf.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vg.asd995.cn

JS:   greet() { return "admin"; }
来源：http://sv.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://gc.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://cn.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vl.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://uh.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://yu.asd995.cn

[G07] 调用父类方法
来源：http://jq.muxihuayi.cn

Py:   super().greet()
来源：http://ce.muxihuayi.cn

PHP:  parent::greet();
来源：http://np.szxytkj.cn

JS:   super.greet();
来源：http://vl.muxihuayi.cn

TS:   super.greet();
来源：http://to.huixiangedu.cn

Java: super.greet();
来源：http://zt.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tt.haigaiapp.cn

Ruby: super
来源：http://jw.colortex.cn

C#:   base.Greet();
来源：http://mq.521024.cn

[G08] 静态方法与属性
来源：http://le.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xa.newstarts.cn

PHP:  public static function f() {}
来源：http://ua.yuexingan06.cn

JS:   static f() {}
来源：http://tt.gzmigu.cn

TS:   static f(): void {}
来源：http://ro.huixiangedu.cn

Java: static void f() {}
来源：http://md.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qw.gzmigu.cn

Ruby: def self.f; end
来源：http://le.shxzukj.cn

C#:   public static void F() {}
来源：http://bq.huanxung.cn

[G09] 接口 / 抽象类
来源：http://dj.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://mn.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fo.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zt.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://tp.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://tb.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://ay.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nk.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://nn.lnxyls.cn

[G10] 访问控制
来源：http://dt.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://cx.nicolike.cn

PHP:  public / protected / private
来源：http://ut.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://it.chemitech.net.cn

TS:   public / protected / private
来源：http://qz.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://yn.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cm.nicolike.cn

Ruby: public / protected / private
来源：http://gj.nicolike.cn

C#:   public / protected / private / internal
来源：http://bf.newstarts.cn

[G11] getter / setter
来源：http://ds.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://qf.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hn.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://em.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://jd.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://ob.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xr.9csxet.cn

Ruby: attr_accessor :name
来源：http://fb.newstarts.cn

C#:   public string Name { get; set; }
来源：http://md.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://tq.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://bu.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ef.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://zj.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://di.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://tt.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pq.asd995.cn

Ruby: def to_s; @name; end
来源：http://kx.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://zg.colortex.cn

[G13] 判断对象类型
来源：http://pr.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://hl.nszjky.cn

PHP:  $u instanceof User
来源：http://sq.gzmigu.cn

JS:   u instanceof User
来源：http://wk.huixinmuqiang.cn

TS:   u instanceof User
来源：http://bi.lnxyls.cn

Java: u instanceof User
来源：http://mi.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mx.huanxung.cn

Ruby: u.is_a?(User)
来源：http://rp.lnxyls.cn

C#:   u is User
来源：http://xf.hahajie.cn


<!-- 参考信息 -->