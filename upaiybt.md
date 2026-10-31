代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cu.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qe.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yq.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wh.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://ms.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xe.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://wx.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://qd.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://nv.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ky.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://na.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://hu.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://wm.yuexingan06.cn

[F06] 删除文件
来源：http://aw.szsharing.cn

Py:   os.remove("a.txt")
来源：http://ww.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://lh.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://es.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tm.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ck.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://fw.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://ho.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://zz.asd995.cn

[F07] 创建目录（含多级）
来源：http://bo.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ho.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xv.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nj.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nv.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ad.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://it.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://np.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bz.huixinmuqiang.cn

[F08] 遍历目录
来源：http://cp.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ha.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wn.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://la.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://gz.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cy.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iv.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://hp.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://ez.newstarts.cn

[F09] 获取文件大小
来源：http://gf.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://xi.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://br.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://mr.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://ea.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wy.huanxung.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vr.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://fs.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://uw.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://tp.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jm.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ur.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uv.nszjky.cn

TS:   path.extname("a.txt")
来源：http://to.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fr.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wj.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gw.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ui.shxzskj.cn

[F11] 复制与移动文件
来源：http://eg.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bu.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fp.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pn.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dh.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zg.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ot.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://of.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xs.nicolike.cn

[F12] CSV 读写
来源：http://wj.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zs.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ir.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qs.yuntaijiaju.cn

TS:   // 同上
来源：http://ua.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xu.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pt.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zw.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ou.bookmarksfly.cn

================================================================================
来源：http://kv.panjiajie.cn

G. 面向对象
来源：http://sf.lnxyls.cn

================================================================================
来源：http://pg.shtwfgs.cn

[G01] 定义类
来源：http://sj.haigaiapp.cn

Py:   class User: pass
来源：http://hc.gzmigu.cn

PHP:  class User {}
来源：http://kz.nszjky.cn

JS:   class User {}
来源：http://hg.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://jt.lnxyls.cn

Java: class User {}
来源：http://cm.huanxung.cn

Go:   type User struct { Name string }
来源：http://lu.shxzukj.cn

Ruby: class User; end
来源：http://fd.panjiajie.cn

C#:   class User {}
来源：http://hv.bjjhwx.cn

[G02] 构造函数
来源：http://nc.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://no.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://sz.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ot.colortex.cn

TS:   constructor(public name: string) {}
来源：http://xv.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://df.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xf.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://fm.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://is.nicolike.cn

[G03] 实例属性
来源：http://oi.huanxung.cn

Py:   self.name = "x"
来源：http://nv.shxzukj.cn

PHP:  public string $name = "x";
来源：http://dg.shxzukj.cn

JS:   this.name = "x";
来源：http://ky.nszjky.cn

TS:   name: string = "x";
来源：http://er.lnxyls.cn

Java: private String name;
来源：http://gc.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ho.gzmigu.cn

Ruby: @name = "x"
来源：http://sc.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://ul.newstarts.cn

[G04] 定义方法
来源：http://xl.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://wg.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jb.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://cx.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://ru.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://jo.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bq.521024.cn

Ruby: def greet; @name; end
来源：http://gl.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://eb.chemitech.net.cn

[G05] 继承
来源：http://ta.nszjky.cn

Py:   class Admin(User): pass
来源：http://rv.521024.cn

PHP:  class Admin extends User {}
来源：http://sz.asd995.cn

JS:   class Admin extends User {}
来源：http://tu.shxzskj.cn

TS:   class Admin extends User {}
来源：http://qy.yuexingan06.cn

Java: class Admin extends User {}
来源：http://yc.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sd.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://xt.hahajie.cn

C#:   class Admin : User {}
来源：http://mw.panjiajie.cn

[G06] 重写方法
来源：http://ck.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://ms.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sr.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://fd.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://fr.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://ly.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eg.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://px.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://cs.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://ob.huixinmuqiang.cn

Py:   super().greet()
来源：http://gr.hnjuh.cn

PHP:  parent::greet();
来源：http://bs.nszjky.cn

JS:   super.greet();
来源：http://vw.521024.cn

TS:   super.greet();
来源：http://dn.yuntaijiaju.cn

Java: super.greet();
来源：http://zp.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ok.hnjuh.cn

Ruby: super
来源：http://ot.colortex.cn

C#:   base.Greet();
来源：http://ki.gzmigu.cn

[G08] 静态方法与属性
来源：http://gk.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vx.huanxung.cn

PHP:  public static function f() {}
来源：http://ro.nszjky.cn

JS:   static f() {}
来源：http://oe.hnjuh.cn

TS:   static f(): void {}
来源：http://ca.yuntaijiaju.cn

Java: static void f() {}
来源：http://ln.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hd.newstarts.cn

Ruby: def self.f; end
来源：http://jt.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://em.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://px.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://lg.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rp.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pj.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://yj.hahajie.cn

Java: interface Shape { double area(); }
来源：http://kh.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://we.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yy.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://xv.shxzskj.cn

[G10] 访问控制
来源：http://bo.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://jy.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://uv.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://yz.hnjuh.cn

TS:   public / protected / private
来源：http://tf.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://bf.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kt.bjjhwx.cn

Ruby: public / protected / private
来源：http://fu.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://dd.yuntaijiaju.cn

[G11] getter / setter
来源：http://lu.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://ej.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sr.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://ko.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://yb.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://al.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://we.asd995.cn

Ruby: attr_accessor :name
来源：http://wc.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://uq.asd995.cn

[G12] 对象转字符串
来源：http://nv.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://vz.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ci.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://ga.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://qy.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://ut.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vq.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://gs.asd995.cn

C#:   public override string ToString() => Name;
来源：http://gt.muxihuayi.cn

[G13] 判断对象类型
来源：http://gp.nicolike.cn

Py:   isinstance(u, User)
来源：http://xh.hahajie.cn

PHP:  $u instanceof User
来源：http://vy.shtwfgs.cn

JS:   u instanceof User
来源：http://ln.shxzskj.cn

TS:   u instanceof User
来源：http://yk.asd995.cn

Java: u instanceof User
来源：http://yp.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fd.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://ai.shxzukj.cn

C#:   u is User
来源：http://wl.asd995.cn

[G14] 数据类 / record
来源：http://zv.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mp.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://ss.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xq.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://ed.huanxung.cn

Java: record User(String name, int age) {}
来源：http://rk.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://dh.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ca.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://ac.bookmarksfly.cn

[G15] 枚举
来源：http://ki.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zq.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gk.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fs.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mh.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://oh.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cu.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://qu.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ln.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://ad.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cb.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://df.asd995.cn

JS:   Object.entries(obj)
来源：http://pf.nszjky.cn

TS:   Object.entries(obj)
来源：http://fk.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yb.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jt.szsharing.cn

Ruby: obj.instance_variables
来源：http://yf.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://bs.colortex.cn

================================================================================
来源：http://ky.panjiajie.cn

H. 异常与错误处理
来源：http://ko.9csxet.cn

================================================================================
来源：http://mj.wgjwhj.cn

[H01] try / catch 基础
来源：http://wp.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tl.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eo.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ly.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fb.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ps.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kc.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://up.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rq.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://mn.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ow.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kw.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hb.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ic.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kl.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oc.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bm.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sy.lnxyls.cn

[H03] 主动抛出异常
来源：http://wy.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://fh.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ps.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://ec.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://hq.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xy.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tj.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ch.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gt.bjjhwx.cn

[H04] 自定义异常类型
来源：http://bm.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://pa.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ja.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://fp.asd995.cn

TS:   class MyError extends Error {}
来源：http://nu.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://oh.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://se.521024.cn

Ruby: class MyError < StandardError; end
来源：http://pu.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://km.huixiangedu.cn

[H05] 捕获特定类型
来源：http://zb.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://wv.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pt.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://dy.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://ju.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://cc.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gw.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://ex.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kz.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://nb.nicolike.cn

Py:   value = d.get("k") or default
来源：http://qr.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jk.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ln.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://id.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fp.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gl.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://ne.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://ab.huanxung.cn

[H07] 断言
来源：http://ui.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://py.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://lp.asd995.cn

JS:   console.assert(x > 0);
来源：http://fq.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://sq.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://rp.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://np.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pw.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://er.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://ak.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://co.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rk.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://td.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dg.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://by.jctech888.com.cn

Go:   err.Error()
来源：http://eo.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://me.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://cb.nicolike.cn

[H09] 带错误码的异常
来源：http://ka.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sa.huanxung.cn


<!-- 参考信息 -->