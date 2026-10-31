代发 wailian999

Go:   if s == "" {}
来源：http://cr.newstarts.cn

Ruby: if s.empty?
来源：http://sa.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ft.gzmigu.cn

[E21] 超长截断加省略号
来源：http://lx.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sg.wgjwhj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://od.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hv.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bm.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ax.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://qt.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fm.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://od.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ja.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lk.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vd.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ff.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xl.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xb.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://db.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uu.shxzskj.cn

================================================================================
来源：http://cj.shxzukj.cn

F. 文件与目录
来源：http://tz.nszjky.cn

================================================================================
来源：http://ms.colortex.cn

[F01] 读取整个文件
来源：http://vv.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yv.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://tp.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ek.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pt.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tz.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rh.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://zj.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://mn.colortex.cn

[F02] 逐行读取文件
来源：http://vv.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dw.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://en.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nw.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dt.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cf.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ay.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://no.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://el.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://ug.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xd.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bw.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zh.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nw.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xg.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jc.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://yu.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sn.bookmarksfly.cn

[F04] 追加写入文件
来源：http://yl.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://br.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://by.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oa.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yl.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bw.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ie.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yd.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mc.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://ei.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ag.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://ji.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://ps.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://kk.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kl.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uj.nicolike.cn

Ruby: File.exist?("a.txt")
来源：http://fb.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://cm.9csxet.cn

[F06] 删除文件
来源：http://sf.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://jz.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://mg.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cr.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rq.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://go.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://mz.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://dx.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://vg.newstarts.cn

[F07] 创建目录（含多级）
来源：http://ca.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nn.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cb.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ef.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tm.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://st.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dp.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qc.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pn.yuntaijiaju.cn

[F08] 遍历目录
来源：http://gi.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zw.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vf.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://lf.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://ml.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wk.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cx.newstarts.cn

Ruby: Dir.children("dir")
来源：http://yt.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://xk.gzmigu.cn

[F09] 获取文件大小
来源：http://ha.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://wv.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://ob.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://ur.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://rb.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yf.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jr.nszjky.cn

Ruby: File.size("a.txt")
来源：http://fv.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://rs.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://cv.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pc.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aj.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ua.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://hh.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qq.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lw.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sb.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hc.9csxet.cn

[F11] 复制与移动文件
来源：http://eh.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xd.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tm.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fr.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://au.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mp.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sp.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gx.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dp.shtwfgs.cn

[F12] CSV 读写
来源：http://ll.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ez.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://om.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bo.9csxet.cn

TS:   // 同上
来源：http://hr.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kj.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vv.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mp.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wt.bjjhwx.cn

================================================================================
来源：http://py.hnjuh.cn

G. 面向对象
来源：http://og.yuntaijiaju.cn

================================================================================
来源：http://dk.huanxung.cn

[G01] 定义类
来源：http://dc.nszjky.cn

Py:   class User: pass
来源：http://kl.lnxyls.cn

PHP:  class User {}
来源：http://lu.9csxet.cn

JS:   class User {}
来源：http://nz.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://ip.hnjuh.cn

Java: class User {}
来源：http://zm.gzmigu.cn

Go:   type User struct { Name string }
来源：http://xa.wgjwhj.cn

Ruby: class User; end
来源：http://vx.hahajie.cn

C#:   class User {}
来源：http://gm.chemitech.net.cn

[G02] 构造函数
来源：http://xz.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://xj.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://bm.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://fh.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://fb.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://ze.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iz.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://pm.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://xd.shxzukj.cn

[G03] 实例属性
来源：http://tj.nszjky.cn

Py:   self.name = "x"
来源：http://ff.panjiajie.cn

PHP:  public string $name = "x";
来源：http://ep.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ie.newstarts.cn

TS:   name: string = "x";
来源：http://mz.huanxung.cn

Java: private String name;
来源：http://ch.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ai.shxzukj.cn

Ruby: @name = "x"
来源：http://su.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://cs.shxzukj.cn

[G04] 定义方法
来源：http://hq.9csxet.cn

Py:   def greet(self): return self.name
来源：http://so.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://go.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://sa.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://ln.521024.cn

Java: String greet() { return name; }
来源：http://fk.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rt.szxytkj.cn

Ruby: def greet; @name; end
来源：http://mn.szsharing.cn

C#:   public string Greet() => Name;
来源：http://kj.huanxung.cn

[G05] 继承
来源：http://vd.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ov.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://kx.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://mu.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ej.newstarts.cn

Java: class Admin extends User {}
来源：http://uf.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jw.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://wh.szxytkj.cn

C#:   class Admin : User {}
来源：http://vj.shtwfgs.cn

[G06] 重写方法
来源：http://kc.asd995.cn

Py:   def greet(self): return "admin"
来源：http://hr.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fh.asd995.cn

JS:   greet() { return "admin"; }
来源：http://gj.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://dg.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://up.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fy.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://dm.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://cy.szsharing.cn

[G07] 调用父类方法
来源：http://vt.huixiangedu.cn

Py:   super().greet()
来源：http://vi.gzmigu.cn

PHP:  parent::greet();
来源：http://kw.szsharing.cn

JS:   super.greet();
来源：http://jy.gzmigu.cn

TS:   super.greet();
来源：http://bu.nszjky.cn

Java: super.greet();
来源：http://ok.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lw.521024.cn

Ruby: super
来源：http://lu.huanxung.cn

C#:   base.Greet();
来源：http://ig.newstarts.cn

[G08] 静态方法与属性
来源：http://pg.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hf.9csxet.cn

PHP:  public static function f() {}
来源：http://yu.panjiajie.cn

JS:   static f() {}
来源：http://dq.bookmarksfly.cn

TS:   static f(): void {}
来源：http://mz.gzmigu.cn

Java: static void f() {}
来源：http://ut.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qd.bjjhwx.cn

Ruby: def self.f; end
来源：http://ca.nicolike.cn

C#:   public static void F() {}
来源：http://jl.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://kb.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://so.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wh.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://da.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://cz.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://yb.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://ov.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://df.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://tm.bjjhwx.cn

[G10] 访问控制
来源：http://ug.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://fj.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://cy.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://lr.nszjky.cn

TS:   public / protected / private
来源：http://im.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://jo.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gp.nicolike.cn

Ruby: public / protected / private
来源：http://mu.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://dl.yuntaijiaju.cn

[G11] getter / setter
来源：http://ql.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://ez.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nz.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://qv.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://tz.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://oa.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rw.shxzskj.cn

Ruby: attr_accessor :name
来源：http://rx.nicolike.cn

C#:   public string Name { get; set; }
来源：http://bt.shxzukj.cn

[G12] 对象转字符串
来源：http://ds.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://jc.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gs.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://yr.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://bs.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://od.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qp.nszjky.cn

Ruby: def to_s; @name; end
来源：http://jb.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://nv.panjiajie.cn

[G13] 判断对象类型
来源：http://me.shxzskj.cn

Py:   isinstance(u, User)
来源：http://wd.gzmigu.cn

PHP:  $u instanceof User
来源：http://lq.lnxyls.cn

JS:   u instanceof User
来源：http://gz.lnxyls.cn

TS:   u instanceof User
来源：http://cx.huixinmuqiang.cn

Java: u instanceof User
来源：http://fj.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sx.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://ui.yuexingan06.cn

C#:   u is User
来源：http://ct.szxytkj.cn

[G14] 数据类 / record
来源：http://fl.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://og.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://ji.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jk.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://os.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://vd.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://ko.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wu.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://yx.shtwfgs.cn

[G15] 枚举
来源：http://zr.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xr.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fd.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aj.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ry.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://km.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bs.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://ne.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sm.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://ep.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zn.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://nw.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://os.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://pu.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sg.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://er.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://xl.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://to.nicolike.cn

================================================================================
来源：http://yv.jianghongdianzi.cn

H. 异常与错误处理
来源：http://sd.hahajie.cn

================================================================================
来源：http://ue.lnxyls.cn

[H01] try / catch 基础
来源：http://eh.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dj.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://el.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qu.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zj.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://or.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xo.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hk.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ia.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://at.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vw.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sr.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jv.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ei.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yl.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dw.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ds.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oq.haigaiapp.cn


<!-- 参考信息 -->