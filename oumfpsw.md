代发 wailian999

[F01] 读取整个文件
来源：http://jw.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dn.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://hu.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ml.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mp.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hf.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rp.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://yz.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://bt.lnxyls.cn

[F02] 逐行读取文件
来源：http://ou.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://an.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oh.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rh.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cs.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qm.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xr.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://su.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yx.521024.cn

[F03] 写入文件（覆盖）
来源：http://hq.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://td.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pz.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ne.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://me.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gp.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kw.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ls.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://oo.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oq.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kk.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sy.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ge.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://al.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bo.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kh.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lv.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://kz.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ky.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://yp.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://bx.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://hb.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gp.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eb.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://gc.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://nm.jianghongdianzi.cn

[F06] 删除文件
来源：http://mh.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://bb.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://ml.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mr.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sa.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xb.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://ew.colortex.cn

Ruby: File.delete("a.txt")
来源：http://lg.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://ig.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://ku.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sh.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xw.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vm.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hm.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dg.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sf.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gu.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ps.lnxyls.cn

[F08] 遍历目录
来源：http://bv.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gv.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pq.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://jl.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://it.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nh.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qu.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://dt.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://ee.bookmarksfly.cn

[F09] 获取文件大小
来源：http://ji.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://kh.nszjky.cn

PHP:  filesize("a.txt");
来源：http://pz.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://fq.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://rx.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mp.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fx.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://tq.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://nd.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://nz.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uj.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pe.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mr.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://hf.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gl.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ou.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nt.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zl.nicolike.cn

[F11] 复制与移动文件
来源：http://am.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kw.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bg.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tb.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fq.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jf.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wd.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gf.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hi.chemitech.net.cn

[F12] CSV 读写
来源：http://cn.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mv.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ni.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eh.newstarts.cn

TS:   // 同上
来源：http://sb.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xq.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bi.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hs.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ki.wgjwhj.cn

================================================================================
来源：http://dk.yuexingan06.cn

G. 面向对象
来源：http://yo.9csxet.cn

================================================================================
来源：http://ie.huixiangedu.cn

[G01] 定义类
来源：http://vh.szsharing.cn

Py:   class User: pass
来源：http://sk.shxzukj.cn

PHP:  class User {}
来源：http://hu.asd995.cn

JS:   class User {}
来源：http://bs.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://pt.521024.cn

Java: class User {}
来源：http://fv.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://qp.huixiangedu.cn

Ruby: class User; end
来源：http://eg.huanxung.cn

C#:   class User {}
来源：http://rx.szsharing.cn

[G02] 构造函数
来源：http://tt.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://qs.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://pm.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://mx.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://ek.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://py.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://is.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://jj.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://wl.chemitech.net.cn

[G03] 实例属性
来源：http://hb.hnjuh.cn

Py:   self.name = "x"
来源：http://ys.szsharing.cn

PHP:  public string $name = "x";
来源：http://ng.haigaiapp.cn

JS:   this.name = "x";
来源：http://xg.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://xf.lnxyls.cn

Java: private String name;
来源：http://vb.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hw.bjjhwx.cn

Ruby: @name = "x"
来源：http://bf.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://gy.yuexingan06.cn

[G04] 定义方法
来源：http://zd.hahajie.cn

Py:   def greet(self): return self.name
来源：http://tg.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fy.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://xa.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://yl.yuexingan06.cn

Java: String greet() { return name; }
来源：http://hp.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wn.nszjky.cn

Ruby: def greet; @name; end
来源：http://xx.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://lp.yuntaijiaju.cn

[G05] 继承
来源：http://vk.9csxet.cn

Py:   class Admin(User): pass
来源：http://na.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://wu.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://ie.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://bh.wgjwhj.cn

Java: class Admin extends User {}
来源：http://ul.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fd.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://pq.yuexingan06.cn

C#:   class Admin : User {}
来源：http://qi.nszjky.cn

[G06] 重写方法
来源：http://oh.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://sc.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ce.521024.cn

JS:   greet() { return "admin"; }
来源：http://gn.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://aq.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://ji.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hg.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://lx.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://vb.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://wt.muxihuayi.cn

Py:   super().greet()
来源：http://hb.szsharing.cn

PHP:  parent::greet();
来源：http://dp.gzmigu.cn

JS:   super.greet();
来源：http://te.jianghongdianzi.cn

TS:   super.greet();
来源：http://st.huixiangedu.cn

Java: super.greet();
来源：http://px.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bb.asd995.cn

Ruby: super
来源：http://yo.9csxet.cn

C#:   base.Greet();
来源：http://rk.9csxet.cn

[G08] 静态方法与属性
来源：http://aq.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xq.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://ev.yuexingan06.cn

JS:   static f() {}
来源：http://ei.lnxyls.cn

TS:   static f(): void {}
来源：http://ky.yuexingan06.cn

Java: static void f() {}
来源：http://sh.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vx.hnjuh.cn

Ruby: def self.f; end
来源：http://fv.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://bv.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://ck.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://wc.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dc.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bk.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://hn.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://bd.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://cg.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ic.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://dv.chemitech.net.cn

[G10] 访问控制
来源：http://ey.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://ko.newstarts.cn

PHP:  public / protected / private
来源：http://bd.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://fw.newstarts.cn

TS:   public / protected / private
来源：http://dr.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://ik.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rr.bjjhwx.cn

Ruby: public / protected / private
来源：http://ie.9csxet.cn

C#:   public / protected / private / internal
来源：http://pw.newstarts.cn

[G11] getter / setter
来源：http://au.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ml.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sm.asd995.cn

JS:   get name() { return this._name; }
来源：http://hj.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://gs.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://as.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cf.asd995.cn

Ruby: attr_accessor :name
来源：http://ty.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://of.hahajie.cn

[G12] 对象转字符串
来源：http://eg.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://lt.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bt.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://ga.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://da.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://df.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://op.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://eb.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://ho.huixiangedu.cn

[G13] 判断对象类型
来源：http://iv.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://my.nicolike.cn

PHP:  $u instanceof User
来源：http://yr.asd995.cn

JS:   u instanceof User
来源：http://jx.colortex.cn

TS:   u instanceof User
来源：http://to.nicolike.cn

Java: u instanceof User
来源：http://qn.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vw.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ms.panjiajie.cn

C#:   u is User
来源：http://yo.hnjuh.cn

[G14] 数据类 / record
来源：http://xo.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mm.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://xt.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://up.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://gj.9csxet.cn

Java: record User(String name, int age) {}
来源：http://hw.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://kb.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://az.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://jb.wgjwhj.cn

[G15] 枚举
来源：http://kn.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ek.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://do.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mf.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bi.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://ew.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uc.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://ua.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tu.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://im.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qt.521024.cn

PHP:  get_object_vars($obj);
来源：http://vg.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://gk.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://fr.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rv.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sp.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://yr.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://et.yuntaijiaju.cn

================================================================================
来源：http://gh.bjjhwx.cn

H. 异常与错误处理
来源：http://zk.panjiajie.cn

================================================================================
来源：http://mp.asd995.cn

[H01] try / catch 基础
来源：http://zd.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zj.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ez.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nx.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sy.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ss.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nl.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ry.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oe.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ja.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://si.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kg.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nb.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iw.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wg.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://um.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ah.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qd.asd995.cn

[H03] 主动抛出异常
来源：http://em.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://qh.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://no.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://bh.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://hq.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eu.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jj.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ry.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ae.bjjhwx.cn

[H04] 自定义异常类型
来源：http://um.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://hf.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://to.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://kk.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://er.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://gr.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qi.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://bd.colortex.cn

C#:   class MyException : Exception {}
来源：http://ro.asd995.cn

[H05] 捕获特定类型
来源：http://sh.szsharing.cn

Py:   except ValueError as e:
来源：http://gg.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zc.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://zq.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://hj.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://cs.muxihuayi.cn


<!-- 参考信息 -->