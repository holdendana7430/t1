代发 wailian999

Go:   if s == "" {}
来源：http://fe.wgjwhj.cn

Ruby: if s.empty?
来源：http://xm.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vu.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://nd.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nu.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://to.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yj.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ww.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uu.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://ga.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kg.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kj.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://jk.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ud.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xy.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://go.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vh.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cj.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://za.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://qv.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jm.muxihuayi.cn

================================================================================
来源：http://zt.huanxung.cn

F. 文件与目录
来源：http://zn.haigaiapp.cn

================================================================================
来源：http://vt.hnjuh.cn

[F01] 读取整个文件
来源：http://fd.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hy.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://tu.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yj.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sc.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yv.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jh.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://nu.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://ry.yuexingan06.cn

[F02] 逐行读取文件
来源：http://in.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ok.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dt.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fm.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ff.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cv.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ks.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jj.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jx.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://tb.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hd.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mr.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kc.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vu.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://di.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://te.nicolike.cn

Ruby: File.write("a.txt", "hi")
来源：http://hy.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qn.colortex.cn

[F04] 追加写入文件
来源：http://br.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qe.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hb.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nw.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hr.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mw.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gp.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://is.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xe.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://ox.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ey.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://lh.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://ka.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://fl.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sy.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wl.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://bw.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://rg.yuntaijiaju.cn

[F06] 删除文件
来源：http://tc.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://eo.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://zx.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cf.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rp.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qb.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://kc.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://jj.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://or.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://mg.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jc.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nl.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wg.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ru.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ey.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bp.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uj.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://op.huixiangedu.cn

[F08] 遍历目录
来源：http://vi.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gd.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tj.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://xb.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://jf.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ur.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fp.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://ov.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://vd.colortex.cn

[F09] 获取文件大小
来源：http://cb.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://ze.nszjky.cn

PHP:  filesize("a.txt");
来源：http://lx.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://gw.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://kl.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dn.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fb.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://xh.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://cw.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://pb.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wx.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ni.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eu.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://je.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ff.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oo.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vr.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wz.haigaiapp.cn

[F11] 复制与移动文件
来源：http://bz.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://of.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dz.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qw.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hx.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ir.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mk.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lw.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zi.shxzukj.cn

[F12] CSV 读写
来源：http://ya.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gm.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://br.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cd.yuntaijiaju.cn

TS:   // 同上
来源：http://nf.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ss.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hi.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ah.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ma.gzmigu.cn

================================================================================
来源：http://vy.yuexingan06.cn

G. 面向对象
来源：http://fg.yuexingan06.cn

================================================================================
来源：http://ae.yuexingan06.cn

[G01] 定义类
来源：http://cr.panjiajie.cn

Py:   class User: pass
来源：http://zq.panjiajie.cn

PHP:  class User {}
来源：http://di.hnjuh.cn

JS:   class User {}
来源：http://qy.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://li.panjiajie.cn

Java: class User {}
来源：http://ri.9csxet.cn

Go:   type User struct { Name string }
来源：http://aq.chemitech.net.cn

Ruby: class User; end
来源：http://qy.colortex.cn

C#:   class User {}
来源：http://xc.szxytkj.cn

[G02] 构造函数
来源：http://se.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://au.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://ls.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://la.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://rf.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://wl.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uu.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://lj.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ti.yuntaijiaju.cn

[G03] 实例属性
来源：http://lo.jctech888.com.cn

Py:   self.name = "x"
来源：http://il.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://vh.nicolike.cn

JS:   this.name = "x";
来源：http://ft.shxzskj.cn

TS:   name: string = "x";
来源：http://ak.shxzukj.cn

Java: private String name;
来源：http://ys.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wl.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://ay.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://hu.huixiangedu.cn

[G04] 定义方法
来源：http://bi.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://mp.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://up.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://mj.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://qy.szxytkj.cn

Java: String greet() { return name; }
来源：http://vm.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sn.521024.cn

Ruby: def greet; @name; end
来源：http://aj.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://tm.huanxung.cn

[G05] 继承
来源：http://sv.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ua.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://hh.gzmigu.cn

JS:   class Admin extends User {}
来源：http://fz.521024.cn

TS:   class Admin extends User {}
来源：http://iq.szxytkj.cn

Java: class Admin extends User {}
来源：http://ad.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zv.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://ak.chemitech.net.cn

C#:   class Admin : User {}
来源：http://dz.huixiangedu.cn

[G06] 重写方法
来源：http://uk.521024.cn

Py:   def greet(self): return "admin"
来源：http://me.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ar.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://sk.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://sh.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://oh.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vp.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://ib.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://pn.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://dt.shxzskj.cn

Py:   super().greet()
来源：http://km.hnjuh.cn

PHP:  parent::greet();
来源：http://ba.szxytkj.cn

JS:   super.greet();
来源：http://qx.hahajie.cn

TS:   super.greet();
来源：http://jv.shxzskj.cn

Java: super.greet();
来源：http://sy.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zw.colortex.cn

Ruby: super
来源：http://qz.hahajie.cn

C#:   base.Greet();
来源：http://xq.haigaiapp.cn

[G08] 静态方法与属性
来源：http://cd.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lc.nszjky.cn

PHP:  public static function f() {}
来源：http://vn.hahajie.cn

JS:   static f() {}
来源：http://tv.shxzukj.cn

TS:   static f(): void {}
来源：http://sa.lnxyls.cn

Java: static void f() {}
来源：http://ud.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kw.szsharing.cn

Ruby: def self.f; end
来源：http://bn.hnjuh.cn

C#:   public static void F() {}
来源：http://ne.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://tl.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://zk.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vy.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cw.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://jw.asd995.cn

Java: interface Shape { double area(); }
来源：http://xa.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ua.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uv.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://hm.huanxung.cn

[G10] 访问控制
来源：http://yt.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://tg.shxzukj.cn

PHP:  public / protected / private
来源：http://tq.colortex.cn

JS:   #private 字段；其余公开
来源：http://os.nszjky.cn

TS:   public / protected / private
来源：http://xx.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://il.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gu.gzmigu.cn

Ruby: public / protected / private
来源：http://jb.newstarts.cn

C#:   public / protected / private / internal
来源：http://av.chemitech.net.cn

[G11] getter / setter
来源：http://pl.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://it.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pt.colortex.cn

JS:   get name() { return this._name; }
来源：http://vb.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://yg.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://ql.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://re.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://xl.nszjky.cn

C#:   public string Name { get; set; }
来源：http://dc.huixiangedu.cn

[G12] 对象转字符串
来源：http://hy.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://xz.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tr.hahajie.cn

JS:   toString() { return this.name; }
来源：http://tl.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://ei.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://pj.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fm.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://gm.521024.cn

C#:   public override string ToString() => Name;
来源：http://ar.huanxung.cn

[G13] 判断对象类型
来源：http://vi.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://di.9csxet.cn

PHP:  $u instanceof User
来源：http://st.haigaiapp.cn

JS:   u instanceof User
来源：http://yx.muxihuayi.cn

TS:   u instanceof User
来源：http://zp.haigaiapp.cn

Java: u instanceof User
来源：http://as.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ed.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://th.jianghongdianzi.cn

C#:   u is User
来源：http://wn.huanxung.cn

[G14] 数据类 / record
来源：http://ms.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xm.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://lk.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ug.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://fi.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://go.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://wz.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rq.asd995.cn

C#:   record User(string Name, int Age);
来源：http://no.hnjuh.cn

[G15] 枚举
来源：http://dw.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bt.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://er.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ic.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cq.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://jv.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pz.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://pw.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gt.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://gk.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yb.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://ho.newstarts.cn

JS:   Object.entries(obj)
来源：http://oy.szxytkj.cn

TS:   Object.entries(obj)
来源：http://bg.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qz.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ry.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://lp.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://le.hnjuh.cn

================================================================================
来源：http://wu.huixinmuqiang.cn

H. 异常与错误处理
来源：http://be.szxytkj.cn

================================================================================
来源：http://er.wgjwhj.cn

[H01] try / catch 基础
来源：http://wc.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xz.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gl.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jg.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xz.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jx.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://op.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gh.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oh.huanxung.cn

[H02] finally / ensure 收尾
来源：http://ug.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nc.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ka.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://un.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eo.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bn.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rf.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kv.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lo.chemitech.net.cn


<!-- 参考信息 -->