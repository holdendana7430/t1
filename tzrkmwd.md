代发 wailian999

[F01] 读取整个文件
来源：http://mg.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://st.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://ld.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pk.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pv.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jl.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hc.colortex.cn

Ruby: File.read("a.txt")
来源：http://jm.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://yp.chemitech.net.cn

[F02] 逐行读取文件
来源：http://ax.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yp.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://er.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ot.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yk.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lp.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ka.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wj.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ei.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://rl.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cw.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yd.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kx.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ks.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ik.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kf.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ox.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rh.shxzskj.cn

[F04] 追加写入文件
来源：http://tc.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jf.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cl.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zf.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ps.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uw.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qg.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sc.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ap.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://gb.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yj.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://su.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://ok.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://pr.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://py.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://te.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://lf.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://jq.wgjwhj.cn

[F06] 删除文件
来源：http://im.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://ji.nicolike.cn

PHP:  unlink("a.txt");
来源：http://nk.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aw.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dj.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sc.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://nd.521024.cn

Ruby: File.delete("a.txt")
来源：http://ks.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://yd.colortex.cn

[F07] 创建目录（含多级）
来源：http://by.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://la.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zi.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kk.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ay.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tz.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cy.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vb.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oe.lnxyls.cn

[F08] 遍历目录
来源：http://rl.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ra.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ti.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://jt.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://ak.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lq.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yb.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://up.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://qx.asd995.cn

[F09] 获取文件大小
来源：http://wy.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://nj.huanxung.cn

PHP:  filesize("a.txt");
来源：http://fh.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://qc.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://ud.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://on.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jk.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://vf.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://zq.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://po.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://da.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zy.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sr.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://za.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ln.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zy.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ki.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ip.nszjky.cn

[F11] 复制与移动文件
来源：http://zr.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kr.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wj.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xe.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pw.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vd.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ju.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zz.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gb.newstarts.cn

[F12] CSV 读写
来源：http://xm.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wl.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ji.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qb.huanxung.cn

TS:   // 同上
来源：http://hl.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cq.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bb.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xk.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zm.nszjky.cn

================================================================================
来源：http://wr.jianghongdianzi.cn

G. 面向对象
来源：http://vf.huixinmuqiang.cn

================================================================================
来源：http://yb.bookmarksfly.cn

[G01] 定义类
来源：http://ra.muxihuayi.cn

Py:   class User: pass
来源：http://bo.newstarts.cn

PHP:  class User {}
来源：http://yf.521024.cn

JS:   class User {}
来源：http://cz.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://fl.nicolike.cn

Java: class User {}
来源：http://am.shxzukj.cn

Go:   type User struct { Name string }
来源：http://zh.nicolike.cn

Ruby: class User; end
来源：http://av.nszjky.cn

C#:   class User {}
来源：http://jz.szxytkj.cn

[G02] 构造函数
来源：http://zm.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://mn.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://qc.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://nr.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://wv.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://wm.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qm.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ce.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://la.huixinmuqiang.cn

[G03] 实例属性
来源：http://pi.panjiajie.cn

Py:   self.name = "x"
来源：http://zj.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://dk.jctech888.com.cn

JS:   this.name = "x";
来源：http://ld.nicolike.cn

TS:   name: string = "x";
来源：http://hs.hnjuh.cn

Java: private String name;
来源：http://vk.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zj.colortex.cn

Ruby: @name = "x"
来源：http://db.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://yx.shxzukj.cn

[G04] 定义方法
来源：http://mm.asd995.cn

Py:   def greet(self): return self.name
来源：http://ta.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kx.521024.cn

JS:   greet() { return this.name; }
来源：http://wd.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://mf.panjiajie.cn

Java: String greet() { return name; }
来源：http://hz.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rv.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://dj.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://dd.huixinmuqiang.cn

[G05] 继承
来源：http://pk.newstarts.cn

Py:   class Admin(User): pass
来源：http://gh.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://we.nszjky.cn

JS:   class Admin extends User {}
来源：http://am.szsharing.cn

TS:   class Admin extends User {}
来源：http://zw.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://gw.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fx.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://dj.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://ce.szsharing.cn

[G06] 重写方法
来源：http://ik.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://ka.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pl.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://ze.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://wr.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://ed.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ww.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://nh.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://ba.asd995.cn

[G07] 调用父类方法
来源：http://yy.yuexingan06.cn

Py:   super().greet()
来源：http://rt.521024.cn

PHP:  parent::greet();
来源：http://nf.yuexingan06.cn

JS:   super.greet();
来源：http://wl.shxzskj.cn

TS:   super.greet();
来源：http://yp.gzmigu.cn

Java: super.greet();
来源：http://pd.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wz.9csxet.cn

Ruby: super
来源：http://wz.nicolike.cn

C#:   base.Greet();
来源：http://va.szsharing.cn

[G08] 静态方法与属性
来源：http://pb.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ao.521024.cn

PHP:  public static function f() {}
来源：http://oo.gzmigu.cn

JS:   static f() {}
来源：http://pe.szsharing.cn

TS:   static f(): void {}
来源：http://bs.nszjky.cn

Java: static void f() {}
来源：http://gw.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mo.hnjuh.cn

Ruby: def self.f; end
来源：http://wa.hahajie.cn

C#:   public static void F() {}
来源：http://uq.szsharing.cn

[G09] 接口 / 抽象类
来源：http://cc.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://yg.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xx.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bj.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ad.hahajie.cn

Java: interface Shape { double area(); }
来源：http://st.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://jf.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ex.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://zy.nicolike.cn

[G10] 访问控制
来源：http://ai.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://tu.jctech888.com.cn

PHP:  public / protected / private
来源：http://lo.hahajie.cn

JS:   #private 字段；其余公开
来源：http://xk.chemitech.net.cn

TS:   public / protected / private
来源：http://nn.colortex.cn

Java: public / protected / private / 默认包级
来源：http://ja.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pp.9csxet.cn

Ruby: public / protected / private
来源：http://iq.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://ld.haigaiapp.cn

[G11] getter / setter
来源：http://jr.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://jc.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tc.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://rj.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://yz.szxytkj.cn

Java: public String getName() { return name; }
来源：http://cr.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gz.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://im.nszjky.cn

C#:   public string Name { get; set; }
来源：http://zc.lnxyls.cn

[G12] 对象转字符串
来源：http://ra.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://md.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lx.hahajie.cn

JS:   toString() { return this.name; }
来源：http://mb.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://sb.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://di.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cg.asd995.cn

Ruby: def to_s; @name; end
来源：http://kj.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://wc.szsharing.cn

[G13] 判断对象类型
来源：http://yz.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://ox.huixiangedu.cn

PHP:  $u instanceof User
来源：http://ce.huixinmuqiang.cn

JS:   u instanceof User
来源：http://al.huixinmuqiang.cn

TS:   u instanceof User
来源：http://se.jianghongdianzi.cn

Java: u instanceof User
来源：http://ck.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yy.newstarts.cn

Ruby: u.is_a?(User)
来源：http://yu.jianghongdianzi.cn

C#:   u is User
来源：http://mo.wgjwhj.cn

[G14] 数据类 / record
来源：http://cd.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vh.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://cl.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ft.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://kw.newstarts.cn

Java: record User(String name, int age) {}
来源：http://gh.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://ep.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dv.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://sw.lnxyls.cn

[G15] 枚举
来源：http://rr.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nb.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kz.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hr.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cd.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://vu.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oq.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://ky.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vm.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://iq.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dv.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://lk.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://qi.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://fm.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jp.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mk.gzmigu.cn

Ruby: obj.instance_variables
来源：http://cq.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://ir.muxihuayi.cn

================================================================================
来源：http://cz.haigaiapp.cn

H. 异常与错误处理
来源：http://wv.yuexingan06.cn

================================================================================
来源：http://yp.huanxung.cn

[H01] try / catch 基础
来源：http://bi.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ho.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vk.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ww.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zg.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wa.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://el.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eg.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ks.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://oi.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uu.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ni.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ck.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zp.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://we.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gk.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hh.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://al.shxzskj.cn

[H03] 主动抛出异常
来源：http://zu.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://ts.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zj.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://fn.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://mu.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rg.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ya.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://os.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yh.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://uy.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://vh.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nw.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://vb.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://ce.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://nb.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mn.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://rz.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://fb.521024.cn

[H05] 捕获特定类型
来源：http://uu.szxytkj.cn

Py:   except ValueError as e:
来源：http://fj.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lr.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://lf.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://sd.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://oh.haigaiapp.cn


<!-- 参考信息 -->