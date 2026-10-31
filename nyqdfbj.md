代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oe.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ov.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://he.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://cu.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://fe.szxytkj.cn

[F02] 逐行读取文件
来源：http://we.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xp.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://se.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vo.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ta.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eh.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iw.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rr.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fc.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://uy.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rs.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zw.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ow.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yl.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zh.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wc.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://yo.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xj.bjjhwx.cn

[F04] 追加写入文件
来源：http://dp.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://of.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tu.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zd.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pq.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qg.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kg.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gc.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nr.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://rr.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jr.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://nt.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://lq.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://ci.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://av.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qe.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://ch.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://ve.bjjhwx.cn

[F06] 删除文件
来源：http://gg.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://nd.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://yz.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fq.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ck.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dw.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://ls.jianghongdianzi.cn

Ruby: File.delete("a.txt")
来源：http://eu.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://ue.nszjky.cn

[F07] 创建目录（含多级）
来源：http://xr.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fh.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gk.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ag.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://la.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nr.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yb.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uo.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kh.9csxet.cn

[F08] 遍历目录
来源：http://hh.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gz.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://og.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://bu.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://vg.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cr.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wt.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://pv.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://ui.lnxyls.cn

[F09] 获取文件大小
来源：http://sj.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://cb.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://gl.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://ju.muxihuayi.cn

TS:   fs.statSync("a.txt").size
来源：http://xe.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uf.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jh.szsharing.cn

Ruby: File.size("a.txt")
来源：http://cd.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://hh.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://yi.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ub.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ec.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fs.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://tc.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hl.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xy.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wa.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kl.hnjuh.cn

[F11] 复制与移动文件
来源：http://ar.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cg.521024.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fw.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://el.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ab.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mr.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://so.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wf.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fp.jctech888.com.cn

[F12] CSV 读写
来源：http://hn.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eq.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://th.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ss.huanxung.cn

TS:   // 同上
来源：http://kq.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://we.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ab.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sm.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://if.lnxyls.cn

================================================================================
来源：http://pt.chemitech.net.cn

G. 面向对象
来源：http://fg.nszjky.cn

================================================================================
来源：http://ku.yuexingan06.cn

[G01] 定义类
来源：http://nz.chemitech.net.cn

Py:   class User: pass
来源：http://pg.gzmigu.cn

PHP:  class User {}
来源：http://zi.huixiangedu.cn

JS:   class User {}
来源：http://ix.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://ci.asd995.cn

Java: class User {}
来源：http://ms.colortex.cn

Go:   type User struct { Name string }
来源：http://ta.nszjky.cn

Ruby: class User; end
来源：http://ic.haigaiapp.cn

C#:   class User {}
来源：http://yu.hahajie.cn

[G02] 构造函数
来源：http://wm.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://kq.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://yp.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://sr.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://mf.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://gv.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nw.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://sd.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://nd.521024.cn

[G03] 实例属性
来源：http://fl.shxzukj.cn

Py:   self.name = "x"
来源：http://db.szxytkj.cn

PHP:  public string $name = "x";
来源：http://is.muxihuayi.cn

JS:   this.name = "x";
来源：http://gd.hahajie.cn

TS:   name: string = "x";
来源：http://ff.huixiangedu.cn

Java: private String name;
来源：http://dd.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bc.panjiajie.cn

Ruby: @name = "x"
来源：http://nh.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://rw.newstarts.cn

[G04] 定义方法
来源：http://rw.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://mi.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ye.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://gs.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://yh.asd995.cn

Java: String greet() { return name; }
来源：http://ko.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qs.lnxyls.cn

Ruby: def greet; @name; end
来源：http://fw.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://pq.muxihuayi.cn

[G05] 继承
来源：http://fb.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://rk.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://fd.colortex.cn

JS:   class Admin extends User {}
来源：http://yp.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://jo.wgjwhj.cn

Java: class Admin extends User {}
来源：http://mr.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zd.asd995.cn

Ruby: class Admin < User; end
来源：http://yy.shtwfgs.cn

C#:   class Admin : User {}
来源：http://za.muxihuayi.cn

[G06] 重写方法
来源：http://ca.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://jj.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hv.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://og.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://pp.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://gk.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wm.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://kv.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://uz.huixiangedu.cn

[G07] 调用父类方法
来源：http://tx.bjjhwx.cn

Py:   super().greet()
来源：http://gw.gzmigu.cn

PHP:  parent::greet();
来源：http://rn.shxzskj.cn

JS:   super.greet();
来源：http://xi.colortex.cn

TS:   super.greet();
来源：http://jb.jctech888.com.cn

Java: super.greet();
来源：http://hk.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fz.huixinmuqiang.cn

Ruby: super
来源：http://dt.chemitech.net.cn

C#:   base.Greet();
来源：http://ld.haigaiapp.cn

[G08] 静态方法与属性
来源：http://ag.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ev.szsharing.cn

PHP:  public static function f() {}
来源：http://os.huixinmuqiang.cn

JS:   static f() {}
来源：http://fm.newstarts.cn

TS:   static f(): void {}
来源：http://qy.nicolike.cn

Java: static void f() {}
来源：http://eb.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ql.hahajie.cn

Ruby: def self.f; end
来源：http://ss.lnxyls.cn

C#:   public static void F() {}
来源：http://ni.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ik.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://dz.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://la.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wi.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://jd.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://rq.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://it.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ey.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://nf.nicolike.cn

[G10] 访问控制
来源：http://mv.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://er.szxytkj.cn

PHP:  public / protected / private
来源：http://bb.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://rr.haigaiapp.cn

TS:   public / protected / private
来源：http://uw.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://xe.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hv.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://gj.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://gz.panjiajie.cn

[G11] getter / setter
来源：http://lu.huanxung.cn

Py:   @property 与 @x.setter
来源：http://oy.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sk.szsharing.cn

JS:   get name() { return this._name; }
来源：http://rg.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://tf.szsharing.cn

Java: public String getName() { return name; }
来源：http://yk.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bg.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://iq.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://ni.huixiangedu.cn

[G12] 对象转字符串
来源：http://yz.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://rx.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ya.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://yk.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://fe.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://ri.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ol.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://jz.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://gh.gzmigu.cn

[G13] 判断对象类型
来源：http://sc.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://zo.jctech888.com.cn

PHP:  $u instanceof User
来源：http://rg.asd995.cn

JS:   u instanceof User
来源：http://oc.shxzukj.cn

TS:   u instanceof User
来源：http://qm.jctech888.com.cn

Java: u instanceof User
来源：http://pr.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ss.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://ei.hahajie.cn

C#:   u is User
来源：http://qj.lnxyls.cn

[G14] 数据类 / record
来源：http://od.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xu.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://iv.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ra.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://le.colortex.cn

Java: record User(String name, int age) {}
来源：http://gf.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://la.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://br.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://oa.hnjuh.cn

[G15] 枚举
来源：http://dn.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nk.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cr.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fp.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dw.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://vf.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qp.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://tu.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sm.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://dp.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zn.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://fk.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://gw.lnxyls.cn

TS:   Object.entries(obj)
来源：http://dc.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rx.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gu.newstarts.cn

Ruby: obj.instance_variables
来源：http://wi.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://hf.yuntaijiaju.cn

================================================================================
来源：http://sd.haigaiapp.cn

H. 异常与错误处理
来源：http://sz.huanxung.cn

================================================================================
来源：http://st.colortex.cn

[H01] try / catch 基础
来源：http://uv.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ka.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mg.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ow.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bc.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ac.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kb.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ix.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cr.9csxet.cn

[H02] finally / ensure 收尾
来源：http://wx.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fu.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ns.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tt.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cf.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qy.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ta.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://he.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://py.haigaiapp.cn

[H03] 主动抛出异常
来源：http://jv.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://xg.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oy.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://ti.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://kl.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cp.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://em.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hl.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ff.521024.cn

[H04] 自定义异常类型
来源：http://yk.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://nm.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://he.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://wz.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://cg.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://dp.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ac.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://zv.asd995.cn

C#:   class MyException : Exception {}
来源：http://tg.newstarts.cn

[H05] 捕获特定类型
来源：http://si.huixiangedu.cn

Py:   except ValueError as e:
来源：http://dz.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wr.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://sv.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://ko.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://rx.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ot.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://cq.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ol.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://yn.panjiajie.cn


<!-- 参考信息 -->