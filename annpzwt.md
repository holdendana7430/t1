代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fh.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lw.yuexingan06.cn

[E16] 数字千分位
来源：http://nt.521024.cn

Py:   f"{1234567:,}"
来源：http://hc.colortex.cn

PHP:  number_format(1234567);
来源：http://ni.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ir.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jg.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://or.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yq.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://da.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://ej.bjjhwx.cn

[E17] 首字母大写
来源：http://om.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mp.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ig.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bq.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yb.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ne.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hs.hnjuh.cn

Ruby: s.capitalize
来源：http://df.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ws.wgjwhj.cn

[E18] 模板占位符替换
来源：http://jn.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wi.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nn.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gv.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zt.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ab.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jb.521024.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zh.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lb.521024.cn

[E19] 多行文本按行拆分
来源：http://bg.shxzskj.cn

Py:   s.splitlines()
来源：http://uw.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qd.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://yo.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://ph.asd995.cn

Java: s.lines().toList()
来源：http://na.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://vq.hnjuh.cn

Ruby: s.lines
来源：http://ci.muxihuayi.cn

C#:   s.Split('\n')
来源：http://wo.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://jk.szsharing.cn

Py:   if not s:
来源：http://bl.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fo.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qx.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://xf.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://ex.haigaiapp.cn

Go:   if s == "" {}
来源：http://st.shxzskj.cn

Ruby: if s.empty?
来源：http://ar.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://eu.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bs.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sm.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wm.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hl.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aq.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://jm.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jb.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hf.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://ui.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yh.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qq.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sq.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pg.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lm.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tn.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://nj.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eu.bookmarksfly.cn

================================================================================
来源：http://qx.jctech888.com.cn

F. 文件与目录
来源：http://ah.chemitech.net.cn

================================================================================
来源：http://bg.haigaiapp.cn

[F01] 读取整个文件
来源：http://hp.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qw.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://yj.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fy.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zm.hahajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ei.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kt.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://os.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://zq.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://ed.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ep.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://io.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wy.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://up.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pz.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iz.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lt.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://en.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://js.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lv.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pp.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pt.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://od.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yc.wgjwhj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ua.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://ok.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ts.gzmigu.cn

[F04] 追加写入文件
来源：http://kq.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xp.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ro.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mg.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rm.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nd.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rp.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ca.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tm.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://st.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ij.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://dy.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://bv.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://iv.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tj.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vr.521024.cn

Ruby: File.exist?("a.txt")
来源：http://kq.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://mk.szsharing.cn

[F06] 删除文件
来源：http://wp.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://ll.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://pf.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fk.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nq.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sg.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://fa.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://yn.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://yp.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://zg.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vu.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ck.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aa.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sy.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tz.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qw.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hl.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oy.newstarts.cn

[F08] 遍历目录
来源：http://tz.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mj.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dx.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://oi.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://wj.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yj.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qa.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://sk.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://bd.lnxyls.cn

[F09] 获取文件大小
来源：http://va.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://sx.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://ri.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://ul.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://mz.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rj.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uz.hahajie.cn

Ruby: File.size("a.txt")
来源：http://jo.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://tr.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://cz.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uo.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sb.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jt.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://sd.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rp.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pp.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ph.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://we.bjjhwx.cn

[F11] 复制与移动文件
来源：http://yu.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hm.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uw.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eg.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vj.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jv.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zs.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ee.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qg.yuntaijiaju.cn

[F12] CSV 读写
来源：http://lg.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wu.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ln.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fm.lnxyls.cn

TS:   // 同上
来源：http://mu.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vv.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dy.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nz.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gg.wgjwhj.cn

================================================================================
来源：http://dp.jctech888.com.cn

G. 面向对象
来源：http://dl.newstarts.cn

================================================================================
来源：http://qr.yuntaijiaju.cn

[G01] 定义类
来源：http://rd.jianghongdianzi.cn

Py:   class User: pass
来源：http://we.hnjuh.cn

PHP:  class User {}
来源：http://em.muxihuayi.cn

JS:   class User {}
来源：http://wm.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://sh.hahajie.cn

Java: class User {}
来源：http://sp.asd995.cn

Go:   type User struct { Name string }
来源：http://zj.shxzskj.cn

Ruby: class User; end
来源：http://ej.jianghongdianzi.cn

C#:   class User {}
来源：http://zh.chemitech.net.cn

[G02] 构造函数
来源：http://zw.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ky.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://hd.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://up.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://ff.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://zz.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ls.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://ov.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://ek.jianghongdianzi.cn

[G03] 实例属性
来源：http://he.yuexingan06.cn

Py:   self.name = "x"
来源：http://pa.asd995.cn

PHP:  public string $name = "x";
来源：http://ma.lnxyls.cn

JS:   this.name = "x";
来源：http://ks.shxzukj.cn

TS:   name: string = "x";
来源：http://kk.bookmarksfly.cn

Java: private String name;
来源：http://rv.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gp.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://gr.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://wb.nszjky.cn

[G04] 定义方法
来源：http://ku.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://kf.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hf.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://vr.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://oj.yuexingan06.cn

Java: String greet() { return name; }
来源：http://yl.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vf.colortex.cn

Ruby: def greet; @name; end
来源：http://vf.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://yz.bjjhwx.cn

[G05] 继承
来源：http://ib.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://dg.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://xm.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://bm.gzmigu.cn

TS:   class Admin extends User {}
来源：http://fg.szxytkj.cn

Java: class Admin extends User {}
来源：http://it.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bb.hnjuh.cn

Ruby: class Admin < User; end
来源：http://wt.shtwfgs.cn

C#:   class Admin : User {}
来源：http://wv.lnxyls.cn

[G06] 重写方法
来源：http://ac.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://mn.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ag.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://lq.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://ci.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://fp.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ym.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://jq.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ek.hahajie.cn

[G07] 调用父类方法
来源：http://ba.colortex.cn

Py:   super().greet()
来源：http://ey.huanxung.cn

PHP:  parent::greet();
来源：http://kl.yuexingan06.cn

JS:   super.greet();
来源：http://sf.hnjuh.cn

TS:   super.greet();
来源：http://db.yuexingan06.cn

Java: super.greet();
来源：http://ov.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ge.bookmarksfly.cn

Ruby: super
来源：http://bc.521024.cn

C#:   base.Greet();
来源：http://rr.colortex.cn

[G08] 静态方法与属性
来源：http://mx.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zu.chemitech.net.cn

PHP:  public static function f() {}
来源：http://gi.shxzskj.cn

JS:   static f() {}
来源：http://qv.muxihuayi.cn

TS:   static f(): void {}
来源：http://cw.521024.cn

Java: static void f() {}
来源：http://bc.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ov.wgjwhj.cn

Ruby: def self.f; end
来源：http://jm.nszjky.cn

C#:   public static void F() {}
来源：http://yo.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://hf.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://ym.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qy.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xc.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://uh.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://pm.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ve.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hv.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://uc.wgjwhj.cn

[G10] 访问控制
来源：http://gs.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://of.szxytkj.cn

PHP:  public / protected / private
来源：http://kw.colortex.cn

JS:   #private 字段；其余公开
来源：http://sy.wgjwhj.cn

TS:   public / protected / private
来源：http://iv.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://vk.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gz.huixiangedu.cn

Ruby: public / protected / private
来源：http://dg.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://sc.shtwfgs.cn

[G11] getter / setter
来源：http://bd.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://om.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tx.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://hc.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://ki.shxzukj.cn

Java: public String getName() { return name; }
来源：http://lh.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cs.hnjuh.cn

Ruby: attr_accessor :name
来源：http://wu.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://jh.nszjky.cn

[G12] 对象转字符串
来源：http://zz.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://hm.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ov.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://yq.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://be.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://sh.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wk.nicolike.cn

Ruby: def to_s; @name; end
来源：http://bb.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://uc.shxzskj.cn

[G13] 判断对象类型
来源：http://vx.nicolike.cn

Py:   isinstance(u, User)
来源：http://jz.lnxyls.cn

PHP:  $u instanceof User
来源：http://oi.shxzskj.cn

JS:   u instanceof User
来源：http://nh.haigaiapp.cn

TS:   u instanceof User
来源：http://yg.lnxyls.cn

Java: u instanceof User
来源：http://nw.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://is.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://ad.nicolike.cn

C#:   u is User
来源：http://qw.szsharing.cn

[G14] 数据类 / record
来源：http://gx.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sg.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://io.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://md.huanxung.cn


<!-- 参考信息 -->