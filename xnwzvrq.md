代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iq.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dy.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yo.colortex.cn

Ruby: File.read("a.txt")
来源：http://pq.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://nz.huixiangedu.cn

[F02] 逐行读取文件
来源：http://ob.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://he.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jk.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qq.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wi.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://su.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://co.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jh.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jf.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://ok.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gm.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://su.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pl.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sp.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yt.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uy.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://mn.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ft.szsharing.cn

[F04] 追加写入文件
来源：http://xk.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cf.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ch.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nd.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qr.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zx.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ul.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vf.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xt.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://ly.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ux.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://dt.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://rn.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://na.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mc.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ld.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://rj.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://ds.shxzukj.cn

[F06] 删除文件
来源：http://mb.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://wo.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://gb.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fk.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hk.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://de.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://ac.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://pv.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ki.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://av.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jj.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qc.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ri.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ys.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pl.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fz.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ik.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cs.shxzskj.cn

[F08] 遍历目录
来源：http://xw.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cr.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bt.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://hv.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://dj.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bo.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://np.huanxung.cn

Ruby: Dir.children("dir")
来源：http://zk.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://bd.nicolike.cn

[F09] 获取文件大小
来源：http://zz.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://nr.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://nu.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://fh.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://uw.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zn.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mb.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://ib.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://me.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://xj.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nf.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://is.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://be.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://jw.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fj.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qf.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fm.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dg.colortex.cn

[F11] 复制与移动文件
来源：http://js.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pf.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jb.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hr.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uz.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aj.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kz.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rl.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bh.hahajie.cn

[F12] CSV 读写
来源：http://rp.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://do.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bs.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bu.hahajie.cn

TS:   // 同上
来源：http://kr.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ia.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hb.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nk.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jv.haigaiapp.cn

================================================================================
来源：http://qi.jctech888.com.cn

G. 面向对象
来源：http://ki.panjiajie.cn

================================================================================
来源：http://bd.muxihuayi.cn

[G01] 定义类
来源：http://ip.colortex.cn

Py:   class User: pass
来源：http://id.bjjhwx.cn

PHP:  class User {}
来源：http://eu.jianghongdianzi.cn

JS:   class User {}
来源：http://vn.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://fw.gzmigu.cn

Java: class User {}
来源：http://uy.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://sy.521024.cn

Ruby: class User; end
来源：http://fb.szsharing.cn

C#:   class User {}
来源：http://oj.bookmarksfly.cn

[G02] 构造函数
来源：http://uv.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://kx.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://hd.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://oh.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://tb.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://on.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rj.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ow.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://ne.hahajie.cn

[G03] 实例属性
来源：http://ct.521024.cn

Py:   self.name = "x"
来源：http://pt.panjiajie.cn

PHP:  public string $name = "x";
来源：http://km.521024.cn

JS:   this.name = "x";
来源：http://jg.shtwfgs.cn

TS:   name: string = "x";
来源：http://wk.asd995.cn

Java: private String name;
来源：http://bi.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wi.hahajie.cn

Ruby: @name = "x"
来源：http://pq.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://cn.yuexingan06.cn

[G04] 定义方法
来源：http://za.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://si.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yr.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://wq.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://dj.szsharing.cn

Java: String greet() { return name; }
来源：http://uc.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wy.colortex.cn

Ruby: def greet; @name; end
来源：http://eo.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://ec.hnjuh.cn

[G05] 继承
来源：http://so.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://mh.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://tb.lnxyls.cn

JS:   class Admin extends User {}
来源：http://zw.nicolike.cn

TS:   class Admin extends User {}
来源：http://jy.nicolike.cn

Java: class Admin extends User {}
来源：http://ds.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jw.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://ou.nszjky.cn

C#:   class Admin : User {}
来源：http://rj.szsharing.cn

[G06] 重写方法
来源：http://tq.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://er.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wk.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://qr.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://ze.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://wb.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jr.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://uq.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://lm.gzmigu.cn

[G07] 调用父类方法
来源：http://xl.muxihuayi.cn

Py:   super().greet()
来源：http://md.shxzskj.cn

PHP:  parent::greet();
来源：http://wv.jianghongdianzi.cn

JS:   super.greet();
来源：http://no.huixiangedu.cn

TS:   super.greet();
来源：http://vg.szxytkj.cn

Java: super.greet();
来源：http://or.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vj.huanxung.cn

Ruby: super
来源：http://dq.nicolike.cn

C#:   base.Greet();
来源：http://mo.chemitech.net.cn

[G08] 静态方法与属性
来源：http://nf.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ho.9csxet.cn

PHP:  public static function f() {}
来源：http://uj.hnjuh.cn

JS:   static f() {}
来源：http://oj.hahajie.cn

TS:   static f(): void {}
来源：http://wn.huixinmuqiang.cn

Java: static void f() {}
来源：http://nv.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nv.hnjuh.cn

Ruby: def self.f; end
来源：http://tz.nicolike.cn

C#:   public static void F() {}
来源：http://cu.newstarts.cn

[G09] 接口 / 抽象类
来源：http://oo.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://cs.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vn.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hq.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://ti.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://tn.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ay.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://by.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://ao.asd995.cn

[G10] 访问控制
来源：http://ic.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://gj.lnxyls.cn

PHP:  public / protected / private
来源：http://gv.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://nw.muxihuayi.cn

TS:   public / protected / private
来源：http://oe.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://iw.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lv.gzmigu.cn

Ruby: public / protected / private
来源：http://yt.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://au.9csxet.cn

[G11] getter / setter
来源：http://sm.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://wc.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://km.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://mx.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://ja.szsharing.cn

Java: public String getName() { return name; }
来源：http://el.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hq.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://kt.nszjky.cn

C#:   public string Name { get; set; }
来源：http://tt.9csxet.cn

[G12] 对象转字符串
来源：http://cx.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://tm.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mx.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://bp.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://dv.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://vq.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gj.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://bv.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://nm.shxzukj.cn

[G13] 判断对象类型
来源：http://si.521024.cn

Py:   isinstance(u, User)
来源：http://tb.asd995.cn

PHP:  $u instanceof User
来源：http://bs.huanxung.cn

JS:   u instanceof User
来源：http://nl.huixiangedu.cn

TS:   u instanceof User
来源：http://kp.wgjwhj.cn

Java: u instanceof User
来源：http://bk.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gz.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://vr.jianghongdianzi.cn

C#:   u is User
来源：http://as.hnjuh.cn

[G14] 数据类 / record
来源：http://kj.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oy.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://bx.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hx.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://xk.asd995.cn

Java: record User(String name, int age) {}
来源：http://ud.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://au.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fy.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://cb.shtwfgs.cn

[G15] 枚举
来源：http://ap.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://es.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uc.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bf.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qv.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://st.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zo.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://zj.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ia.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://mo.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nv.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://oa.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://ao.nszjky.cn

TS:   Object.entries(obj)
来源：http://if.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ma.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hi.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://in.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://dw.shxzukj.cn

================================================================================
来源：http://jr.huixiangedu.cn

H. 异常与错误处理
来源：http://ob.huanxung.cn

================================================================================
来源：http://ug.shxzukj.cn

[H01] try / catch 基础
来源：http://gr.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rz.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cy.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lc.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lv.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ga.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yp.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eq.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pd.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://yj.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ef.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ss.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xv.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fe.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zt.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nv.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dk.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eh.chemitech.net.cn

[H03] 主动抛出异常
来源：http://hl.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://pn.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vl.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://li.asd995.cn

TS:   throw new Error("错误信息");
来源：http://ei.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://en.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ja.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://af.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hv.nicolike.cn

[H04] 自定义异常类型
来源：http://gw.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://gw.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nl.asd995.cn

JS:   class MyError extends Error {}
来源：http://ce.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://vl.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://ek.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tv.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://vt.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://lg.shxzukj.cn

[H05] 捕获特定类型
来源：http://yp.huixiangedu.cn

Py:   except ValueError as e:
来源：http://iz.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://si.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://yj.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://fp.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://jq.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tl.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://yt.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kh.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://bm.gzmigu.cn


<!-- 参考信息 -->