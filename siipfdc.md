代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yx.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vo.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://un.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://om.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://bi.9csxet.cn

[F02] 逐行读取文件
来源：http://hj.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pa.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ik.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://af.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qi.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xe.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sy.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wy.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ht.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ed.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ut.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hn.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xj.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uz.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://be.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qv.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ok.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xn.szxytkj.cn

[F04] 追加写入文件
来源：http://ak.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sm.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dh.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nn.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wl.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://li.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kb.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yq.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://td.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://jq.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nv.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://hf.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://rs.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://qx.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pz.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://on.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://hs.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://gz.shxzskj.cn

[F06] 删除文件
来源：http://fx.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://qo.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://ce.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zo.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qm.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qp.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://dx.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://pe.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://ij.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://lv.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://am.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ru.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ko.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fi.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ci.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rg.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yy.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ig.hahajie.cn

[F08] 遍历目录
来源：http://pq.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fq.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lo.521024.cn

JS:   fs.readdirSync("dir")
来源：http://rp.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://kt.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gg.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gb.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://ng.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://xn.chemitech.net.cn

[F09] 获取文件大小
来源：http://bn.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://st.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://rf.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://km.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://hv.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dx.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://od.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://ax.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://hx.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://so.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ni.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ru.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kv.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://mo.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://br.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vy.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qx.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://um.shtwfgs.cn

[F11] 复制与移动文件
来源：http://nt.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sp.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gn.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hb.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zb.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cd.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pn.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://su.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kd.9csxet.cn

[F12] CSV 读写
来源：http://lh.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ys.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dy.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gv.521024.cn

TS:   // 同上
来源：http://ih.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yf.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qr.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aq.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sb.yuntaijiaju.cn

================================================================================
来源：http://vo.muxihuayi.cn

G. 面向对象
来源：http://cy.huanxung.cn

================================================================================
来源：http://qo.bjjhwx.cn

[G01] 定义类
来源：http://ne.521024.cn

Py:   class User: pass
来源：http://xq.yuexingan06.cn

PHP:  class User {}
来源：http://pc.wgjwhj.cn

JS:   class User {}
来源：http://bk.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://vu.newstarts.cn

Java: class User {}
来源：http://bu.gzmigu.cn

Go:   type User struct { Name string }
来源：http://bk.muxihuayi.cn

Ruby: class User; end
来源：http://no.huixiangedu.cn

C#:   class User {}
来源：http://yu.muxihuayi.cn

[G02] 构造函数
来源：http://ud.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://pk.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://sg.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://wg.521024.cn

TS:   constructor(public name: string) {}
来源：http://jh.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://md.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qj.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://km.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://an.shxzukj.cn

[G03] 实例属性
来源：http://nk.huixiangedu.cn

Py:   self.name = "x"
来源：http://rk.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://gr.jctech888.com.cn

JS:   this.name = "x";
来源：http://fw.asd995.cn

TS:   name: string = "x";
来源：http://hs.muxihuayi.cn

Java: private String name;
来源：http://zj.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yv.9csxet.cn

Ruby: @name = "x"
来源：http://jw.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://aq.huixiangedu.cn

[G04] 定义方法
来源：http://vz.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://dx.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tu.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://se.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://ac.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://cl.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ap.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://fa.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://tu.bjjhwx.cn

[G05] 继承
来源：http://sz.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://or.nicolike.cn

PHP:  class Admin extends User {}
来源：http://ka.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://ax.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://tu.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://yc.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cw.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://zm.9csxet.cn

C#:   class Admin : User {}
来源：http://bf.gzmigu.cn

[G06] 重写方法
来源：http://tj.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://ma.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nm.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://wq.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://iu.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://tm.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xm.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://ft.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ow.panjiajie.cn

[G07] 调用父类方法
来源：http://ue.colortex.cn

Py:   super().greet()
来源：http://iz.lnxyls.cn

PHP:  parent::greet();
来源：http://ap.huixinmuqiang.cn

JS:   super.greet();
来源：http://od.szsharing.cn

TS:   super.greet();
来源：http://fr.szxytkj.cn

Java: super.greet();
来源：http://fq.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cz.shtwfgs.cn

Ruby: super
来源：http://xt.lnxyls.cn

C#:   base.Greet();
来源：http://lu.shxzukj.cn

[G08] 静态方法与属性
来源：http://xq.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xa.shxzukj.cn

PHP:  public static function f() {}
来源：http://wp.szxytkj.cn

JS:   static f() {}
来源：http://sx.yuexingan06.cn

TS:   static f(): void {}
来源：http://iv.yuntaijiaju.cn

Java: static void f() {}
来源：http://on.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hj.szsharing.cn

Ruby: def self.f; end
来源：http://ck.shtwfgs.cn

C#:   public static void F() {}
来源：http://vs.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://nt.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://gp.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tm.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zm.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://rn.huanxung.cn

Java: interface Shape { double area(); }
来源：http://fg.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ku.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wa.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://ai.521024.cn

[G10] 访问控制
来源：http://dc.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://fb.wgjwhj.cn

PHP:  public / protected / private
来源：http://ns.colortex.cn

JS:   #private 字段；其余公开
来源：http://kq.lnxyls.cn

TS:   public / protected / private
来源：http://au.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://nl.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gr.jctech888.com.cn

Ruby: public / protected / private
来源：http://oi.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://po.9csxet.cn

[G11] getter / setter
来源：http://uc.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://rg.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lp.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://om.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://vw.asd995.cn

Java: public String getName() { return name; }
来源：http://zb.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ej.panjiajie.cn

Ruby: attr_accessor :name
来源：http://xs.szsharing.cn

C#:   public string Name { get; set; }
来源：http://lv.shxzskj.cn

[G12] 对象转字符串
来源：http://mu.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://ln.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gc.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://yj.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://qm.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://xg.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cj.521024.cn

Ruby: def to_s; @name; end
来源：http://wq.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://un.colortex.cn

[G13] 判断对象类型
来源：http://xb.shxzukj.cn

Py:   isinstance(u, User)
来源：http://he.szsharing.cn

PHP:  $u instanceof User
来源：http://av.shtwfgs.cn

JS:   u instanceof User
来源：http://eo.asd995.cn

TS:   u instanceof User
来源：http://ww.lnxyls.cn

Java: u instanceof User
来源：http://pt.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fb.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://bl.hahajie.cn

C#:   u is User
来源：http://qc.gzmigu.cn

[G14] 数据类 / record
来源：http://pr.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jc.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://xx.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fs.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://us.9csxet.cn

Java: record User(String name, int age) {}
来源：http://gu.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://yh.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qn.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://ma.yuexingan06.cn

[G15] 枚举
来源：http://qt.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qh.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jz.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ps.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kl.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://bd.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tb.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://ac.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qz.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://yt.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wn.colortex.cn

PHP:  get_object_vars($obj);
来源：http://br.szxytkj.cn

JS:   Object.entries(obj)
来源：http://lo.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://sq.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sy.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ks.9csxet.cn

Ruby: obj.instance_variables
来源：http://fp.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://je.huixinmuqiang.cn

================================================================================
来源：http://oi.panjiajie.cn

H. 异常与错误处理
来源：http://vv.nszjky.cn

================================================================================
来源：http://mg.chemitech.net.cn

[H01] try / catch 基础
来源：http://oq.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bz.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ag.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ss.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://av.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ww.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zf.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uo.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mt.nicolike.cn

[H02] finally / ensure 收尾
来源：http://zj.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ct.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cf.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gc.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cx.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ms.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iw.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aa.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://el.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://pu.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://fg.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xb.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://fz.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://le.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dm.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://em.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://az.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mb.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://yx.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://jk.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vz.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://ae.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://bb.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://nj.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qb.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://sg.9csxet.cn

C#:   class MyException : Exception {}
来源：http://ai.shtwfgs.cn

[H05] 捕获特定类型
来源：http://fs.lnxyls.cn

Py:   except ValueError as e:
来源：http://wb.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rb.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://ul.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://lb.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://qo.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yr.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://oq.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uh.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://sf.bookmarksfly.cn


<!-- 参考信息 -->