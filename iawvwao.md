代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yw.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ub.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ii.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sn.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dp.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://bu.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dp.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ou.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://tb.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ti.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kt.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dn.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mr.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ae.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sw.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://la.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nb.yuexingan06.cn

================================================================================
来源：http://ol.nszjky.cn

F. 文件与目录
来源：http://zu.shxzskj.cn

================================================================================
来源：http://fx.shtwfgs.cn

[F01] 读取整个文件
来源：http://sj.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mk.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://ey.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wz.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hk.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nz.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xf.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://ph.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://iw.colortex.cn

[F02] 逐行读取文件
来源：http://lz.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sk.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mq.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ak.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qz.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bb.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://td.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ua.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://em.asd995.cn

[F03] 写入文件（覆盖）
来源：http://ww.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jj.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tp.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vr.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://th.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wq.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yd.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://mh.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vt.szxytkj.cn

[F04] 追加写入文件
来源：http://bk.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sm.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jt.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rs.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gz.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ho.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dm.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dl.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jy.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://oc.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://da.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://fg.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://tt.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://lq.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dk.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sm.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://by.521024.cn

C#:   File.Exists("a.txt")
来源：http://cm.nicolike.cn

[F06] 删除文件
来源：http://sp.nszjky.cn

Py:   os.remove("a.txt")
来源：http://sr.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://aj.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bd.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ba.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oj.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://gf.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://qb.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://hi.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://jk.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qe.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sq.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yk.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://be.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://av.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ot.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://br.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cj.jctech888.com.cn

[F08] 遍历目录
来源：http://na.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vy.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ui.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://oc.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ex.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ud.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pe.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://dd.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://dg.9csxet.cn

[F09] 获取文件大小
来源：http://eq.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://mb.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://yq.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://aa.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://th.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ng.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oo.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://sh.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ed.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://gg.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cl.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sd.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xy.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://hj.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ij.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cp.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ub.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://id.wgjwhj.cn

[F11] 复制与移动文件
来源：http://av.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ba.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://el.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gy.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fa.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vd.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fy.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wd.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gb.chemitech.net.cn

[F12] CSV 读写
来源：http://ae.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jd.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wc.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://st.huixinmuqiang.cn

TS:   // 同上
来源：http://pc.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vm.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qo.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nu.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://to.huixinmuqiang.cn

================================================================================
来源：http://go.lnxyls.cn

G. 面向对象
来源：http://ub.bookmarksfly.cn

================================================================================
来源：http://xy.muxihuayi.cn

[G01] 定义类
来源：http://zs.shxzukj.cn

Py:   class User: pass
来源：http://jb.shtwfgs.cn

PHP:  class User {}
来源：http://bh.szsharing.cn

JS:   class User {}
来源：http://re.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://oj.huixiangedu.cn

Java: class User {}
来源：http://co.nicolike.cn

Go:   type User struct { Name string }
来源：http://pq.lnxyls.cn

Ruby: class User; end
来源：http://gc.huixinmuqiang.cn

C#:   class User {}
来源：http://be.gzmigu.cn

[G02] 构造函数
来源：http://ws.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://ds.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://kj.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://mi.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://ou.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://zc.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gx.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://nh.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://ej.shxzukj.cn

[G03] 实例属性
来源：http://kw.huanxung.cn

Py:   self.name = "x"
来源：http://tj.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://rw.newstarts.cn

JS:   this.name = "x";
来源：http://tn.shxzskj.cn

TS:   name: string = "x";
来源：http://dr.asd995.cn

Java: private String name;
来源：http://wt.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yo.huixiangedu.cn

Ruby: @name = "x"
来源：http://wg.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://tk.wgjwhj.cn

[G04] 定义方法
来源：http://tw.521024.cn

Py:   def greet(self): return self.name
来源：http://uj.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cz.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://ia.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://ea.lnxyls.cn

Java: String greet() { return name; }
来源：http://bs.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vw.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://ju.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://oh.shxzskj.cn

[G05] 继承
来源：http://wv.newstarts.cn

Py:   class Admin(User): pass
来源：http://ti.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://ie.lnxyls.cn

JS:   class Admin extends User {}
来源：http://me.nszjky.cn

TS:   class Admin extends User {}
来源：http://fo.huixiangedu.cn

Java: class Admin extends User {}
来源：http://ht.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tg.shxzskj.cn

Ruby: class Admin < User; end
来源：http://kr.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://id.lnxyls.cn

[G06] 重写方法
来源：http://bl.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://vx.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mp.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://dl.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://xd.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://oz.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bp.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://xb.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://pu.shxzukj.cn

[G07] 调用父类方法
来源：http://rp.colortex.cn

Py:   super().greet()
来源：http://fl.9csxet.cn

PHP:  parent::greet();
来源：http://cn.bjjhwx.cn

JS:   super.greet();
来源：http://tu.panjiajie.cn

TS:   super.greet();
来源：http://fm.shxzskj.cn

Java: super.greet();
来源：http://xg.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vy.bjjhwx.cn

Ruby: super
来源：http://kv.bookmarksfly.cn

C#:   base.Greet();
来源：http://zv.szsharing.cn

[G08] 静态方法与属性
来源：http://yn.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qr.huixiangedu.cn

PHP:  public static function f() {}
来源：http://sf.wgjwhj.cn

JS:   static f() {}
来源：http://cm.hahajie.cn

TS:   static f(): void {}
来源：http://vo.colortex.cn

Java: static void f() {}
来源：http://zh.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://es.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://iy.521024.cn

C#:   public static void F() {}
来源：http://tb.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://ue.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://jx.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sd.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yi.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://ll.521024.cn

Java: interface Shape { double area(); }
来源：http://rh.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://nk.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vz.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://dm.chemitech.net.cn

[G10] 访问控制
来源：http://lf.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://el.nicolike.cn

PHP:  public / protected / private
来源：http://xs.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://gw.9csxet.cn

TS:   public / protected / private
来源：http://pn.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://ak.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lp.hahajie.cn

Ruby: public / protected / private
来源：http://yb.521024.cn

C#:   public / protected / private / internal
来源：http://fk.panjiajie.cn

[G11] getter / setter
来源：http://ji.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://re.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jq.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://gh.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://mu.gzmigu.cn

Java: public String getName() { return name; }
来源：http://hx.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://le.newstarts.cn

Ruby: attr_accessor :name
来源：http://nn.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://mm.asd995.cn

[G12] 对象转字符串
来源：http://oz.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://yg.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://re.9csxet.cn

JS:   toString() { return this.name; }
来源：http://sd.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://ts.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://gh.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ja.asd995.cn

Ruby: def to_s; @name; end
来源：http://jq.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://sv.shxzskj.cn

[G13] 判断对象类型
来源：http://cm.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://bz.newstarts.cn

PHP:  $u instanceof User
来源：http://fb.panjiajie.cn

JS:   u instanceof User
来源：http://mu.bookmarksfly.cn

TS:   u instanceof User
来源：http://tw.huanxung.cn

Java: u instanceof User
来源：http://gs.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://so.nicolike.cn

Ruby: u.is_a?(User)
来源：http://xn.panjiajie.cn

C#:   u is User
来源：http://aa.colortex.cn

[G14] 数据类 / record
来源：http://ac.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://be.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://tq.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fs.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://mf.nicolike.cn

Java: record User(String name, int age) {}
来源：http://hd.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://fu.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qa.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://vb.panjiajie.cn

[G15] 枚举
来源：http://uy.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ym.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xs.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cs.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ji.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://fh.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sj.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://oy.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vq.colortex.cn

[G16] 对象转数组 / 字典
来源：http://os.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cm.colortex.cn

PHP:  get_object_vars($obj);
来源：http://tv.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://ta.nszjky.cn

TS:   Object.entries(obj)
来源：http://su.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fd.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ra.szxytkj.cn

Ruby: obj.instance_variables
来源：http://vf.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://ty.gzmigu.cn

================================================================================
来源：http://eb.newstarts.cn

H. 异常与错误处理
来源：http://nq.jianghongdianzi.cn

================================================================================
来源：http://ww.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://lx.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xo.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://em.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lm.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ft.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dh.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ci.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bz.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qu.szsharing.cn

[H02] finally / ensure 收尾
来源：http://sz.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ue.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://em.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ov.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yt.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aa.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zt.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://to.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vz.nicolike.cn

[H03] 主动抛出异常
来源：http://ji.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://sy.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vz.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://xe.yuntaijiaju.cn


<!-- 参考信息 -->