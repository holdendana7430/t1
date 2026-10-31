代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://oe.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nj.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://bq.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://eg.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://ok.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ax.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://un.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://sr.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://af.newstarts.cn

[F06] 删除文件
来源：http://ug.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://ll.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://hm.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kh.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mz.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qp.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://jy.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://hx.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://ba.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://lf.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pj.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uk.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://au.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://se.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wl.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xq.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vj.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fm.hnjuh.cn

[F08] 遍历目录
来源：http://bj.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ci.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dm.521024.cn

JS:   fs.readdirSync("dir")
来源：http://us.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://gd.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bn.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lv.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://tt.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://ks.yuexingan06.cn

[F09] 获取文件大小
来源：http://ja.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://fk.huanxung.cn

PHP:  filesize("a.txt");
来源：http://ws.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://lv.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://dx.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bf.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ri.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://zy.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://dj.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://nw.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ej.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://si.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ln.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://ig.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tf.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sf.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sq.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sq.nszjky.cn

[F11] 复制与移动文件
来源：http://jh.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tn.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zg.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bl.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hi.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pr.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zf.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://np.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ir.szxytkj.cn

[F12] CSV 读写
来源：http://dp.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://um.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ml.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vt.huanxung.cn

TS:   // 同上
来源：http://va.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zc.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://my.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vq.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qx.9csxet.cn

================================================================================
来源：http://jl.gzmigu.cn

G. 面向对象
来源：http://qk.newstarts.cn

================================================================================
来源：http://iy.chemitech.net.cn

[G01] 定义类
来源：http://kv.szsharing.cn

Py:   class User: pass
来源：http://hs.nicolike.cn

PHP:  class User {}
来源：http://kj.huanxung.cn

JS:   class User {}
来源：http://vr.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://na.jctech888.com.cn

Java: class User {}
来源：http://iq.newstarts.cn

Go:   type User struct { Name string }
来源：http://fu.lnxyls.cn

Ruby: class User; end
来源：http://az.jianghongdianzi.cn

C#:   class User {}
来源：http://jy.jianghongdianzi.cn

[G02] 构造函数
来源：http://fz.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://cg.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://pc.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://sf.asd995.cn

TS:   constructor(public name: string) {}
来源：http://nt.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://kd.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yp.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://nk.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://ot.bjjhwx.cn

[G03] 实例属性
来源：http://zw.gzmigu.cn

Py:   self.name = "x"
来源：http://fq.panjiajie.cn

PHP:  public string $name = "x";
来源：http://hd.szsharing.cn

JS:   this.name = "x";
来源：http://ge.shtwfgs.cn

TS:   name: string = "x";
来源：http://sj.szxytkj.cn

Java: private String name;
来源：http://jb.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lt.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://ou.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://nq.newstarts.cn

[G04] 定义方法
来源：http://ja.nszjky.cn

Py:   def greet(self): return self.name
来源：http://rb.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://us.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://tw.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://aa.szsharing.cn

Java: String greet() { return name; }
来源：http://dt.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zw.nicolike.cn

Ruby: def greet; @name; end
来源：http://tw.521024.cn

C#:   public string Greet() => Name;
来源：http://vh.colortex.cn

[G05] 继承
来源：http://vi.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://ed.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://tk.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://cr.nszjky.cn

TS:   class Admin extends User {}
来源：http://bb.wgjwhj.cn

Java: class Admin extends User {}
来源：http://sy.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tt.shxzukj.cn

Ruby: class Admin < User; end
来源：http://cc.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://xs.nicolike.cn

[G06] 重写方法
来源：http://it.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://jv.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nt.521024.cn

JS:   greet() { return "admin"; }
来源：http://hz.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://jd.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://bx.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xs.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://vj.521024.cn

C#:   public override string Greet() => "admin";
来源：http://el.jctech888.com.cn

[G07] 调用父类方法
来源：http://zn.szsharing.cn

Py:   super().greet()
来源：http://vr.hnjuh.cn

PHP:  parent::greet();
来源：http://zm.9csxet.cn

JS:   super.greet();
来源：http://vb.yuntaijiaju.cn

TS:   super.greet();
来源：http://lx.bjjhwx.cn

Java: super.greet();
来源：http://qd.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gl.newstarts.cn

Ruby: super
来源：http://ah.muxihuayi.cn

C#:   base.Greet();
来源：http://ta.lnxyls.cn

[G08] 静态方法与属性
来源：http://qh.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://db.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://wb.huixiangedu.cn

JS:   static f() {}
来源：http://lu.nszjky.cn

TS:   static f(): void {}
来源：http://xm.wgjwhj.cn

Java: static void f() {}
来源：http://pf.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fu.szsharing.cn

Ruby: def self.f; end
来源：http://km.nszjky.cn

C#:   public static void F() {}
来源：http://xw.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://fg.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://ut.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://es.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dj.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://hi.huanxung.cn

Java: interface Shape { double area(); }
来源：http://kv.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://oj.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yh.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://fa.bookmarksfly.cn

[G10] 访问控制
来源：http://ul.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://fe.panjiajie.cn

PHP:  public / protected / private
来源：http://xg.huanxung.cn

JS:   #private 字段；其余公开
来源：http://kc.521024.cn

TS:   public / protected / private
来源：http://bq.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://pc.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lh.szxytkj.cn

Ruby: public / protected / private
来源：http://gl.shxzskj.cn

C#:   public / protected / private / internal
来源：http://ts.wgjwhj.cn

[G11] getter / setter
来源：http://rx.nszjky.cn

Py:   @property 与 @x.setter
来源：http://aw.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xb.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://jp.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://zj.huanxung.cn

Java: public String getName() { return name; }
来源：http://jn.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gf.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://jw.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://tc.szsharing.cn

[G12] 对象转字符串
来源：http://qt.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://np.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mm.hahajie.cn

JS:   toString() { return this.name; }
来源：http://oc.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://os.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://bh.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ip.colortex.cn

Ruby: def to_s; @name; end
来源：http://sp.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://jp.nicolike.cn

[G13] 判断对象类型
来源：http://gk.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://fk.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://se.huixiangedu.cn

JS:   u instanceof User
来源：http://nw.wgjwhj.cn

TS:   u instanceof User
来源：http://qf.gzmigu.cn

Java: u instanceof User
来源：http://mt.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ma.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://ph.hahajie.cn

C#:   u is User
来源：http://sj.muxihuayi.cn

[G14] 数据类 / record
来源：http://pd.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rb.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://ug.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://un.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://fi.newstarts.cn

Java: record User(String name, int age) {}
来源：http://or.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://qi.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dm.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://bk.bookmarksfly.cn

[G15] 枚举
来源：http://mz.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xn.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pj.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eg.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lx.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://vv.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sg.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://ko.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rj.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://nv.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hq.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://tb.szxytkj.cn

JS:   Object.entries(obj)
来源：http://gb.szxytkj.cn

TS:   Object.entries(obj)
来源：http://uv.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rc.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ml.hnjuh.cn

Ruby: obj.instance_variables
来源：http://rq.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ki.9csxet.cn

================================================================================
来源：http://ll.shtwfgs.cn

H. 异常与错误处理
来源：http://wd.huanxung.cn

================================================================================
来源：http://tv.hnjuh.cn

[H01] try / catch 基础
来源：http://fj.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tt.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://og.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qk.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cl.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kb.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lr.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sv.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jf.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://ju.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dw.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sk.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zt.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gb.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wq.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tg.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ua.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yj.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://le.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://np.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zp.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://ye.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://ll.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fy.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yl.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tx.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vr.shxzskj.cn

[H04] 自定义异常类型
来源：http://eu.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://nw.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gx.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://mc.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://sm.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://aw.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sq.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://xe.colortex.cn

C#:   class MyException : Exception {}
来源：http://zl.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://xw.newstarts.cn

Py:   except ValueError as e:
来源：http://md.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pg.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ju.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://bb.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://di.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mv.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://lo.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cw.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://lm.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://xf.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wh.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xj.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hl.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ar.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hn.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://qq.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://vd.shxzskj.cn

[H07] 断言
来源：http://gi.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://xt.colortex.cn

PHP:  assert($x > 0);
来源：http://mw.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://zy.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://vr.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://jl.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ar.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ed.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://yw.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://ss.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ss.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://so.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://tp.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vr.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uj.shxzskj.cn

Go:   err.Error()
来源：http://lv.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://he.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://wp.asd995.cn

[H09] 带错误码的异常
来源：http://hv.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yf.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dq.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ni.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ez.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ka.panjiajie.cn


<!-- 参考信息 -->