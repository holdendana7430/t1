代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yz.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yc.wgjwhj.cn

TS:   if (s === "") {}
来源：http://pd.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://lr.wgjwhj.cn

Go:   if s == "" {}
来源：http://jq.bookmarksfly.cn

Ruby: if s.empty?
来源：http://gq.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bh.shxzukj.cn

[E21] 超长截断加省略号
来源：http://ti.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ze.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ty.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ai.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yj.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://js.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://px.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fd.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rs.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://uq.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mo.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kr.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aq.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aa.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://of.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ia.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://pb.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ei.muxihuayi.cn

================================================================================
来源：http://jl.huanxung.cn

F. 文件与目录
来源：http://dj.bookmarksfly.cn

================================================================================
来源：http://sy.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://wy.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://af.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://lb.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uy.szxytkj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mk.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ad.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tt.asd995.cn

Ruby: File.read("a.txt")
来源：http://eb.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://ce.muxihuayi.cn

[F02] 逐行读取文件
来源：http://dk.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nx.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hy.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://te.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uf.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ts.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ck.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cq.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zd.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://tk.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lf.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yb.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pm.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://md.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oh.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dm.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://pw.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oq.521024.cn

[F04] 追加写入文件
来源：http://ez.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zl.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uj.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lr.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vt.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ul.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pl.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yl.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kx.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://yl.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hy.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://mc.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://sp.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://jq.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sz.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://fu.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://su.9csxet.cn

[F06] 删除文件
来源：http://fn.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://cj.nszjky.cn

PHP:  unlink("a.txt");
来源：http://af.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xs.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dq.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://de.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://ka.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://pw.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://dt.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://zf.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eu.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zf.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dk.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gc.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://le.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kq.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gq.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://un.nszjky.cn

[F08] 遍历目录
来源：http://yy.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://do.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ez.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://fn.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://bs.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bh.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ue.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://qk.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://ko.colortex.cn

[F09] 获取文件大小
来源：http://ux.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://gk.hahajie.cn

PHP:  filesize("a.txt");
来源：http://bb.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://dx.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://un.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ip.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gv.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://cr.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://yn.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://dk.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xi.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://to.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fm.newstarts.cn

TS:   path.extname("a.txt")
来源：http://ep.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rv.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oy.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vz.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://to.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://ig.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wr.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dk.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cb.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://je.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bm.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tp.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cy.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ak.asd995.cn

[F12] CSV 读写
来源：http://cp.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jr.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uu.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vj.9csxet.cn

TS:   // 同上
来源：http://od.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pe.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tq.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iu.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vw.9csxet.cn

================================================================================
来源：http://mo.nicolike.cn

G. 面向对象
来源：http://px.gzmigu.cn

================================================================================
来源：http://kp.huanxung.cn

[G01] 定义类
来源：http://zq.newstarts.cn

Py:   class User: pass
来源：http://vo.panjiajie.cn

PHP:  class User {}
来源：http://zf.hnjuh.cn

JS:   class User {}
来源：http://mt.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://db.wgjwhj.cn

Java: class User {}
来源：http://lk.panjiajie.cn

Go:   type User struct { Name string }
来源：http://ou.521024.cn

Ruby: class User; end
来源：http://ci.huixiangedu.cn

C#:   class User {}
来源：http://md.chemitech.net.cn

[G02] 构造函数
来源：http://yq.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://fq.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://iq.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://rt.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://in.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://mr.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rm.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://dz.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://lf.yuexingan06.cn

[G03] 实例属性
来源：http://bi.shxzukj.cn

Py:   self.name = "x"
来源：http://yd.huanxung.cn

PHP:  public string $name = "x";
来源：http://ux.haigaiapp.cn

JS:   this.name = "x";
来源：http://qf.szsharing.cn

TS:   name: string = "x";
来源：http://od.jctech888.com.cn

Java: private String name;
来源：http://tp.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wn.bookmarksfly.cn

Ruby: @name = "x"
来源：http://mn.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://zh.huixiangedu.cn

[G04] 定义方法
来源：http://rz.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://an.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lv.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://pr.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://su.wgjwhj.cn

Java: String greet() { return name; }
来源：http://gb.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://to.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://cq.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://xz.hahajie.cn

[G05] 继承
来源：http://zf.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://py.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://in.huanxung.cn

JS:   class Admin extends User {}
来源：http://bp.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://up.panjiajie.cn

Java: class Admin extends User {}
来源：http://jq.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pc.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://al.muxihuayi.cn

C#:   class Admin : User {}
来源：http://po.521024.cn

[G06] 重写方法
来源：http://kl.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://eq.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uc.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://bi.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://kg.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ub.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://he.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://gv.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://km.colortex.cn

[G07] 调用父类方法
来源：http://zv.yuntaijiaju.cn

Py:   super().greet()
来源：http://lw.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://hu.shxzskj.cn

JS:   super.greet();
来源：http://ss.muxihuayi.cn

TS:   super.greet();
来源：http://il.szsharing.cn

Java: super.greet();
来源：http://rb.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sd.panjiajie.cn

Ruby: super
来源：http://ut.muxihuayi.cn

C#:   base.Greet();
来源：http://ne.9csxet.cn

[G08] 静态方法与属性
来源：http://si.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://br.9csxet.cn

PHP:  public static function f() {}
来源：http://dq.wgjwhj.cn

JS:   static f() {}
来源：http://ni.panjiajie.cn

TS:   static f(): void {}
来源：http://zy.colortex.cn

Java: static void f() {}
来源：http://eg.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uk.9csxet.cn

Ruby: def self.f; end
来源：http://rd.yuexingan06.cn

C#:   public static void F() {}
来源：http://wh.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://bl.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://vt.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kw.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wj.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://lu.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://po.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://fj.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ci.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://dl.huixinmuqiang.cn

[G10] 访问控制
来源：http://xh.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://gw.hahajie.cn

PHP:  public / protected / private
来源：http://pp.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://ll.huixinmuqiang.cn

TS:   public / protected / private
来源：http://fa.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://ug.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://le.szsharing.cn

Ruby: public / protected / private
来源：http://nq.newstarts.cn

C#:   public / protected / private / internal
来源：http://hr.asd995.cn

[G11] getter / setter
来源：http://di.asd995.cn

Py:   @property 与 @x.setter
来源：http://hb.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dr.colortex.cn

JS:   get name() { return this._name; }
来源：http://mx.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://sv.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://uc.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sj.asd995.cn

Ruby: attr_accessor :name
来源：http://zw.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://yx.gzmigu.cn

[G12] 对象转字符串
来源：http://gm.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://bc.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://me.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://lu.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://hg.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://pe.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pe.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://pk.colortex.cn

C#:   public override string ToString() => Name;
来源：http://nm.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://fp.nicolike.cn

Py:   isinstance(u, User)
来源：http://ci.9csxet.cn

PHP:  $u instanceof User
来源：http://ll.panjiajie.cn

JS:   u instanceof User
来源：http://vp.colortex.cn

TS:   u instanceof User
来源：http://fo.hahajie.cn

Java: u instanceof User
来源：http://vf.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vs.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://cx.nicolike.cn

C#:   u is User
来源：http://qd.huanxung.cn

[G14] 数据类 / record
来源：http://tl.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fk.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://of.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jf.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://hw.9csxet.cn

Java: record User(String name, int age) {}
来源：http://wd.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://my.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mi.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://xh.wgjwhj.cn

[G15] 枚举
来源：http://rq.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xq.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hf.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://or.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://du.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://uj.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bm.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://tj.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dh.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://un.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hn.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://xm.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://ph.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://by.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ba.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ao.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://rr.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ji.huixinmuqiang.cn

================================================================================
来源：http://et.chemitech.net.cn

H. 异常与错误处理
来源：http://bz.jctech888.com.cn

================================================================================
来源：http://si.panjiajie.cn

[H01] try / catch 基础
来源：http://yx.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ke.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yv.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mb.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://io.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pa.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lj.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qc.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yl.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://vb.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mk.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://me.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sa.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ky.521024.cn


<!-- 参考信息 -->