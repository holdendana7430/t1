代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xo.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wi.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://lb.szxytkj.cn

[E17] 首字母大写
来源：http://rq.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xf.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dk.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cm.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ee.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gm.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mb.wgjwhj.cn

Ruby: s.capitalize
来源：http://xr.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wk.muxihuayi.cn

[E18] 模板占位符替换
来源：http://nw.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mi.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://df.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mn.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://my.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ip.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ep.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lr.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xr.hahajie.cn

[E19] 多行文本按行拆分
来源：http://rp.yuexingan06.cn

Py:   s.splitlines()
来源：http://sa.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hg.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://ib.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://vi.lnxyls.cn

Java: s.lines().toList()
来源：http://se.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://bz.bjjhwx.cn

Ruby: s.lines
来源：http://um.shxzukj.cn

C#:   s.Split('\n')
来源：http://sv.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://cx.lnxyls.cn

Py:   if not s:
来源：http://rc.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vo.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cv.chemitech.net.cn

TS:   if (s === "") {}
来源：http://ug.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://uv.bookmarksfly.cn

Go:   if s == "" {}
来源：http://cg.jctech888.com.cn

Ruby: if s.empty?
来源：http://kz.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://so.hnjuh.cn

[E21] 超长截断加省略号
来源：http://yw.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qw.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://en.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rh.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cb.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://si.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://vq.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mb.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ai.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://sw.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hs.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nz.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gq.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wy.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pe.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ta.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://uh.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dw.colortex.cn

================================================================================
来源：http://ni.yuexingan06.cn

F. 文件与目录
来源：http://pk.wgjwhj.cn

================================================================================
来源：http://qd.panjiajie.cn

[F01] 读取整个文件
来源：http://us.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sn.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://sk.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fp.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bz.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vp.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fq.9csxet.cn

Ruby: File.read("a.txt")
来源：http://vd.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://pf.muxihuayi.cn

[F02] 逐行读取文件
来源：http://ev.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gt.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ax.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ls.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pv.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ph.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zs.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vv.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://en.asd995.cn

[F03] 写入文件（覆盖）
来源：http://sq.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dd.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qb.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nj.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pp.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yx.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xp.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://dg.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dd.szsharing.cn

[F04] 追加写入文件
来源：http://kq.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lf.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gz.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ae.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oa.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ay.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ia.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ye.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://ua.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bb.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://fk.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://gq.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://zh.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ps.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rf.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://rs.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://gj.jctech888.com.cn

[F06] 删除文件
来源：http://zh.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://mj.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://fp.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gq.jianghongdianzi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://db.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uf.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://zo.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://bk.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://rm.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ov.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://en.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ui.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pw.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ix.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jh.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gf.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tu.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kl.521024.cn

[F08] 遍历目录
来源：http://zt.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zd.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cx.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://vs.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://ym.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yb.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rw.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://dr.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://uj.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://ak.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://mq.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://ou.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://lv.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://wd.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kk.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://au.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://pb.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://rv.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://lp.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xl.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yl.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ld.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://ua.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oe.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qr.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ds.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gc.nszjky.cn

[F11] 复制与移动文件
来源：http://cg.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ci.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yl.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ob.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ks.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ji.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://du.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bm.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kk.shtwfgs.cn

[F12] CSV 读写
来源：http://az.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vs.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ar.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://un.szxytkj.cn

TS:   // 同上
来源：http://py.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gj.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yl.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gg.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tq.yuntaijiaju.cn

================================================================================
来源：http://uh.shtwfgs.cn

G. 面向对象
来源：http://iu.nicolike.cn

================================================================================
来源：http://mk.panjiajie.cn

[G01] 定义类
来源：http://tj.9csxet.cn

Py:   class User: pass
来源：http://nt.asd995.cn

PHP:  class User {}
来源：http://ta.asd995.cn

JS:   class User {}
来源：http://dv.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://fz.panjiajie.cn

Java: class User {}
来源：http://cs.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://aw.jctech888.com.cn

Ruby: class User; end
来源：http://td.nicolike.cn

C#:   class User {}
来源：http://gt.shtwfgs.cn

[G02] 构造函数
来源：http://zr.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://sv.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ek.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://bz.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://yn.521024.cn

Java: User(String name) { this.name = name; }
来源：http://lq.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xe.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://jl.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://ff.bookmarksfly.cn

[G03] 实例属性
来源：http://kv.colortex.cn

Py:   self.name = "x"
来源：http://iu.gzmigu.cn

PHP:  public string $name = "x";
来源：http://hs.colortex.cn

JS:   this.name = "x";
来源：http://ii.shxzskj.cn

TS:   name: string = "x";
来源：http://hg.szsharing.cn

Java: private String name;
来源：http://md.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bj.yuexingan06.cn

Ruby: @name = "x"
来源：http://mg.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://ri.yuntaijiaju.cn

[G04] 定义方法
来源：http://fr.colortex.cn

Py:   def greet(self): return self.name
来源：http://dd.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://co.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://hz.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://xw.haigaiapp.cn

Java: String greet() { return name; }
来源：http://fn.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://to.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://ky.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://rh.bjjhwx.cn

[G05] 继承
来源：http://np.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://rs.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://ij.nszjky.cn

JS:   class Admin extends User {}
来源：http://ey.hnjuh.cn

TS:   class Admin extends User {}
来源：http://fc.wgjwhj.cn

Java: class Admin extends User {}
来源：http://xu.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mq.panjiajie.cn

Ruby: class Admin < User; end
来源：http://my.newstarts.cn

C#:   class Admin : User {}
来源：http://wn.huixinmuqiang.cn

[G06] 重写方法
来源：http://gg.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://ve.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nb.asd995.cn

JS:   greet() { return "admin"; }
来源：http://be.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://nc.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://eh.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://to.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://ra.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://lt.huanxung.cn

[G07] 调用父类方法
来源：http://lv.hahajie.cn

Py:   super().greet()
来源：http://od.yuexingan06.cn

PHP:  parent::greet();
来源：http://yt.bjjhwx.cn

JS:   super.greet();
来源：http://fx.szxytkj.cn

TS:   super.greet();
来源：http://jm.521024.cn

Java: super.greet();
来源：http://zx.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kz.huixinmuqiang.cn

Ruby: super
来源：http://bn.yuexingan06.cn

C#:   base.Greet();
来源：http://ik.bjjhwx.cn

[G08] 静态方法与属性
来源：http://qr.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oh.jctech888.com.cn

PHP:  public static function f() {}
来源：http://jo.lnxyls.cn

JS:   static f() {}
来源：http://ux.9csxet.cn

TS:   static f(): void {}
来源：http://ui.hnjuh.cn

Java: static void f() {}
来源：http://nr.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vl.newstarts.cn

Ruby: def self.f; end
来源：http://yj.gzmigu.cn

C#:   public static void F() {}
来源：http://hz.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://uy.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://lp.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qf.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://of.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://vh.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://dn.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://ir.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tu.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://tf.yuntaijiaju.cn

[G10] 访问控制
来源：http://za.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://im.chemitech.net.cn

PHP:  public / protected / private
来源：http://ze.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://iz.lnxyls.cn

TS:   public / protected / private
来源：http://rw.521024.cn

Java: public / protected / private / 默认包级
来源：http://ru.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mh.szxytkj.cn

Ruby: public / protected / private
来源：http://dp.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://ui.nicolike.cn

[G11] getter / setter
来源：http://me.asd995.cn

Py:   @property 与 @x.setter
来源：http://bs.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://li.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://nd.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://ib.shxzukj.cn

Java: public String getName() { return name; }
来源：http://pv.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sl.hnjuh.cn

Ruby: attr_accessor :name
来源：http://cn.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://wa.hahajie.cn

[G12] 对象转字符串
来源：http://xp.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://nc.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jd.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://pg.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://wg.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://fz.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hc.nicolike.cn

Ruby: def to_s; @name; end
来源：http://yy.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://ym.shxzskj.cn

[G13] 判断对象类型
来源：http://up.9csxet.cn

Py:   isinstance(u, User)
来源：http://dz.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://gv.szxytkj.cn

JS:   u instanceof User
来源：http://zl.szsharing.cn

TS:   u instanceof User
来源：http://ii.bjjhwx.cn

Java: u instanceof User
来源：http://vq.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qk.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://ss.panjiajie.cn

C#:   u is User
来源：http://qt.panjiajie.cn

[G14] 数据类 / record
来源：http://uq.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tt.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://fz.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wa.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://je.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://wt.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://gf.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pm.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://lk.panjiajie.cn

[G15] 枚举
来源：http://eg.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qy.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pd.wgjwhj.cn


<!-- 参考信息 -->