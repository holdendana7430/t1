代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hb.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gx.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ct.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ph.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ey.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rn.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sk.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xi.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://jc.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mw.asd995.cn

PHP:  file_exists("a.txt");
来源：http://rf.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://py.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://xa.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ws.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://id.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://pt.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://ud.panjiajie.cn

[F06] 删除文件
来源：http://nf.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://do.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://ly.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mq.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://as.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cv.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://tt.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://ss.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://yb.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://oh.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sd.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cs.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gs.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rk.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sm.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jz.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qe.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://je.haigaiapp.cn

[F08] 遍历目录
来源：http://st.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cu.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gp.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://jg.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://ng.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kp.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kd.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://jk.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://rd.bookmarksfly.cn

[F09] 获取文件大小
来源：http://ka.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://zu.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ye.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://wd.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://ds.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ey.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rk.huanxung.cn

Ruby: File.size("a.txt")
来源：http://ox.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://sb.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ju.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gd.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aw.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rl.colortex.cn

TS:   path.extname("a.txt")
来源：http://ep.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ur.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bu.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qt.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gy.szsharing.cn

[F11] 复制与移动文件
来源：http://qs.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://le.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nk.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://br.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oh.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ji.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rg.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pp.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cv.hahajie.cn

[F12] CSV 读写
来源：http://ek.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ec.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gz.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nc.asd995.cn

TS:   // 同上
来源：http://ta.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pd.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://od.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://op.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ot.muxihuayi.cn

================================================================================
来源：http://gl.chemitech.net.cn

G. 面向对象
来源：http://jr.hnjuh.cn

================================================================================
来源：http://pc.bookmarksfly.cn

[G01] 定义类
来源：http://ht.newstarts.cn

Py:   class User: pass
来源：http://ak.shxzukj.cn

PHP:  class User {}
来源：http://dr.haigaiapp.cn

JS:   class User {}
来源：http://zd.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://sh.huanxung.cn

Java: class User {}
来源：http://pv.nicolike.cn

Go:   type User struct { Name string }
来源：http://yp.lnxyls.cn

Ruby: class User; end
来源：http://yb.lnxyls.cn

C#:   class User {}
来源：http://if.nszjky.cn

[G02] 构造函数
来源：http://gv.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://hc.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://vo.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://qn.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://st.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://la.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rf.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://tr.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ys.szxytkj.cn

[G03] 实例属性
来源：http://yb.colortex.cn

Py:   self.name = "x"
来源：http://xc.shxzskj.cn

PHP:  public string $name = "x";
来源：http://ls.hahajie.cn

JS:   this.name = "x";
来源：http://wg.9csxet.cn

TS:   name: string = "x";
来源：http://zl.bjjhwx.cn

Java: private String name;
来源：http://mx.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://le.521024.cn

Ruby: @name = "x"
来源：http://hj.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://wi.9csxet.cn

[G04] 定义方法
来源：http://mg.9csxet.cn

Py:   def greet(self): return self.name
来源：http://cx.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sk.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://wo.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://ib.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://cr.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xk.521024.cn

Ruby: def greet; @name; end
来源：http://zm.nszjky.cn

C#:   public string Greet() => Name;
来源：http://za.wgjwhj.cn

[G05] 继承
来源：http://pq.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://ct.nszjky.cn

PHP:  class Admin extends User {}
来源：http://uk.shxzskj.cn

JS:   class Admin extends User {}
来源：http://qc.asd995.cn

TS:   class Admin extends User {}
来源：http://rh.newstarts.cn

Java: class Admin extends User {}
来源：http://lv.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xa.colortex.cn

Ruby: class Admin < User; end
来源：http://cn.chemitech.net.cn

C#:   class Admin : User {}
来源：http://xc.bjjhwx.cn

[G06] 重写方法
来源：http://jk.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://zn.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mg.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://ky.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ur.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://yx.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qe.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://qo.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://mx.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://bh.hahajie.cn

Py:   super().greet()
来源：http://my.hnjuh.cn

PHP:  parent::greet();
来源：http://wl.panjiajie.cn

JS:   super.greet();
来源：http://th.colortex.cn

TS:   super.greet();
来源：http://ir.muxihuayi.cn

Java: super.greet();
来源：http://ih.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pa.wgjwhj.cn

Ruby: super
来源：http://jw.huixiangedu.cn

C#:   base.Greet();
来源：http://sf.shxzukj.cn

[G08] 静态方法与属性
来源：http://jb.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nx.nicolike.cn

PHP:  public static function f() {}
来源：http://hv.lnxyls.cn

JS:   static f() {}
来源：http://ur.huanxung.cn

TS:   static f(): void {}
来源：http://ip.hahajie.cn

Java: static void f() {}
来源：http://xz.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cw.lnxyls.cn

Ruby: def self.f; end
来源：http://rd.wgjwhj.cn

C#:   public static void F() {}
来源：http://vc.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://hb.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://pj.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jf.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fh.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://ma.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://ru.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://xj.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fw.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://uz.shtwfgs.cn

[G10] 访问控制
来源：http://yk.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://ng.bjjhwx.cn

PHP:  public / protected / private
来源：http://kw.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://wc.panjiajie.cn

TS:   public / protected / private
来源：http://qq.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://gn.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jw.gzmigu.cn

Ruby: public / protected / private
来源：http://fw.szsharing.cn

C#:   public / protected / private / internal
来源：http://zf.huixiangedu.cn

[G11] getter / setter
来源：http://wx.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://en.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ey.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://zr.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://zu.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://cb.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nf.hahajie.cn

Ruby: attr_accessor :name
来源：http://lv.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://tu.panjiajie.cn

[G12] 对象转字符串
来源：http://wi.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://nu.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://za.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://po.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://mi.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://sm.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fr.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://uj.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://tz.yuexingan06.cn

[G13] 判断对象类型
来源：http://wr.panjiajie.cn

Py:   isinstance(u, User)
来源：http://wk.shxzskj.cn

PHP:  $u instanceof User
来源：http://fz.jctech888.com.cn

JS:   u instanceof User
来源：http://vy.huanxung.cn

TS:   u instanceof User
来源：http://vc.lnxyls.cn

Java: u instanceof User
来源：http://xw.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ip.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://ga.huixinmuqiang.cn

C#:   u is User
来源：http://vc.gzmigu.cn

[G14] 数据类 / record
来源：http://me.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://je.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://bb.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://py.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://rr.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://rj.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://ys.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wq.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://an.colortex.cn

[G15] 枚举
来源：http://hw.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://py.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://be.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hf.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pg.521024.cn

Java: enum Color { RED, GREEN }
来源：http://ex.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zn.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://tt.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xo.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://xs.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ce.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ed.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://xz.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://md.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ap.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oy.panjiajie.cn

Ruby: obj.instance_variables
来源：http://ct.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://bk.521024.cn

================================================================================
来源：http://tu.szxytkj.cn

H. 异常与错误处理
来源：http://ux.huanxung.cn

================================================================================
来源：http://ta.szsharing.cn

[H01] try / catch 基础
来源：http://ud.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kw.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bg.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mb.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eo.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gd.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xf.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ny.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qr.521024.cn

[H02] finally / ensure 收尾
来源：http://ue.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jy.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jw.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vm.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cu.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eu.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wk.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://po.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://df.szxytkj.cn

[H03] 主动抛出异常
来源：http://uh.521024.cn

Py:   raise ValueError("错误信息")
来源：http://sg.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uo.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://mm.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://yz.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yx.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://es.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://da.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cn.haigaiapp.cn

[H04] 自定义异常类型
来源：http://bw.asd995.cn

Py:   class MyError(Exception): pass
来源：http://rl.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pk.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://yp.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://gq.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://ay.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://me.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://fk.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://gu.9csxet.cn

[H05] 捕获特定类型
来源：http://sp.haigaiapp.cn

Py:   except ValueError as e:
来源：http://bn.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nc.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://bl.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://cv.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://du.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gu.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://uo.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oj.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://tz.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://pg.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jv.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sm.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://on.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nf.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ue.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://vw.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://dm.bjjhwx.cn

[H07] 断言
来源：http://xw.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://mq.521024.cn

PHP:  assert($x > 0);
来源：http://rh.colortex.cn

JS:   console.assert(x > 0);
来源：http://vw.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://mo.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://zd.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ij.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pw.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://nl.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://gi.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://tc.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ea.shxzukj.cn

JS:   e.message;  e.stack
来源：http://qx.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hw.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jc.lnxyls.cn

Go:   err.Error()
来源：http://cp.szxytkj.cn


<!-- 参考信息 -->