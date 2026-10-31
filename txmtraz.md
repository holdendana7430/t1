代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vw.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sz.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jb.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oi.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://cp.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ay.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://qj.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://lp.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://jy.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pl.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ek.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://gu.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://qd.huanxung.cn

[F06] 删除文件
来源：http://sd.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://lb.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://ik.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qi.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lm.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://se.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://bu.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://fq.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://dn.asd995.cn

[F07] 创建目录（含多级）
来源：http://dh.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qm.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vh.asd995.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://js.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ne.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zh.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://au.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ln.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://me.huixiangedu.cn

[F08] 遍历目录
来源：http://rh.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lp.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ey.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://my.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://zk.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dw.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iz.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://vl.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://tq.huixiangedu.cn

[F09] 获取文件大小
来源：http://ue.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://ow.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://ih.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://vj.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://wj.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ih.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xy.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://ff.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://lm.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://cx.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cy.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://do.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hr.hahajie.cn

TS:   path.extname("a.txt")
来源：http://lm.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zh.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ju.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bq.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cy.chemitech.net.cn

[F11] 复制与移动文件
来源：http://ct.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://di.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zv.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rq.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://he.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ps.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nk.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nh.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bm.asd995.cn

[F12] CSV 读写
来源：http://mm.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uq.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lo.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vf.jctech888.com.cn

TS:   // 同上
来源：http://ak.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bs.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ol.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dm.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hf.bookmarksfly.cn

================================================================================
来源：http://is.wgjwhj.cn

G. 面向对象
来源：http://rc.wgjwhj.cn

================================================================================
来源：http://lt.nicolike.cn

[G01] 定义类
来源：http://zc.hnjuh.cn

Py:   class User: pass
来源：http://gt.lnxyls.cn

PHP:  class User {}
来源：http://ss.huixinmuqiang.cn

JS:   class User {}
来源：http://nu.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://im.huixinmuqiang.cn

Java: class User {}
来源：http://fi.hnjuh.cn

Go:   type User struct { Name string }
来源：http://jw.huanxung.cn

Ruby: class User; end
来源：http://fz.asd995.cn

C#:   class User {}
来源：http://by.9csxet.cn

[G02] 构造函数
来源：http://hb.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://hk.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://sd.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://cu.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://pw.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://wn.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ln.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://dy.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://gk.lnxyls.cn

[G03] 实例属性
来源：http://qa.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://wc.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://cz.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://ep.newstarts.cn

TS:   name: string = "x";
来源：http://ff.newstarts.cn

Java: private String name;
来源：http://fv.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cy.gzmigu.cn

Ruby: @name = "x"
来源：http://po.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://no.szxytkj.cn

[G04] 定义方法
来源：http://wg.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://rm.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jj.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://gl.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://op.shtwfgs.cn

Java: String greet() { return name; }
来源：http://fg.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oe.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://dc.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://vk.shtwfgs.cn

[G05] 继承
来源：http://zc.shxzskj.cn

Py:   class Admin(User): pass
来源：http://fd.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://lx.shxzukj.cn

JS:   class Admin extends User {}
来源：http://sw.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://vj.shtwfgs.cn

Java: class Admin extends User {}
来源：http://pb.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rm.panjiajie.cn

Ruby: class Admin < User; end
来源：http://dy.haigaiapp.cn

C#:   class Admin : User {}
来源：http://ue.jctech888.com.cn

[G06] 重写方法
来源：http://is.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://lj.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://on.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://ud.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://oq.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://ny.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kj.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://eo.521024.cn

C#:   public override string Greet() => "admin";
来源：http://so.colortex.cn

[G07] 调用父类方法
来源：http://ea.yuexingan06.cn

Py:   super().greet()
来源：http://nj.bjjhwx.cn

PHP:  parent::greet();
来源：http://dd.nszjky.cn

JS:   super.greet();
来源：http://am.huixinmuqiang.cn

TS:   super.greet();
来源：http://aw.bookmarksfly.cn

Java: super.greet();
来源：http://oc.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lx.newstarts.cn

Ruby: super
来源：http://pe.haigaiapp.cn

C#:   base.Greet();
来源：http://zn.newstarts.cn

[G08] 静态方法与属性
来源：http://am.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ji.nicolike.cn

PHP:  public static function f() {}
来源：http://sc.wgjwhj.cn

JS:   static f() {}
来源：http://mh.wgjwhj.cn

TS:   static f(): void {}
来源：http://rk.gzmigu.cn

Java: static void f() {}
来源：http://cz.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jt.gzmigu.cn

Ruby: def self.f; end
来源：http://tn.muxihuayi.cn

C#:   public static void F() {}
来源：http://gj.colortex.cn

[G09] 接口 / 抽象类
来源：http://jc.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://dn.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ga.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tu.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://aq.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://jp.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://jb.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wg.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://wb.nszjky.cn

[G10] 访问控制
来源：http://vs.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://vp.bjjhwx.cn

PHP:  public / protected / private
来源：http://mm.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://yx.asd995.cn

TS:   public / protected / private
来源：http://bk.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://xa.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ha.huixiangedu.cn

Ruby: public / protected / private
来源：http://mz.nicolike.cn

C#:   public / protected / private / internal
来源：http://uf.huixinmuqiang.cn

[G11] getter / setter
来源：http://kc.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://fq.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ka.asd995.cn

JS:   get name() { return this._name; }
来源：http://dt.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://wy.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://au.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://an.shxzukj.cn

Ruby: attr_accessor :name
来源：http://qs.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ib.huanxung.cn

[G12] 对象转字符串
来源：http://an.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://xi.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ch.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://zb.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://gf.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://ay.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ud.9csxet.cn

Ruby: def to_s; @name; end
来源：http://rz.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://zq.chemitech.net.cn

[G13] 判断对象类型
来源：http://wd.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://vo.yuexingan06.cn

PHP:  $u instanceof User
来源：http://mk.521024.cn

JS:   u instanceof User
来源：http://cq.bjjhwx.cn

TS:   u instanceof User
来源：http://te.panjiajie.cn

Java: u instanceof User
来源：http://if.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rx.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://lk.huixiangedu.cn

C#:   u is User
来源：http://yv.nszjky.cn

[G14] 数据类 / record
来源：http://xs.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ro.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://ti.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mh.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://no.521024.cn

Java: record User(String name, int age) {}
来源：http://yg.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://ij.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ah.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://rp.hahajie.cn

[G15] 枚举
来源：http://au.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xz.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xv.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rf.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ap.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://mc.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tv.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://ln.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bh.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://fd.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vw.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://vz.9csxet.cn

JS:   Object.entries(obj)
来源：http://lr.newstarts.cn

TS:   Object.entries(obj)
来源：http://cz.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gz.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://od.szsharing.cn

Ruby: obj.instance_variables
来源：http://jt.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://bz.wgjwhj.cn

================================================================================
来源：http://td.szxytkj.cn

H. 异常与错误处理
来源：http://ta.bjjhwx.cn

================================================================================
来源：http://kz.szxytkj.cn

[H01] try / catch 基础
来源：http://hb.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mu.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fs.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pd.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://po.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kd.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fz.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hq.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ht.nszjky.cn

[H02] finally / ensure 收尾
来源：http://eh.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qf.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://is.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yq.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vh.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zp.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nh.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fh.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gi.shxzskj.cn

[H03] 主动抛出异常
来源：http://rn.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://po.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lo.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://uc.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://yc.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nf.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lb.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xn.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ni.haigaiapp.cn

[H04] 自定义异常类型
来源：http://bc.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://ke.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vw.nicolike.cn

JS:   class MyError extends Error {}
来源：http://ca.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://af.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://bi.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qj.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://xi.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://nn.wgjwhj.cn

[H05] 捕获特定类型
来源：http://ul.9csxet.cn

Py:   except ValueError as e:
来源：http://ww.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://it.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://rz.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://rr.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://vi.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rr.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://cd.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wm.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://lq.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://pg.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://in.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ap.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zm.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mf.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ti.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://yc.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://bl.szsharing.cn

[H07] 断言
来源：http://fh.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://qz.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://lg.newstarts.cn

JS:   console.assert(x > 0);
来源：http://bx.521024.cn

TS:   console.assert(x > 0);
来源：http://zz.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://iw.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xw.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dr.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://pr.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://fh.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://gb.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ju.521024.cn

JS:   e.message;  e.stack
来源：http://zo.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hg.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ou.shtwfgs.cn

Go:   err.Error()
来源：http://mx.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://qp.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://wm.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://bw.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gd.jctech888.com.cn


<!-- 参考信息 -->