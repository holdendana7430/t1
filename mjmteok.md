代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xi.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zl.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://to.newstarts.cn

Ruby: File.read("a.txt")
来源：http://lc.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://cf.gzmigu.cn

[F02] 逐行读取文件
来源：http://cs.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ur.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vd.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rv.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rv.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bw.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nd.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sh.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ll.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://oa.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vj.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yx.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bi.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qa.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tv.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://px.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://kw.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rp.gzmigu.cn

[F04] 追加写入文件
来源：http://la.shxzskj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bb.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kg.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://np.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xw.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ad.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wi.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yb.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://ea.huanxung.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qe.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://hn.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://ih.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://bv.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sp.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ij.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://xb.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://zg.muxihuayi.cn

[F06] 删除文件
来源：http://py.asd995.cn

Py:   os.remove("a.txt")
来源：http://om.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://ja.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pt.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gi.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kx.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://db.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://xg.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://dm.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://qf.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fp.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ep.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rp.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ks.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://su.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lp.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ph.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zu.shxzskj.cn

[F08] 遍历目录
来源：http://ur.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dn.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qi.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://zi.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://yw.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cd.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://io.asd995.cn

Ruby: Dir.children("dir")
来源：http://ep.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://jw.szxytkj.cn

[F09] 获取文件大小
来源：http://fd.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://el.521024.cn

PHP:  filesize("a.txt");
来源：http://ns.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ps.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://rr.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wh.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zk.9csxet.cn

Ruby: File.size("a.txt")
来源：http://jo.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://ya.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://fg.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://il.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hj.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jz.nszjky.cn

TS:   path.extname("a.txt")
来源：http://la.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ss.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bj.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ip.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sn.521024.cn

[F11] 复制与移动文件
来源：http://tt.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://am.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rd.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qm.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zw.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cf.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mq.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://al.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ax.muxihuayi.cn

[F12] CSV 读写
来源：http://ts.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cr.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wd.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xp.jianghongdianzi.cn

TS:   // 同上
来源：http://li.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tx.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://av.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dn.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ch.gzmigu.cn

================================================================================
来源：http://qn.nicolike.cn

G. 面向对象
来源：http://no.yuntaijiaju.cn

================================================================================
来源：http://wy.521024.cn

[G01] 定义类
来源：http://ak.shxzskj.cn

Py:   class User: pass
来源：http://aw.hnjuh.cn

PHP:  class User {}
来源：http://sk.wgjwhj.cn

JS:   class User {}
来源：http://aw.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://qb.9csxet.cn

Java: class User {}
来源：http://bh.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://ya.asd995.cn

Ruby: class User; end
来源：http://cx.szsharing.cn

C#:   class User {}
来源：http://se.szsharing.cn

[G02] 构造函数
来源：http://ry.nicolike.cn

Py:   def __init__(self, name): self.name = name
来源：http://pz.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://kw.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://ow.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://ii.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://jr.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lr.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://ah.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://mo.szsharing.cn

[G03] 实例属性
来源：http://ai.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://cc.lnxyls.cn

PHP:  public string $name = "x";
来源：http://cy.shtwfgs.cn

JS:   this.name = "x";
来源：http://rk.haigaiapp.cn

TS:   name: string = "x";
来源：http://yw.szxytkj.cn

Java: private String name;
来源：http://vd.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kc.szsharing.cn

Ruby: @name = "x"
来源：http://nh.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://xd.haigaiapp.cn

[G04] 定义方法
来源：http://ir.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://wm.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yo.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://ju.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://nh.shxzskj.cn

Java: String greet() { return name; }
来源：http://cz.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xl.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://lg.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://tp.lnxyls.cn

[G05] 继承
来源：http://eb.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://ua.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://hf.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://xf.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://yp.chemitech.net.cn

Java: class Admin extends User {}
来源：http://dd.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://po.shxzskj.cn

Ruby: class Admin < User; end
来源：http://td.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ar.lnxyls.cn

[G06] 重写方法
来源：http://dv.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://vk.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fg.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://lu.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://lt.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://bv.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zy.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://fn.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://pi.9csxet.cn

[G07] 调用父类方法
来源：http://ve.yuntaijiaju.cn

Py:   super().greet()
来源：http://zl.chemitech.net.cn

PHP:  parent::greet();
来源：http://xh.bookmarksfly.cn

JS:   super.greet();
来源：http://xv.nicolike.cn

TS:   super.greet();
来源：http://sd.szxytkj.cn

Java: super.greet();
来源：http://oa.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uf.hahajie.cn

Ruby: super
来源：http://ti.bjjhwx.cn

C#:   base.Greet();
来源：http://qs.panjiajie.cn

[G08] 静态方法与属性
来源：http://hw.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vw.gzmigu.cn

PHP:  public static function f() {}
来源：http://sq.lnxyls.cn

JS:   static f() {}
来源：http://ya.hnjuh.cn

TS:   static f(): void {}
来源：http://xv.yuexingan06.cn

Java: static void f() {}
来源：http://ko.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tz.huanxung.cn

Ruby: def self.f; end
来源：http://tm.nszjky.cn

C#:   public static void F() {}
来源：http://oa.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://tu.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://al.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ui.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://on.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://hp.hahajie.cn

Java: interface Shape { double area(); }
来源：http://nt.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://ok.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gs.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://yg.wgjwhj.cn

[G10] 访问控制
来源：http://gd.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://yq.shxzukj.cn

PHP:  public / protected / private
来源：http://zq.huanxung.cn

JS:   #private 字段；其余公开
来源：http://ce.bookmarksfly.cn

TS:   public / protected / private
来源：http://oa.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://hx.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mx.nszjky.cn

Ruby: public / protected / private
来源：http://xr.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://ht.huixinmuqiang.cn

[G11] getter / setter
来源：http://zl.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://xi.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yr.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://cd.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://ub.hnjuh.cn

Java: public String getName() { return name; }
来源：http://fk.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qz.gzmigu.cn

Ruby: attr_accessor :name
来源：http://hr.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://xm.lnxyls.cn

[G12] 对象转字符串
来源：http://mu.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://nd.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rw.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://di.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://pg.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://zf.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qv.nszjky.cn

Ruby: def to_s; @name; end
来源：http://ry.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://tr.shxzukj.cn

[G13] 判断对象类型
来源：http://jl.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://yw.newstarts.cn

PHP:  $u instanceof User
来源：http://bc.bjjhwx.cn

JS:   u instanceof User
来源：http://hv.huanxung.cn

TS:   u instanceof User
来源：http://dk.shxzskj.cn

Java: u instanceof User
来源：http://uh.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ls.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://cd.gzmigu.cn

C#:   u is User
来源：http://cd.yuexingan06.cn

[G14] 数据类 / record
来源：http://eg.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iv.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://ov.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wv.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://xx.newstarts.cn

Java: record User(String name, int age) {}
来源：http://ah.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://dx.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ki.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://cs.yuntaijiaju.cn

[G15] 枚举
来源：http://um.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ui.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rx.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://md.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jk.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://rc.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mr.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://xy.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mv.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://zt.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gk.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://kv.szsharing.cn

JS:   Object.entries(obj)
来源：http://hf.colortex.cn

TS:   Object.entries(obj)
来源：http://kz.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hp.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wx.shxzukj.cn

Ruby: obj.instance_variables
来源：http://eu.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://nv.panjiajie.cn

================================================================================
来源：http://xt.asd995.cn

H. 异常与错误处理
来源：http://cc.shxzukj.cn

================================================================================
来源：http://xd.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://yv.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://it.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ie.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xa.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iq.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qv.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sx.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kd.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nx.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://pd.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://av.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cf.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wv.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mw.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ju.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ne.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pm.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lv.newstarts.cn

[H03] 主动抛出异常
来源：http://hi.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://yo.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hj.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://ue.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://cr.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gz.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hc.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://na.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cx.gzmigu.cn

[H04] 自定义异常类型
来源：http://ea.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://kx.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wy.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://gc.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://rk.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://bh.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cm.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://jd.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://aw.panjiajie.cn

[H05] 捕获特定类型
来源：http://sv.bjjhwx.cn

Py:   except ValueError as e:
来源：http://bu.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ua.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://er.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://xp.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://vx.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yj.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://jl.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://je.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://lh.wgjwhj.cn


<!-- 参考信息 -->