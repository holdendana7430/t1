代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wa.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cy.colortex.cn

[E16] 数字千分位
来源：http://xh.nicolike.cn

Py:   f"{1234567:,}"
来源：http://ju.gzmigu.cn

PHP:  number_format(1234567);
来源：http://za.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vh.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lc.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bs.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mk.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zm.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://uu.9csxet.cn

[E17] 首字母大写
来源：http://li.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dh.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aw.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lf.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wb.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xl.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sd.nicolike.cn

Ruby: s.capitalize
来源：http://ph.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ee.nicolike.cn

[E18] 模板占位符替换
来源：http://uv.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xr.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cv.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ul.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bo.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lx.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ar.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hf.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://it.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://dz.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ed.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lw.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://kq.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://hw.huanxung.cn

Java: s.lines().toList()
来源：http://xa.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://qu.huixiangedu.cn

Ruby: s.lines
来源：http://ea.lnxyls.cn

C#:   s.Split('\n')
来源：http://rx.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://id.lnxyls.cn

Py:   if not s:
来源：http://mn.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qo.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fg.yuexingan06.cn

TS:   if (s === "") {}
来源：http://df.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://ey.newstarts.cn

Go:   if s == "" {}
来源：http://rl.panjiajie.cn

Ruby: if s.empty?
来源：http://np.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jk.521024.cn

[E21] 超长截断加省略号
来源：http://tn.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://om.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fk.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://co.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uj.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qz.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://nn.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gw.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tl.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://ys.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kg.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qv.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cd.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bs.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ei.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dp.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://mk.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wb.yuntaijiaju.cn

================================================================================
来源：http://oo.hnjuh.cn

F. 文件与目录
来源：http://dn.nicolike.cn

================================================================================
来源：http://ds.huixiangedu.cn

[F01] 读取整个文件
来源：http://vb.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gw.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://ex.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bu.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rf.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zn.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uw.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://sf.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://my.9csxet.cn

[F02] 逐行读取文件
来源：http://ei.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fj.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yk.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hg.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ju.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ca.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zr.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bh.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gx.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://kh.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mm.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zl.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yu.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rx.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uc.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nl.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://qg.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nz.asd995.cn

[F04] 追加写入文件
来源：http://lm.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ce.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xq.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vg.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ek.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iw.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ci.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ak.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pr.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://qs.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jj.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://zq.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://df.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://jj.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ip.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://va.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://vq.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://tl.muxihuayi.cn

[F06] 删除文件
来源：http://np.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://mw.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://tn.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zy.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sm.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yq.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://qk.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://xi.521024.cn

C#:   File.Delete("a.txt");
来源：http://gc.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://cp.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vc.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ua.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://se.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jb.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gq.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qs.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sr.muxihuayi.cn

[F08] 遍历目录
来源：http://xa.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ky.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://db.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://tj.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://nf.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fv.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ug.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://bx.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://fh.muxihuayi.cn

[F09] 获取文件大小
来源：http://il.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://qy.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://wp.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://nt.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://dy.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xf.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gw.nszjky.cn

Ruby: File.size("a.txt")
来源：http://lt.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ic.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://tt.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wr.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tk.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dr.newstarts.cn

TS:   path.extname("a.txt")
来源：http://ay.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ej.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qm.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wd.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sp.haigaiapp.cn

[F11] 复制与移动文件
来源：http://oc.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jo.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iv.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://si.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://er.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zd.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wq.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vp.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sc.shxzskj.cn

[F12] CSV 读写
来源：http://bs.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qd.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jo.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://py.shtwfgs.cn

TS:   // 同上
来源：http://ex.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wi.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hd.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rv.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vf.521024.cn

================================================================================
来源：http://oi.shtwfgs.cn

G. 面向对象
来源：http://nn.bjjhwx.cn

================================================================================
来源：http://or.gzmigu.cn

[G01] 定义类
来源：http://hx.newstarts.cn

Py:   class User: pass
来源：http://nl.shxzukj.cn

PHP:  class User {}
来源：http://fk.haigaiapp.cn

JS:   class User {}
来源：http://md.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://do.jianghongdianzi.cn

Java: class User {}
来源：http://td.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://ko.colortex.cn

Ruby: class User; end
来源：http://xj.521024.cn

C#:   class User {}
来源：http://pm.gzmigu.cn

[G02] 构造函数
来源：http://yk.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://ex.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://qt.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://jr.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ng.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://td.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cc.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://ce.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ra.asd995.cn

[G03] 实例属性
来源：http://cm.szsharing.cn

Py:   self.name = "x"
来源：http://aj.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://er.nicolike.cn

JS:   this.name = "x";
来源：http://ya.muxihuayi.cn

TS:   name: string = "x";
来源：http://cu.nicolike.cn

Java: private String name;
来源：http://hp.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://py.muxihuayi.cn

Ruby: @name = "x"
来源：http://bw.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://fp.jianghongdianzi.cn

[G04] 定义方法
来源：http://ow.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://mr.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gq.nszjky.cn

JS:   greet() { return this.name; }
来源：http://yz.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://yy.nicolike.cn

Java: String greet() { return name; }
来源：http://as.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hq.hahajie.cn

Ruby: def greet; @name; end
来源：http://nd.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://qr.huixinmuqiang.cn

[G05] 继承
来源：http://cw.nicolike.cn

Py:   class Admin(User): pass
来源：http://xz.huanxung.cn

PHP:  class Admin extends User {}
来源：http://mf.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://yl.colortex.cn

TS:   class Admin extends User {}
来源：http://yh.wgjwhj.cn

Java: class Admin extends User {}
来源：http://hd.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hs.9csxet.cn

Ruby: class Admin < User; end
来源：http://pv.yuexingan06.cn

C#:   class Admin : User {}
来源：http://kh.lnxyls.cn

[G06] 重写方法
来源：http://ht.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://zr.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://te.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://ul.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://ah.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://oi.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ri.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://vz.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://pq.9csxet.cn

[G07] 调用父类方法
来源：http://dk.jianghongdianzi.cn

Py:   super().greet()
来源：http://xt.szxytkj.cn

PHP:  parent::greet();
来源：http://tv.nszjky.cn

JS:   super.greet();
来源：http://uv.shtwfgs.cn

TS:   super.greet();
来源：http://at.szxytkj.cn

Java: super.greet();
来源：http://oy.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ll.shxzukj.cn

Ruby: super
来源：http://go.yuntaijiaju.cn

C#:   base.Greet();
来源：http://cf.yuexingan06.cn

[G08] 静态方法与属性
来源：http://vp.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lb.nszjky.cn

PHP:  public static function f() {}
来源：http://tv.9csxet.cn

JS:   static f() {}
来源：http://oa.yuexingan06.cn

TS:   static f(): void {}
来源：http://ns.hnjuh.cn

Java: static void f() {}
来源：http://ez.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fc.yuexingan06.cn

Ruby: def self.f; end
来源：http://il.huixiangedu.cn

C#:   public static void F() {}
来源：http://uo.szsharing.cn

[G09] 接口 / 抽象类
来源：http://ou.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://qp.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jk.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pc.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://rm.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://ap.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://mz.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ip.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://je.bjjhwx.cn

[G10] 访问控制
来源：http://jw.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://gs.jctech888.com.cn

PHP:  public / protected / private
来源：http://nd.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://iq.yuntaijiaju.cn

TS:   public / protected / private
来源：http://qx.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://jl.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://px.yuexingan06.cn

Ruby: public / protected / private
来源：http://lr.newstarts.cn

C#:   public / protected / private / internal
来源：http://we.nszjky.cn

[G11] getter / setter
来源：http://al.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://ms.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://au.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://ih.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://qy.nszjky.cn

Java: public String getName() { return name; }
来源：http://jn.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zb.gzmigu.cn

Ruby: attr_accessor :name
来源：http://sr.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://ae.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://xd.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://ui.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://me.huanxung.cn

JS:   toString() { return this.name; }
来源：http://nv.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://xe.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://nn.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dv.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://ws.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://fm.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://ff.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://rq.panjiajie.cn

PHP:  $u instanceof User
来源：http://yd.jctech888.com.cn

JS:   u instanceof User
来源：http://ur.huanxung.cn

TS:   u instanceof User
来源：http://uc.hnjuh.cn

Java: u instanceof User
来源：http://bt.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wr.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://it.shxzukj.cn

C#:   u is User
来源：http://fk.nszjky.cn

[G14] 数据类 / record
来源：http://vt.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fr.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://bg.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kv.huixinmuqiang.cn


<!-- 参考信息 -->