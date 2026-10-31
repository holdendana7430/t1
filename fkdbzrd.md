代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fw.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rm.hnjuh.cn

[E16] 数字千分位
来源：http://uf.nicolike.cn

Py:   f"{1234567:,}"
来源：http://sr.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://nd.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wm.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qo.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ja.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ce.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bu.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://pm.hahajie.cn

[E17] 首字母大写
来源：http://it.shxzukj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gv.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qx.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gt.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zf.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mq.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mp.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://qm.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qg.wgjwhj.cn

[E18] 模板占位符替换
来源：http://mp.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yu.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fx.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jm.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uv.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bf.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nt.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qf.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kz.szsharing.cn

[E19] 多行文本按行拆分
来源：http://mo.yuexingan06.cn

Py:   s.splitlines()
来源：http://hx.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wx.chemitech.net.cn

JS:   s.split(/\r?\n/)
来源：http://ej.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://sb.newstarts.cn

Java: s.lines().toList()
来源：http://rx.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://oc.521024.cn

Ruby: s.lines
来源：http://wh.nicolike.cn

C#:   s.Split('\n')
来源：http://le.asd995.cn

[E20] 判断字符串是否为空
来源：http://pl.jctech888.com.cn

Py:   if not s:
来源：http://bz.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jn.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ev.asd995.cn

TS:   if (s === "") {}
来源：http://pe.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://kk.szxytkj.cn

Go:   if s == "" {}
来源：http://fy.wgjwhj.cn

Ruby: if s.empty?
来源：http://hd.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hv.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://ss.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fq.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zw.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ry.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cm.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nk.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://gq.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tq.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ir.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://tn.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ep.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pw.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wb.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pr.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tl.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://du.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://zn.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tt.szxytkj.cn

================================================================================
来源：http://cz.colortex.cn

F. 文件与目录
来源：http://vw.wgjwhj.cn

================================================================================
来源：http://vx.bookmarksfly.cn

[F01] 读取整个文件
来源：http://wh.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rk.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://ew.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gm.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uq.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xt.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://du.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://ht.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://kn.huixiangedu.cn

[F02] 逐行读取文件
来源：http://yx.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gu.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://on.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cg.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ar.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nu.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oa.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uy.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wz.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://pi.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wb.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tz.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tt.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fo.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fg.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gs.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://qq.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qc.szxytkj.cn

[F04] 追加写入文件
来源：http://cr.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://na.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qx.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fr.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pr.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lo.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kk.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oj.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lr.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://zr.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dd.asd995.cn

PHP:  file_exists("a.txt");
来源：http://qz.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://xi.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://cx.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xr.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://be.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://gd.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://mv.bookmarksfly.cn

[F06] 删除文件
来源：http://qo.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://ib.nicolike.cn

PHP:  unlink("a.txt");
来源：http://yn.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mr.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fu.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wh.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://gt.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://ho.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://uo.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://so.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ox.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ut.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dd.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kb.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sp.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yq.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rw.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nk.yuntaijiaju.cn

[F08] 遍历目录
来源：http://qn.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pw.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hm.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://hh.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://jg.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zu.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yb.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://af.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://zn.newstarts.cn

[F09] 获取文件大小
来源：http://vt.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://fv.nszjky.cn

PHP:  filesize("a.txt");
来源：http://cb.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://fg.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://bc.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ln.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mq.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://pw.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://up.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ss.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vg.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pc.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jp.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://lw.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gp.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fp.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://no.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jr.szsharing.cn

[F11] 复制与移动文件
来源：http://vj.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bo.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jp.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://il.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hq.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bw.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ux.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ag.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://df.huixinmuqiang.cn

[F12] CSV 读写
来源：http://to.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ft.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oh.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vb.hnjuh.cn

TS:   // 同上
来源：http://tu.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uz.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kh.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://id.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://et.9csxet.cn

================================================================================
来源：http://od.bjjhwx.cn

G. 面向对象
来源：http://za.gzmigu.cn

================================================================================
来源：http://av.nicolike.cn

[G01] 定义类
来源：http://la.muxihuayi.cn

Py:   class User: pass
来源：http://lt.shxzukj.cn

PHP:  class User {}
来源：http://uv.shxzukj.cn

JS:   class User {}
来源：http://xd.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://sd.bjjhwx.cn

Java: class User {}
来源：http://jy.asd995.cn

Go:   type User struct { Name string }
来源：http://ej.lnxyls.cn

Ruby: class User; end
来源：http://ms.lnxyls.cn

C#:   class User {}
来源：http://xi.szxytkj.cn

[G02] 构造函数
来源：http://qj.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://iw.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://tt.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://rl.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://ir.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://va.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yh.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://qw.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://gu.gzmigu.cn

[G03] 实例属性
来源：http://fv.panjiajie.cn

Py:   self.name = "x"
来源：http://ic.shxzukj.cn

PHP:  public string $name = "x";
来源：http://ex.huanxung.cn

JS:   this.name = "x";
来源：http://rm.wgjwhj.cn

TS:   name: string = "x";
来源：http://pm.huanxung.cn

Java: private String name;
来源：http://ub.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bu.chemitech.net.cn

Ruby: @name = "x"
来源：http://ev.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://oq.huixiangedu.cn

[G04] 定义方法
来源：http://dt.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://bb.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://aq.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://yz.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://ym.jctech888.com.cn

Java: String greet() { return name; }
来源：http://mp.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cy.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://wa.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://ty.colortex.cn

[G05] 继承
来源：http://nb.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://xh.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://mg.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://om.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://lm.chemitech.net.cn

Java: class Admin extends User {}
来源：http://sy.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ax.hahajie.cn

Ruby: class Admin < User; end
来源：http://xi.huanxung.cn

C#:   class Admin : User {}
来源：http://bt.shtwfgs.cn

[G06] 重写方法
来源：http://mx.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://zd.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eo.asd995.cn

JS:   greet() { return "admin"; }
来源：http://cn.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://yk.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://sg.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yc.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://sp.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://ky.hnjuh.cn

[G07] 调用父类方法
来源：http://hi.hnjuh.cn

Py:   super().greet()
来源：http://al.huanxung.cn

PHP:  parent::greet();
来源：http://im.shxzukj.cn

JS:   super.greet();
来源：http://yn.nszjky.cn

TS:   super.greet();
来源：http://rf.gzmigu.cn

Java: super.greet();
来源：http://iu.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ao.shxzukj.cn

Ruby: super
来源：http://rs.newstarts.cn

C#:   base.Greet();
来源：http://vk.yuexingan06.cn

[G08] 静态方法与属性
来源：http://xs.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ut.asd995.cn

PHP:  public static function f() {}
来源：http://dl.asd995.cn

JS:   static f() {}
来源：http://ql.panjiajie.cn

TS:   static f(): void {}
来源：http://af.shxzskj.cn

Java: static void f() {}
来源：http://ds.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jc.shxzukj.cn

Ruby: def self.f; end
来源：http://hi.jctech888.com.cn

C#:   public static void F() {}
来源：http://za.colortex.cn

[G09] 接口 / 抽象类
来源：http://lz.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://zo.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yl.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dp.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://ez.nszjky.cn

Java: interface Shape { double area(); }
来源：http://ox.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://eu.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tu.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://mn.panjiajie.cn

[G10] 访问控制
来源：http://hy.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ww.hahajie.cn

PHP:  public / protected / private
来源：http://iq.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://rs.gzmigu.cn

TS:   public / protected / private
来源：http://gp.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://is.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qd.wgjwhj.cn

Ruby: public / protected / private
来源：http://ja.hnjuh.cn

C#:   public / protected / private / internal
来源：http://cr.colortex.cn

[G11] getter / setter
来源：http://gr.huanxung.cn

Py:   @property 与 @x.setter
来源：http://op.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cv.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://mx.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://qn.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://lt.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jg.colortex.cn

Ruby: attr_accessor :name
来源：http://xp.huanxung.cn

C#:   public string Name { get; set; }
来源：http://jr.huanxung.cn

[G12] 对象转字符串
来源：http://np.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://bg.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ai.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://ps.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://ab.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://me.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eh.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://zf.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://rq.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://sb.panjiajie.cn

Py:   isinstance(u, User)
来源：http://ot.wgjwhj.cn

PHP:  $u instanceof User
来源：http://vk.haigaiapp.cn

JS:   u instanceof User
来源：http://en.bjjhwx.cn

TS:   u instanceof User
来源：http://jh.shxzukj.cn

Java: u instanceof User
来源：http://tm.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zh.huanxung.cn

Ruby: u.is_a?(User)
来源：http://di.newstarts.cn

C#:   u is User
来源：http://ix.nicolike.cn

[G14] 数据类 / record
来源：http://br.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lt.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://fn.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gf.hahajie.cn


<!-- 参考信息 -->