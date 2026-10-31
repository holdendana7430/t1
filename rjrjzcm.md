代发 wailian999

[F01] 读取整个文件
来源：http://rz.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ge.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://uq.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pu.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zx.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ke.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cv.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://vu.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://yj.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://rh.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pn.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nt.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cj.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sq.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xs.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pz.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hr.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sg.asd995.cn

[F03] 写入文件（覆盖）
来源：http://un.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yv.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vy.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pd.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ak.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tt.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://if.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://xt.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hn.nszjky.cn

[F04] 追加写入文件
来源：http://sr.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hd.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ok.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uq.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yz.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://id.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wg.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lk.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dg.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://iu.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vg.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://yr.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://fe.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://yq.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tu.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nh.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://hu.521024.cn

C#:   File.Exists("a.txt")
来源：http://xp.haigaiapp.cn

[F06] 删除文件
来源：http://uk.colortex.cn

Py:   os.remove("a.txt")
来源：http://co.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://ow.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fa.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jo.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://br.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://ma.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://iw.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://dv.hahajie.cn

[F07] 创建目录（含多级）
来源：http://vk.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dr.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qj.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fc.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pp.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dk.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gp.muxihuayi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sc.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://et.shtwfgs.cn

[F08] 遍历目录
来源：http://hv.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://to.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uf.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://iw.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://po.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oc.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yh.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://xf.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://ak.muxihuayi.cn

[F09] 获取文件大小
来源：http://vh.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://mf.asd995.cn

PHP:  filesize("a.txt");
来源：http://pm.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://oc.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://am.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vy.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aw.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://jx.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://ed.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://ou.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ok.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xp.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nz.nszjky.cn

TS:   path.extname("a.txt")
来源：http://lm.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dm.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zi.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ho.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fl.521024.cn

[F11] 复制与移动文件
来源：http://nb.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uk.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://du.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ye.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rc.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ds.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lo.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qd.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zj.jianghongdianzi.cn

[F12] CSV 读写
来源：http://kn.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ng.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://na.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ps.lnxyls.cn

TS:   // 同上
来源：http://tm.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fw.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ym.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://po.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pr.newstarts.cn

================================================================================
来源：http://uw.lnxyls.cn

G. 面向对象
来源：http://la.9csxet.cn

================================================================================
来源：http://hu.huanxung.cn

[G01] 定义类
来源：http://si.yuntaijiaju.cn

Py:   class User: pass
来源：http://eq.bjjhwx.cn

PHP:  class User {}
来源：http://ne.huanxung.cn

JS:   class User {}
来源：http://uy.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://we.wgjwhj.cn

Java: class User {}
来源：http://gc.panjiajie.cn

Go:   type User struct { Name string }
来源：http://sw.lnxyls.cn

Ruby: class User; end
来源：http://yx.9csxet.cn

C#:   class User {}
来源：http://qt.huixinmuqiang.cn

[G02] 构造函数
来源：http://cv.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ec.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://al.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://jg.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://lx.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://au.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oj.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://jb.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://xm.colortex.cn

[G03] 实例属性
来源：http://st.bookmarksfly.cn

Py:   self.name = "x"
来源：http://yh.nszjky.cn

PHP:  public string $name = "x";
来源：http://vu.shxzukj.cn

JS:   this.name = "x";
来源：http://ac.hnjuh.cn

TS:   name: string = "x";
来源：http://rx.wgjwhj.cn

Java: private String name;
来源：http://df.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zi.shxzskj.cn

Ruby: @name = "x"
来源：http://lv.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://rx.lnxyls.cn

[G04] 定义方法
来源：http://ev.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://yp.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iq.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://qc.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://bz.nicolike.cn

Java: String greet() { return name; }
来源：http://ys.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lo.nszjky.cn

Ruby: def greet; @name; end
来源：http://ww.nszjky.cn

C#:   public string Greet() => Name;
来源：http://eo.szxytkj.cn

[G05] 继承
来源：http://sg.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://fa.asd995.cn

PHP:  class Admin extends User {}
来源：http://sv.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://nv.nicolike.cn

TS:   class Admin extends User {}
来源：http://ba.hnjuh.cn

Java: class Admin extends User {}
来源：http://vl.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dz.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://pn.szsharing.cn

C#:   class Admin : User {}
来源：http://nf.shtwfgs.cn

[G06] 重写方法
来源：http://tv.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://mo.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pw.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://ck.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://fi.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://lb.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mf.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://go.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://xh.bjjhwx.cn

[G07] 调用父类方法
来源：http://zb.nszjky.cn

Py:   super().greet()
来源：http://my.szxytkj.cn

PHP:  parent::greet();
来源：http://nj.gzmigu.cn

JS:   super.greet();
来源：http://mj.newstarts.cn

TS:   super.greet();
来源：http://qz.szsharing.cn

Java: super.greet();
来源：http://vk.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ab.muxihuayi.cn

Ruby: super
来源：http://ky.nszjky.cn

C#:   base.Greet();
来源：http://wk.9csxet.cn

[G08] 静态方法与属性
来源：http://hw.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jf.hahajie.cn

PHP:  public static function f() {}
来源：http://ib.hahajie.cn

JS:   static f() {}
来源：http://if.shxzskj.cn

TS:   static f(): void {}
来源：http://sk.hahajie.cn

Java: static void f() {}
来源：http://tw.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://de.wgjwhj.cn

Ruby: def self.f; end
来源：http://pt.bookmarksfly.cn

C#:   public static void F() {}
来源：http://ej.szsharing.cn

[G09] 接口 / 抽象类
来源：http://nr.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://jp.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bs.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wx.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://kr.nszjky.cn

Java: interface Shape { double area(); }
来源：http://rs.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://if.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hl.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://jk.jianghongdianzi.cn

[G10] 访问控制
来源：http://od.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://wm.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://gn.asd995.cn

JS:   #private 字段；其余公开
来源：http://wq.colortex.cn

TS:   public / protected / private
来源：http://nq.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://cf.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bl.szxytkj.cn

Ruby: public / protected / private
来源：http://kp.lnxyls.cn

C#:   public / protected / private / internal
来源：http://jk.bookmarksfly.cn

[G11] getter / setter
来源：http://ul.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://xj.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ck.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://gf.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ct.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://hh.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wd.shxzskj.cn

Ruby: attr_accessor :name
来源：http://ek.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://am.hnjuh.cn

[G12] 对象转字符串
来源：http://mw.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://uq.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://os.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://uu.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://nz.521024.cn

Java: @Override public String toString() { return name; }
来源：http://du.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gw.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ru.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://wc.shxzskj.cn

[G13] 判断对象类型
来源：http://cs.shxzskj.cn

Py:   isinstance(u, User)
来源：http://yn.huixiangedu.cn

PHP:  $u instanceof User
来源：http://xn.hnjuh.cn

JS:   u instanceof User
来源：http://uu.lnxyls.cn

TS:   u instanceof User
来源：http://qi.haigaiapp.cn

Java: u instanceof User
来源：http://os.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oi.colortex.cn

Ruby: u.is_a?(User)
来源：http://hs.nszjky.cn

C#:   u is User
来源：http://xp.521024.cn

[G14] 数据类 / record
来源：http://qj.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://re.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://xi.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yr.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://ab.szsharing.cn

Java: record User(String name, int age) {}
来源：http://ht.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://bs.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zm.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://di.haigaiapp.cn

[G15] 枚举
来源：http://tz.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uo.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fg.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://on.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rp.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://ph.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pd.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://hz.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pj.asd995.cn

[G16] 对象转数组 / 字典
来源：http://id.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sf.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://us.panjiajie.cn

JS:   Object.entries(obj)
来源：http://ik.colortex.cn

TS:   Object.entries(obj)
来源：http://lq.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lu.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zl.hnjuh.cn

Ruby: obj.instance_variables
来源：http://sn.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ui.huanxung.cn

================================================================================
来源：http://pe.huixinmuqiang.cn

H. 异常与错误处理
来源：http://pd.9csxet.cn

================================================================================
来源：http://hs.newstarts.cn

[H01] try / catch 基础
来源：http://vy.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xa.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cf.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fe.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lz.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rq.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fe.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zu.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aw.nszjky.cn

[H02] finally / ensure 收尾
来源：http://gs.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tf.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xp.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ou.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mx.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hl.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ax.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xl.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gg.panjiajie.cn

[H03] 主动抛出异常
来源：http://rn.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://rh.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rf.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://fq.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://lm.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dt.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ux.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ty.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dg.colortex.cn

[H04] 自定义异常类型
来源：http://em.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://ow.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gt.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://ee.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://zj.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://uf.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yp.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://kp.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://ip.nszjky.cn

[H05] 捕获特定类型
来源：http://pj.wgjwhj.cn

Py:   except ValueError as e:
来源：http://pl.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bd.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://cx.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://an.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://me.chemitech.net.cn


<!-- 参考信息 -->