代发 wailian999

[E22] 字节长度与字符长度
来源：http://pl.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jj.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xf.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wk.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://se.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gw.lnxyls.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://su.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://hd.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ee.521024.cn

================================================================================
来源：http://bk.yuexingan06.cn

F. 文件与目录
来源：http://qy.newstarts.cn

================================================================================
来源：http://dt.bjjhwx.cn

[F01] 读取整个文件
来源：http://xw.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ew.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://pj.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://em.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ud.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gh.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nf.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://qw.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://ib.huixiangedu.cn

[F02] 逐行读取文件
来源：http://cg.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lg.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zf.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://un.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hu.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ay.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xh.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hs.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kt.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://eu.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ks.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qx.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gf.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://du.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nu.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ez.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://dt.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uv.panjiajie.cn

[F04] 追加写入文件
来源：http://iz.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mq.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wc.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://st.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yw.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jy.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ly.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vk.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xq.521024.cn

[F05] 判断文件或目录是否存在
来源：http://ao.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pk.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://we.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://ak.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://nv.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zx.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cm.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://rk.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://rx.szsharing.cn

[F06] 删除文件
来源：http://zd.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://wf.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://ug.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ao.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ac.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bb.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://zw.asd995.cn

Ruby: File.delete("a.txt")
来源：http://rb.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://sq.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://fe.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zi.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sg.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hi.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fw.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://up.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ne.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ej.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lm.huixinmuqiang.cn

[F08] 遍历目录
来源：http://bi.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wm.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ck.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://tc.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://rp.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ga.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://be.huanxung.cn

Ruby: Dir.children("dir")
来源：http://if.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://si.yuexingan06.cn

[F09] 获取文件大小
来源：http://au.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://pq.colortex.cn

PHP:  filesize("a.txt");
来源：http://tk.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://qd.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://vd.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vu.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ku.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://vs.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://er.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://kw.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mg.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://we.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bd.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://cb.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://du.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pg.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xt.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zd.hahajie.cn

[F11] 复制与移动文件
来源：http://dd.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ew.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jx.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xq.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tl.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tq.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ff.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rk.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://px.nszjky.cn

[F12] CSV 读写
来源：http://yl.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vg.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://su.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bn.gzmigu.cn

TS:   // 同上
来源：http://hl.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mr.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sd.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qk.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vd.jianghongdianzi.cn

================================================================================
来源：http://iz.nicolike.cn

G. 面向对象
来源：http://vr.lnxyls.cn

================================================================================
来源：http://zy.shxzukj.cn

[G01] 定义类
来源：http://hh.huanxung.cn

Py:   class User: pass
来源：http://wy.huixinmuqiang.cn

PHP:  class User {}
来源：http://or.wgjwhj.cn

JS:   class User {}
来源：http://aq.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ys.shtwfgs.cn

Java: class User {}
来源：http://tm.colortex.cn

Go:   type User struct { Name string }
来源：http://pf.bjjhwx.cn

Ruby: class User; end
来源：http://yn.szxytkj.cn

C#:   class User {}
来源：http://op.asd995.cn

[G02] 构造函数
来源：http://ib.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://rl.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://yy.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://wg.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://gn.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://za.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ya.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ov.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ci.chemitech.net.cn

[G03] 实例属性
来源：http://ug.chemitech.net.cn

Py:   self.name = "x"
来源：http://ak.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://sq.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://mq.521024.cn

TS:   name: string = "x";
来源：http://gm.bookmarksfly.cn

Java: private String name;
来源：http://rb.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xz.bookmarksfly.cn

Ruby: @name = "x"
来源：http://vi.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://xc.colortex.cn

[G04] 定义方法
来源：http://ks.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://ri.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pj.9csxet.cn

JS:   greet() { return this.name; }
来源：http://wt.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://ei.shxzskj.cn

Java: String greet() { return name; }
来源：http://ck.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rk.szxytkj.cn

Ruby: def greet; @name; end
来源：http://nc.9csxet.cn

C#:   public string Greet() => Name;
来源：http://dr.colortex.cn

[G05] 继承
来源：http://us.shxzskj.cn

Py:   class Admin(User): pass
来源：http://pw.huanxung.cn

PHP:  class Admin extends User {}
来源：http://xg.hahajie.cn

JS:   class Admin extends User {}
来源：http://hc.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://nd.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://nj.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jw.szxytkj.cn

Ruby: class Admin < User; end
来源：http://sh.huanxung.cn

C#:   class Admin : User {}
来源：http://eq.shxzskj.cn

[G06] 重写方法
来源：http://hw.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://go.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jd.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://xv.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://dv.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://sg.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jo.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://wh.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://aq.asd995.cn

[G07] 调用父类方法
来源：http://ds.bjjhwx.cn

Py:   super().greet()
来源：http://pv.jctech888.com.cn

PHP:  parent::greet();
来源：http://nx.huixinmuqiang.cn

JS:   super.greet();
来源：http://bp.lnxyls.cn

TS:   super.greet();
来源：http://aj.yuntaijiaju.cn

Java: super.greet();
来源：http://hy.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ar.newstarts.cn

Ruby: super
来源：http://ha.shtwfgs.cn

C#:   base.Greet();
来源：http://wg.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://me.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yk.521024.cn

PHP:  public static function f() {}
来源：http://hd.jctech888.com.cn

JS:   static f() {}
来源：http://bg.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://ai.shxzskj.cn

Java: static void f() {}
来源：http://qr.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gk.yuexingan06.cn

Ruby: def self.f; end
来源：http://iw.huanxung.cn

C#:   public static void F() {}
来源：http://up.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://qo.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://mb.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hc.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kk.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://lv.colortex.cn

Java: interface Shape { double area(); }
来源：http://ga.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://hv.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aj.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://bj.hnjuh.cn

[G10] 访问控制
来源：http://vq.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://hg.jctech888.com.cn

PHP:  public / protected / private
来源：http://qu.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://hk.muxihuayi.cn

TS:   public / protected / private
来源：http://qk.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://wc.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ps.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://ae.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://hd.colortex.cn

[G11] getter / setter
来源：http://yp.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://gp.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yk.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://gf.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://ho.newstarts.cn

Java: public String getName() { return name; }
来源：http://cj.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tw.nszjky.cn

Ruby: attr_accessor :name
来源：http://bv.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://uo.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://kf.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://rs.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kp.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://hy.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://ml.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://qb.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kw.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://vj.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://tl.shxzukj.cn

[G13] 判断对象类型
来源：http://ro.nszjky.cn

Py:   isinstance(u, User)
来源：http://wi.asd995.cn

PHP:  $u instanceof User
来源：http://nt.9csxet.cn

JS:   u instanceof User
来源：http://og.szsharing.cn

TS:   u instanceof User
来源：http://zw.nszjky.cn

Java: u instanceof User
来源：http://us.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://in.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://me.huixinmuqiang.cn

C#:   u is User
来源：http://hi.jctech888.com.cn

[G14] 数据类 / record
来源：http://qw.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sr.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ny.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qc.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://mz.hahajie.cn

Java: record User(String name, int age) {}
来源：http://xa.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://fg.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ja.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://iw.shxzskj.cn

[G15] 枚举
来源：http://nh.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zb.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yh.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ui.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fw.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://li.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zg.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://ep.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ww.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://si.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wu.521024.cn

PHP:  get_object_vars($obj);
来源：http://mn.panjiajie.cn

JS:   Object.entries(obj)
来源：http://jg.szxytkj.cn

TS:   Object.entries(obj)
来源：http://va.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vh.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vz.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://wa.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://lr.gzmigu.cn

================================================================================
来源：http://ct.szsharing.cn

H. 异常与错误处理
来源：http://wp.huixiangedu.cn

================================================================================
来源：http://ow.muxihuayi.cn

[H01] try / catch 基础
来源：http://lg.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://up.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gh.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uu.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ry.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rq.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lr.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fa.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ie.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://io.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zw.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://um.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pv.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zh.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ge.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dd.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lz.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wp.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://jm.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://bb.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ci.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://mk.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ty.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://of.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gl.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tr.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qu.hnjuh.cn

[H04] 自定义异常类型
来源：http://tj.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://xt.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xf.521024.cn


<!-- 参考信息 -->