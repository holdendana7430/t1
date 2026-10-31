代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://gp.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://ow.newstarts.cn

Java: s.lines().toList()
来源：http://sc.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://fx.hnjuh.cn

Ruby: s.lines
来源：http://mc.panjiajie.cn

C#:   s.Split('\n')
来源：http://li.huanxung.cn

[E20] 判断字符串是否为空
来源：http://rm.jctech888.com.cn

Py:   if not s:
来源：http://us.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://st.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jr.panjiajie.cn

TS:   if (s === "") {}
来源：http://pr.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://le.colortex.cn

Go:   if s == "" {}
来源：http://nj.yuexingan06.cn

Ruby: if s.empty?
来源：http://qw.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ay.gzmigu.cn

[E21] 超长截断加省略号
来源：http://po.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jr.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cy.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sn.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qc.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kz.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://gp.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yv.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qi.nicolike.cn

[E22] 字节长度与字符长度
来源：http://ej.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xb.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://au.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gb.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kb.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wa.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xo.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://bv.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oo.haigaiapp.cn

================================================================================
来源：http://hn.yuntaijiaju.cn

F. 文件与目录
来源：http://rn.huixiangedu.cn

================================================================================
来源：http://pg.szsharing.cn

[F01] 读取整个文件
来源：http://ro.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pl.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://xx.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wi.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://js.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wf.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hb.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://fb.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://qd.colortex.cn

[F02] 逐行读取文件
来源：http://jk.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xz.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://we.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qe.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ki.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sp.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lk.nszjky.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nv.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xm.asd995.cn

[F03] 写入文件（覆盖）
来源：http://yj.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vq.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bk.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uc.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sm.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wf.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://la.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://hu.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ym.wgjwhj.cn

[F04] 追加写入文件
来源：http://if.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://md.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bs.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lk.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zv.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kh.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zr.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ug.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lr.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://go.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://os.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://zu.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://jq.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://hh.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vd.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yc.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://wf.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://zr.huanxung.cn

[F06] 删除文件
来源：http://vo.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://eg.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://wc.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zb.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ov.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lc.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://oh.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://ob.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://vm.hahajie.cn

[F07] 创建目录（含多级）
来源：http://hb.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fu.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://le.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dr.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xy.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fe.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rq.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lq.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zx.9csxet.cn

[F08] 遍历目录
来源：http://zy.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yo.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vy.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://ds.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://np.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qc.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wy.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://xc.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://ig.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://bq.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://dt.colortex.cn

PHP:  filesize("a.txt");
来源：http://uo.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://rk.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://vs.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://au.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pq.colortex.cn

Ruby: File.size("a.txt")
来源：http://ve.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://bn.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ge.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ky.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jo.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mi.9csxet.cn

TS:   path.extname("a.txt")
来源：http://qk.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bl.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bv.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ba.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qt.shxzukj.cn

[F11] 复制与移动文件
来源：http://we.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bk.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cr.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aq.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vx.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://du.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ob.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://to.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://om.szsharing.cn

[F12] CSV 读写
来源：http://as.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rr.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ap.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ln.yuntaijiaju.cn

TS:   // 同上
来源：http://os.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mu.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eh.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ab.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dm.newstarts.cn

================================================================================
来源：http://cb.haigaiapp.cn

G. 面向对象
来源：http://xe.huixinmuqiang.cn

================================================================================
来源：http://yk.muxihuayi.cn

[G01] 定义类
来源：http://jj.huixinmuqiang.cn

Py:   class User: pass
来源：http://if.bookmarksfly.cn

PHP:  class User {}
来源：http://ip.nszjky.cn

JS:   class User {}
来源：http://ky.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://pt.newstarts.cn

Java: class User {}
来源：http://an.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://ok.shxzukj.cn

Ruby: class User; end
来源：http://bz.bookmarksfly.cn

C#:   class User {}
来源：http://cz.jianghongdianzi.cn

[G02] 构造函数
来源：http://kq.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://zc.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://uy.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://yr.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://dc.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://jw.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yp.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://qr.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://gd.panjiajie.cn

[G03] 实例属性
来源：http://qi.huixiangedu.cn

Py:   self.name = "x"
来源：http://ca.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://dm.haigaiapp.cn

JS:   this.name = "x";
来源：http://bd.yuexingan06.cn

TS:   name: string = "x";
来源：http://ip.hnjuh.cn

Java: private String name;
来源：http://xz.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tx.gzmigu.cn

Ruby: @name = "x"
来源：http://ef.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://fl.521024.cn

[G04] 定义方法
来源：http://si.hahajie.cn

Py:   def greet(self): return self.name
来源：http://vj.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ld.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://li.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://ih.huanxung.cn

Java: String greet() { return name; }
来源：http://rv.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zm.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://ly.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://zz.nicolike.cn

[G05] 继承
来源：http://bf.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://sx.nszjky.cn

PHP:  class Admin extends User {}
来源：http://ha.asd995.cn

JS:   class Admin extends User {}
来源：http://ql.newstarts.cn

TS:   class Admin extends User {}
来源：http://ni.muxihuayi.cn

Java: class Admin extends User {}
来源：http://ip.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://he.nicolike.cn

Ruby: class Admin < User; end
来源：http://mt.panjiajie.cn

C#:   class Admin : User {}
来源：http://cy.colortex.cn

[G06] 重写方法
来源：http://et.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://vm.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fx.asd995.cn

JS:   greet() { return "admin"; }
来源：http://at.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://da.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://ef.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xb.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://ah.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://mi.jctech888.com.cn

[G07] 调用父类方法
来源：http://qu.chemitech.net.cn

Py:   super().greet()
来源：http://mz.gzmigu.cn

PHP:  parent::greet();
来源：http://ev.szxytkj.cn

JS:   super.greet();
来源：http://jr.panjiajie.cn

TS:   super.greet();
来源：http://hp.gzmigu.cn

Java: super.greet();
来源：http://pd.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qy.huixiangedu.cn

Ruby: super
来源：http://ly.hnjuh.cn

C#:   base.Greet();
来源：http://qa.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://pz.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ev.huixiangedu.cn

PHP:  public static function f() {}
来源：http://vi.szxytkj.cn

JS:   static f() {}
来源：http://uf.szxytkj.cn

TS:   static f(): void {}
来源：http://ms.huanxung.cn

Java: static void f() {}
来源：http://dv.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zo.nszjky.cn

Ruby: def self.f; end
来源：http://ma.haigaiapp.cn

C#:   public static void F() {}
来源：http://ed.colortex.cn

[G09] 接口 / 抽象类
来源：http://ts.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://nf.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nl.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://av.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://cw.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://so.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://up.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jr.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ld.newstarts.cn

[G10] 访问控制
来源：http://vb.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://vf.9csxet.cn

PHP:  public / protected / private
来源：http://ca.colortex.cn

JS:   #private 字段；其余公开
来源：http://rp.chemitech.net.cn

TS:   public / protected / private
来源：http://mk.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://yb.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sa.szxytkj.cn

Ruby: public / protected / private
来源：http://mt.huanxung.cn

C#:   public / protected / private / internal
来源：http://wt.wgjwhj.cn

[G11] getter / setter
来源：http://dz.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://mq.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fp.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://hx.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://mp.9csxet.cn

Java: public String getName() { return name; }
来源：http://fq.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pb.shxzukj.cn

Ruby: attr_accessor :name
来源：http://vo.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://xi.shxzskj.cn

[G12] 对象转字符串
来源：http://rz.colortex.cn

Py:   def __str__(self): return self.name
来源：http://ty.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lr.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://zh.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://dg.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://sf.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://el.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://ut.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://tx.gzmigu.cn

[G13] 判断对象类型
来源：http://ch.huanxung.cn

Py:   isinstance(u, User)
来源：http://li.huanxung.cn

PHP:  $u instanceof User
来源：http://ek.hahajie.cn

JS:   u instanceof User
来源：http://vz.jianghongdianzi.cn

TS:   u instanceof User
来源：http://kf.szsharing.cn

Java: u instanceof User
来源：http://aa.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lg.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://ui.muxihuayi.cn

C#:   u is User
来源：http://at.bjjhwx.cn

[G14] 数据类 / record
来源：http://jg.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lj.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://fc.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gq.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://mq.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://yb.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://qw.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mp.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://zd.lnxyls.cn

[G15] 枚举
来源：http://ex.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kn.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hu.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qa.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gt.521024.cn

Java: enum Color { RED, GREEN }
来源：http://ev.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nz.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://ma.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vf.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://ey.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pd.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://or.newstarts.cn

JS:   Object.entries(obj)
来源：http://no.nicolike.cn

TS:   Object.entries(obj)
来源：http://ec.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kj.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vt.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://wy.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://ie.jctech888.com.cn

================================================================================
来源：http://kr.bjjhwx.cn

H. 异常与错误处理
来源：http://la.newstarts.cn

================================================================================
来源：http://mj.hnjuh.cn

[H01] try / catch 基础
来源：http://gw.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://av.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kw.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bv.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ko.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fo.haigaiapp.cn


<!-- 参考信息 -->