代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://td.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hq.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wr.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://nq.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fa.yuexingan06.cn

================================================================================
来源：http://dv.shxzskj.cn

F. 文件与目录
来源：http://lz.hahajie.cn

================================================================================
来源：http://uv.shxzukj.cn

[F01] 读取整个文件
来源：http://xf.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gs.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://ib.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uo.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zk.panjiajie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://us.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yk.hahajie.cn

Ruby: File.read("a.txt")
来源：http://ib.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://kq.gzmigu.cn

[F02] 逐行读取文件
来源：http://bx.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://he.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fr.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://no.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://go.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ia.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cf.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ny.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://up.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://ty.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rc.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qy.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cq.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lm.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ga.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ie.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://zg.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nd.szsharing.cn

[F04] 追加写入文件
来源：http://oq.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mm.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uq.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ed.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ei.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uf.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://py.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ma.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://md.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://zk.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bg.521024.cn

PHP:  file_exists("a.txt");
来源：http://em.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://gu.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://zd.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ao.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kd.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://da.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://ca.521024.cn

[F06] 删除文件
来源：http://bb.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://ly.huanxung.cn

PHP:  unlink("a.txt");
来源：http://ra.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wy.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://up.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yd.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://ge.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://gi.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://hp.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://ev.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aw.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mp.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tz.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://es.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ik.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ex.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jx.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sg.jctech888.com.cn

[F08] 遍历目录
来源：http://vs.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://eh.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rc.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://jm.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://ml.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ix.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hu.nicolike.cn

Ruby: Dir.children("dir")
来源：http://bg.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://us.huanxung.cn

[F09] 获取文件大小
来源：http://wy.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://lk.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://ac.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://sc.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://ia.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xr.bjjhwx.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xb.huanxung.cn

Ruby: File.size("a.txt")
来源：http://pm.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://tx.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://kv.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oj.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pd.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rb.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://vw.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ek.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gt.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rc.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iz.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://dh.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zr.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ce.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ua.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qv.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pw.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jk.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ga.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ab.gzmigu.cn

[F12] CSV 读写
来源：http://nx.521024.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aa.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qm.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hy.yuexingan06.cn

TS:   // 同上
来源：http://ff.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ar.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sa.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jv.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hg.shtwfgs.cn

================================================================================
来源：http://ro.colortex.cn

G. 面向对象
来源：http://ap.newstarts.cn

================================================================================
来源：http://xq.jctech888.com.cn

[G01] 定义类
来源：http://xy.szxytkj.cn

Py:   class User: pass
来源：http://ui.shxzukj.cn

PHP:  class User {}
来源：http://ly.hnjuh.cn

JS:   class User {}
来源：http://eh.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://im.shxzskj.cn

Java: class User {}
来源：http://wn.szsharing.cn

Go:   type User struct { Name string }
来源：http://ib.nicolike.cn

Ruby: class User; end
来源：http://mj.shtwfgs.cn

C#:   class User {}
来源：http://pf.newstarts.cn

[G02] 构造函数
来源：http://gc.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://dw.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://gg.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://jd.asd995.cn

TS:   constructor(public name: string) {}
来源：http://bw.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://fe.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bx.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://wq.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://bl.haigaiapp.cn

[G03] 实例属性
来源：http://nu.huixiangedu.cn

Py:   self.name = "x"
来源：http://sn.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://eo.9csxet.cn

JS:   this.name = "x";
来源：http://ku.szxytkj.cn

TS:   name: string = "x";
来源：http://kb.nicolike.cn

Java: private String name;
来源：http://ue.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qx.lnxyls.cn

Ruby: @name = "x"
来源：http://zu.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://um.szxytkj.cn

[G04] 定义方法
来源：http://ck.newstarts.cn

Py:   def greet(self): return self.name
来源：http://pl.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://og.nszjky.cn

JS:   greet() { return this.name; }
来源：http://yu.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://nt.shtwfgs.cn

Java: String greet() { return name; }
来源：http://xq.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gh.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://be.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://bm.gzmigu.cn

[G05] 继承
来源：http://ef.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://hz.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://bf.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://wm.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://wp.lnxyls.cn

Java: class Admin extends User {}
来源：http://mt.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wf.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://yf.huanxung.cn

C#:   class Admin : User {}
来源：http://hz.muxihuayi.cn

[G06] 重写方法
来源：http://my.colortex.cn

Py:   def greet(self): return "admin"
来源：http://oz.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ww.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://bu.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://bn.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://gj.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lg.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://iq.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://jd.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://bv.asd995.cn

Py:   super().greet()
来源：http://rj.chemitech.net.cn

PHP:  parent::greet();
来源：http://gc.bjjhwx.cn

JS:   super.greet();
来源：http://ya.shxzukj.cn

TS:   super.greet();
来源：http://ab.newstarts.cn

Java: super.greet();
来源：http://qu.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rp.colortex.cn

Ruby: super
来源：http://cb.lnxyls.cn

C#:   base.Greet();
来源：http://so.huanxung.cn

[G08] 静态方法与属性
来源：http://ko.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xs.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://wf.nicolike.cn

JS:   static f() {}
来源：http://zv.muxihuayi.cn

TS:   static f(): void {}
来源：http://uy.yuntaijiaju.cn

Java: static void f() {}
来源：http://uv.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vz.9csxet.cn

Ruby: def self.f; end
来源：http://ac.nszjky.cn

C#:   public static void F() {}
来源：http://wm.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://dg.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://le.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yd.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://su.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ub.nszjky.cn

Java: interface Shape { double area(); }
来源：http://jx.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://av.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ce.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://st.bjjhwx.cn

[G10] 访问控制
来源：http://am.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://qx.asd995.cn

PHP:  public / protected / private
来源：http://pv.huanxung.cn

JS:   #private 字段；其余公开
来源：http://tf.521024.cn

TS:   public / protected / private
来源：http://vo.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://em.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yv.gzmigu.cn

Ruby: public / protected / private
来源：http://wv.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://nl.nicolike.cn

[G11] getter / setter
来源：http://wa.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://gy.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mw.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://mv.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://vh.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://ky.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kd.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ac.nszjky.cn

C#:   public string Name { get; set; }
来源：http://ea.huixiangedu.cn

[G12] 对象转字符串
来源：http://xn.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://uc.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rl.nszjky.cn

JS:   toString() { return this.name; }
来源：http://ew.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://ep.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://rt.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ko.nszjky.cn

Ruby: def to_s; @name; end
来源：http://pq.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://rz.panjiajie.cn

[G13] 判断对象类型
来源：http://mk.hahajie.cn

Py:   isinstance(u, User)
来源：http://og.muxihuayi.cn

PHP:  $u instanceof User
来源：http://kq.colortex.cn

JS:   u instanceof User
来源：http://ds.shxzukj.cn

TS:   u instanceof User
来源：http://xj.wgjwhj.cn

Java: u instanceof User
来源：http://vt.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pt.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://ac.bookmarksfly.cn

C#:   u is User
来源：http://hp.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://pd.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lt.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://zd.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dw.521024.cn

TS:   type User = { name: string; age: number };
来源：http://wh.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://iy.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://fa.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mv.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://sz.hnjuh.cn

[G15] 枚举
来源：http://cm.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gq.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rx.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bd.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qr.521024.cn

Java: enum Color { RED, GREEN }
来源：http://hj.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qh.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://dc.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qd.521024.cn

[G16] 对象转数组 / 字典
来源：http://nc.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kj.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://qp.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://uh.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://bn.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mz.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vm.huanxung.cn

Ruby: obj.instance_variables
来源：http://fw.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://zs.shxzukj.cn

================================================================================
来源：http://sk.lnxyls.cn

H. 异常与错误处理
来源：http://jl.shtwfgs.cn

================================================================================
来源：http://ab.colortex.cn

[H01] try / catch 基础
来源：http://lg.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oi.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ud.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jt.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uf.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qt.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hc.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://st.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ws.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://yi.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hy.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ow.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iq.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jw.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jh.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eq.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ve.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ov.asd995.cn

[H03] 主动抛出异常
来源：http://cm.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://od.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gc.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://mq.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://dm.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bb.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ov.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zr.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gt.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://sj.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://lj.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dq.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://sd.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://tp.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://oa.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sr.shtwfgs.cn


<!-- 参考信息 -->