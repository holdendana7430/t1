代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://io.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wp.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lz.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wa.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qw.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ts.chemitech.net.cn

Ruby: s.capitalize
来源：http://fr.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dc.jctech888.com.cn

[E18] 模板占位符替换
来源：http://bv.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yq.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lw.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sa.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jk.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ra.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hy.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xs.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zj.colortex.cn

[E19] 多行文本按行拆分
来源：http://uv.521024.cn

Py:   s.splitlines()
来源：http://dm.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yp.521024.cn

JS:   s.split(/\r?\n/)
来源：http://tz.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://wq.huanxung.cn

Java: s.lines().toList()
来源：http://zv.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://dr.szsharing.cn

Ruby: s.lines
来源：http://gg.lnxyls.cn

C#:   s.Split('\n')
来源：http://mz.9csxet.cn

[E20] 判断字符串是否为空
来源：http://kz.hahajie.cn

Py:   if not s:
来源：http://bn.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nt.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nz.hahajie.cn

TS:   if (s === "") {}
来源：http://fz.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://il.yuexingan06.cn

Go:   if s == "" {}
来源：http://tc.nszjky.cn

Ruby: if s.empty?
来源：http://qm.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cx.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://lr.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://be.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gn.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fb.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tt.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://au.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://qc.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yb.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wd.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://eo.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cw.panjiajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ez.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://na.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hl.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ig.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lk.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://gj.shxzskj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nh.chemitech.net.cn

================================================================================
来源：http://na.newstarts.cn

F. 文件与目录
来源：http://du.gzmigu.cn

================================================================================
来源：http://fb.jctech888.com.cn

[F01] 读取整个文件
来源：http://ci.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ze.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://no.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yc.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hs.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zr.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fo.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://qx.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://cu.szsharing.cn

[F02] 逐行读取文件
来源：http://az.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zl.huixiangedu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yc.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rt.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ks.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ge.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lb.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qb.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nv.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://sm.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sz.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kt.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lv.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dj.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dw.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mk.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://mg.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://py.wgjwhj.cn

[F04] 追加写入文件
来源：http://dl.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bd.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hu.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fn.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uo.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fo.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oz.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://go.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://ac.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cl.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://jo.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://hj.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://ic.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rj.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gx.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://bo.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://oh.wgjwhj.cn

[F06] 删除文件
来源：http://uy.hahajie.cn

Py:   os.remove("a.txt")
来源：http://td.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://my.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ox.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nn.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gh.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://di.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://zv.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://eg.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://ng.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sp.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lt.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tw.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gp.szxytkj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vq.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rf.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tt.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yv.huixiangedu.cn

[F08] 遍历目录
来源：http://lu.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dn.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xp.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://xx.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://if.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wi.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sb.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://kr.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://xw.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://fh.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://pg.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://dm.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://kt.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://mb.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cx.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://et.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://tp.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://hm.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://ao.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ox.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kv.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pt.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://tf.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ru.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ey.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jd.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jr.hahajie.cn

[F11] 复制与移动文件
来源：http://oa.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xi.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xp.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jf.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fz.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kb.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qy.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bi.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xt.huixiangedu.cn

[F12] CSV 读写
来源：http://zd.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wg.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tx.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://st.shxzskj.cn

TS:   // 同上
来源：http://pi.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pk.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wh.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bn.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sq.hnjuh.cn

================================================================================
来源：http://fx.chemitech.net.cn

G. 面向对象
来源：http://ys.jianghongdianzi.cn

================================================================================
来源：http://ki.huixiangedu.cn

[G01] 定义类
来源：http://ct.hnjuh.cn

Py:   class User: pass
来源：http://om.haigaiapp.cn

PHP:  class User {}
来源：http://yr.szsharing.cn

JS:   class User {}
来源：http://uo.colortex.cn

TS:   class User { name: string = ""; }
来源：http://bo.chemitech.net.cn

Java: class User {}
来源：http://yc.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://el.nszjky.cn

Ruby: class User; end
来源：http://yy.bjjhwx.cn

C#:   class User {}
来源：http://tt.huanxung.cn

[G02] 构造函数
来源：http://dx.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://vq.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://au.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://ay.521024.cn

TS:   constructor(public name: string) {}
来源：http://mz.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://hl.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ci.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://md.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://yy.nszjky.cn

[G03] 实例属性
来源：http://uf.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://fd.shxzskj.cn

PHP:  public string $name = "x";
来源：http://zk.shxzukj.cn

JS:   this.name = "x";
来源：http://fa.chemitech.net.cn

TS:   name: string = "x";
来源：http://qp.wgjwhj.cn

Java: private String name;
来源：http://oz.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xt.szxytkj.cn

Ruby: @name = "x"
来源：http://je.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://xs.yuexingan06.cn

[G04] 定义方法
来源：http://ga.521024.cn

Py:   def greet(self): return self.name
来源：http://qa.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ar.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://rc.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://rv.asd995.cn

Java: String greet() { return name; }
来源：http://kp.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dh.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://yc.9csxet.cn

C#:   public string Greet() => Name;
来源：http://vf.shxzskj.cn

[G05] 继承
来源：http://bl.hnjuh.cn

Py:   class Admin(User): pass
来源：http://jp.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://ee.521024.cn

JS:   class Admin extends User {}
来源：http://iw.asd995.cn

TS:   class Admin extends User {}
来源：http://vj.szxytkj.cn

Java: class Admin extends User {}
来源：http://uu.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xt.nszjky.cn

Ruby: class Admin < User; end
来源：http://kh.huanxung.cn

C#:   class Admin : User {}
来源：http://oe.shtwfgs.cn

[G06] 重写方法
来源：http://ak.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://ta.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tw.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://js.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://fh.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://wk.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ns.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://il.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://lv.shtwfgs.cn

[G07] 调用父类方法
来源：http://ld.nicolike.cn

Py:   super().greet()
来源：http://io.chemitech.net.cn

PHP:  parent::greet();
来源：http://jf.szxytkj.cn

JS:   super.greet();
来源：http://ci.jianghongdianzi.cn

TS:   super.greet();
来源：http://zl.jianghongdianzi.cn

Java: super.greet();
来源：http://ay.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qs.shxzskj.cn

Ruby: super
来源：http://lh.jianghongdianzi.cn

C#:   base.Greet();
来源：http://qf.yuexingan06.cn

[G08] 静态方法与属性
来源：http://wi.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://go.muxihuayi.cn

PHP:  public static function f() {}
来源：http://ht.hnjuh.cn

JS:   static f() {}
来源：http://ry.shtwfgs.cn

TS:   static f(): void {}
来源：http://dm.hahajie.cn

Java: static void f() {}
来源：http://pb.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tv.lnxyls.cn

Ruby: def self.f; end
来源：http://pl.shtwfgs.cn

C#:   public static void F() {}
来源：http://qh.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://gw.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://fh.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sb.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ns.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://yk.9csxet.cn

Java: interface Shape { double area(); }
来源：http://zq.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://pj.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pn.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://mr.szsharing.cn

[G10] 访问控制
来源：http://ur.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://qe.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://xg.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://ke.9csxet.cn

TS:   public / protected / private
来源：http://ax.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://ei.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lk.yuexingan06.cn

Ruby: public / protected / private
来源：http://qz.shxzskj.cn

C#:   public / protected / private / internal
来源：http://ap.hahajie.cn

[G11] getter / setter
来源：http://rx.hahajie.cn

Py:   @property 与 @x.setter
来源：http://fc.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uq.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://fj.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://cx.shxzukj.cn

Java: public String getName() { return name; }
来源：http://bk.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cv.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://nw.nszjky.cn

C#:   public string Name { get; set; }
来源：http://sf.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://re.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://aj.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dm.newstarts.cn

JS:   toString() { return this.name; }
来源：http://mn.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://ip.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://yf.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vm.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://qr.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://na.bookmarksfly.cn

[G13] 判断对象类型
来源：http://yb.521024.cn

Py:   isinstance(u, User)
来源：http://ba.shxzskj.cn

PHP:  $u instanceof User
来源：http://hc.shtwfgs.cn

JS:   u instanceof User
来源：http://kt.jctech888.com.cn

TS:   u instanceof User
来源：http://ge.asd995.cn

Java: u instanceof User
来源：http://ji.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cu.nicolike.cn

Ruby: u.is_a?(User)
来源：http://fo.colortex.cn

C#:   u is User
来源：http://zr.chemitech.net.cn

[G14] 数据类 / record
来源：http://qz.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://px.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://mf.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zx.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://rb.colortex.cn

Java: record User(String name, int age) {}
来源：http://xk.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://lh.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://co.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://vm.shtwfgs.cn

[G15] 枚举
来源：http://gd.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rx.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zp.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bz.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nn.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://lj.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://go.521024.cn


<!-- 参考信息 -->