代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://oo.muxihuayi.cn

[F02] 逐行读取文件
来源：http://vd.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lx.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tt.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pj.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vl.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yf.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hs.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xy.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ap.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://mq.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dc.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://op.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qt.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kb.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bf.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gj.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://rg.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zl.muxihuayi.cn

[F04] 追加写入文件
来源：http://rd.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xt.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ty.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ex.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cg.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ln.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gf.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ty.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sh.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://rh.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sq.colortex.cn

PHP:  file_exists("a.txt");
来源：http://ki.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://kc.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://qv.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nf.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ep.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://pq.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://pn.jianghongdianzi.cn

[F06] 删除文件
来源：http://xb.asd995.cn

Py:   os.remove("a.txt")
来源：http://fc.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://dw.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ge.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zm.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kj.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://nh.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://lv.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://ox.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://mm.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://py.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ut.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://na.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://di.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yw.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yv.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wb.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lx.szsharing.cn

[F08] 遍历目录
来源：http://so.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://du.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ba.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://os.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://ju.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wz.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bt.huanxung.cn

Ruby: Dir.children("dir")
来源：http://pb.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://ic.shtwfgs.cn

[F09] 获取文件大小
来源：http://yu.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://xk.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://gs.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://qi.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ky.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vc.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lq.colortex.cn

Ruby: File.size("a.txt")
来源：http://yd.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://yg.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://cf.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mn.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ze.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vo.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://th.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xm.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ay.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tm.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nu.nszjky.cn

[F11] 复制与移动文件
来源：http://jf.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://to.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vb.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qf.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rr.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fm.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zb.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ys.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://or.jctech888.com.cn

[F12] CSV 读写
来源：http://ht.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dr.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xz.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://px.9csxet.cn

TS:   // 同上
来源：http://ha.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wc.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zt.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://in.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ri.nicolike.cn

================================================================================
来源：http://fd.yuexingan06.cn

G. 面向对象
来源：http://ib.lnxyls.cn

================================================================================
来源：http://fb.jctech888.com.cn

[G01] 定义类
来源：http://ix.bookmarksfly.cn

Py:   class User: pass
来源：http://to.jianghongdianzi.cn

PHP:  class User {}
来源：http://kt.yuexingan06.cn

JS:   class User {}
来源：http://xv.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://my.shtwfgs.cn

Java: class User {}
来源：http://sq.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://ds.newstarts.cn

Ruby: class User; end
来源：http://ip.jianghongdianzi.cn

C#:   class User {}
来源：http://og.521024.cn

[G02] 构造函数
来源：http://rj.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://hm.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://wk.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ce.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://ht.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://vm.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qc.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://nx.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://el.yuntaijiaju.cn

[G03] 实例属性
来源：http://vx.bookmarksfly.cn

Py:   self.name = "x"
来源：http://og.9csxet.cn

PHP:  public string $name = "x";
来源：http://if.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://ha.nszjky.cn

TS:   name: string = "x";
来源：http://ql.wgjwhj.cn

Java: private String name;
来源：http://ix.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ao.bookmarksfly.cn

Ruby: @name = "x"
来源：http://ok.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://xs.shxzskj.cn

[G04] 定义方法
来源：http://pr.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://qv.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rg.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://ud.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://xw.bjjhwx.cn

Java: String greet() { return name; }
来源：http://mw.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lp.nicolike.cn

Ruby: def greet; @name; end
来源：http://nz.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://lr.nszjky.cn

[G05] 继承
来源：http://hj.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://xl.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://uz.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://zd.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://lj.9csxet.cn

Java: class Admin extends User {}
来源：http://ge.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gs.panjiajie.cn

Ruby: class Admin < User; end
来源：http://zs.gzmigu.cn

C#:   class Admin : User {}
来源：http://bx.lnxyls.cn

[G06] 重写方法
来源：http://jl.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://wj.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gh.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://rf.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ji.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://tl.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rk.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://lk.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://ld.huixiangedu.cn

[G07] 调用父类方法
来源：http://jk.asd995.cn

Py:   super().greet()
来源：http://fb.wgjwhj.cn

PHP:  parent::greet();
来源：http://qk.muxihuayi.cn

JS:   super.greet();
来源：http://dw.newstarts.cn

TS:   super.greet();
来源：http://qa.asd995.cn

Java: super.greet();
来源：http://le.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xe.bookmarksfly.cn

Ruby: super
来源：http://ab.lnxyls.cn

C#:   base.Greet();
来源：http://ch.asd995.cn

[G08] 静态方法与属性
来源：http://yo.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ao.hnjuh.cn

PHP:  public static function f() {}
来源：http://ag.hahajie.cn

JS:   static f() {}
来源：http://uf.nicolike.cn

TS:   static f(): void {}
来源：http://dc.newstarts.cn

Java: static void f() {}
来源：http://ye.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pq.nicolike.cn

Ruby: def self.f; end
来源：http://ck.haigaiapp.cn

C#:   public static void F() {}
来源：http://rn.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://my.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://ws.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://op.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yi.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://pr.hahajie.cn

Java: interface Shape { double area(); }
来源：http://mr.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://yk.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nb.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://qi.szsharing.cn

[G10] 访问控制
来源：http://oe.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://lt.nicolike.cn

PHP:  public / protected / private
来源：http://qq.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://no.muxihuayi.cn

TS:   public / protected / private
来源：http://xy.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://jx.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vl.haigaiapp.cn

Ruby: public / protected / private
来源：http://yo.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://rd.huanxung.cn

[G11] getter / setter
来源：http://xs.colortex.cn

Py:   @property 与 @x.setter
来源：http://nu.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nu.huanxung.cn

JS:   get name() { return this._name; }
来源：http://qy.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://kb.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://tn.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jw.shxzukj.cn

Ruby: attr_accessor :name
来源：http://yq.colortex.cn

C#:   public string Name { get; set; }
来源：http://ce.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://sz.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://su.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hg.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://rd.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://gr.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://he.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ph.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://wl.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://gw.panjiajie.cn

[G13] 判断对象类型
来源：http://le.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://zq.gzmigu.cn

PHP:  $u instanceof User
来源：http://ab.wgjwhj.cn

JS:   u instanceof User
来源：http://hy.szxytkj.cn

TS:   u instanceof User
来源：http://zt.chemitech.net.cn

Java: u instanceof User
来源：http://ci.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ej.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://ug.shtwfgs.cn

C#:   u is User
来源：http://za.shtwfgs.cn

[G14] 数据类 / record
来源：http://tv.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://um.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://af.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sd.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://ao.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://py.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://zv.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fs.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://yt.huixiangedu.cn

[G15] 枚举
来源：http://mz.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hh.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gd.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wd.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wr.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://yh.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ur.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://jy.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yk.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://vq.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nm.asd995.cn

PHP:  get_object_vars($obj);
来源：http://ic.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://em.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://sy.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qz.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iw.hahajie.cn

Ruby: obj.instance_variables
来源：http://gf.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://jv.hnjuh.cn

================================================================================
来源：http://ew.muxihuayi.cn

H. 异常与错误处理
来源：http://ev.shxzukj.cn

================================================================================
来源：http://jx.lnxyls.cn

[H01] try / catch 基础
来源：http://pn.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ss.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hm.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jz.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ep.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rq.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://md.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yp.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xc.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://eb.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ct.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ut.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cx.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mj.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ej.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sd.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hl.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uf.hahajie.cn

[H03] 主动抛出异常
来源：http://ju.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://zg.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vh.asd995.cn

JS:   throw new Error("错误信息");
来源：http://nh.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://zx.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://da.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pe.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gg.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hv.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://fn.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://un.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lt.9csxet.cn

JS:   class MyError extends Error {}
来源：http://zf.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://xj.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://uo.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ew.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://ek.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://eh.wgjwhj.cn

[H05] 捕获特定类型
来源：http://ky.nicolike.cn

Py:   except ValueError as e:
来源：http://wa.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sc.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://cz.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://xg.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://wc.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ih.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://yq.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fi.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://dv.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://nf.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fv.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zb.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uf.yuexingan06.cn


<!-- 参考信息 -->