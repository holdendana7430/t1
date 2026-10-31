代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://rf.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xy.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lb.521024.cn

Ruby: File.exist?("a.txt")
来源：http://ba.lnxyls.cn

C#:   File.Exists("a.txt")
来源：http://jg.gzmigu.cn

[F06] 删除文件
来源：http://ip.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://ay.colortex.cn

PHP:  unlink("a.txt");
来源：http://wu.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iv.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nl.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tl.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://ut.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://fw.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://ju.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://fu.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://os.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ki.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ro.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fv.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vx.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qb.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cv.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bx.shtwfgs.cn

[F08] 遍历目录
来源：http://id.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pp.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://th.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://dw.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://kc.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://su.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kp.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ri.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://jr.shxzukj.cn

[F09] 获取文件大小
来源：http://la.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://ta.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://uq.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://mj.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://nq.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ug.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ih.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://zo.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://mn.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://nl.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://si.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wa.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ql.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://fm.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tv.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ks.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kw.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ko.muxihuayi.cn

[F11] 复制与移动文件
来源：http://ik.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ca.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xg.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jz.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xx.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uk.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mf.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tw.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://se.lnxyls.cn

[F12] CSV 读写
来源：http://xc.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rt.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ee.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qd.shtwfgs.cn

TS:   // 同上
来源：http://gt.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gq.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sy.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zk.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hh.shxzskj.cn

================================================================================
来源：http://hu.huixiangedu.cn

G. 面向对象
来源：http://tg.nicolike.cn

================================================================================
来源：http://bl.huixinmuqiang.cn

[G01] 定义类
来源：http://vt.muxihuayi.cn

Py:   class User: pass
来源：http://xo.nszjky.cn

PHP:  class User {}
来源：http://ko.shxzskj.cn

JS:   class User {}
来源：http://ya.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://gx.szsharing.cn

Java: class User {}
来源：http://yc.9csxet.cn

Go:   type User struct { Name string }
来源：http://dn.shxzskj.cn

Ruby: class User; end
来源：http://uf.chemitech.net.cn

C#:   class User {}
来源：http://on.lnxyls.cn

[G02] 构造函数
来源：http://jq.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://tl.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://rm.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://vt.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://zn.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://en.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ej.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://kw.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://ft.shxzukj.cn

[G03] 实例属性
来源：http://wn.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://he.huanxung.cn

PHP:  public string $name = "x";
来源：http://lm.jctech888.com.cn

JS:   this.name = "x";
来源：http://dc.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://qt.shtwfgs.cn

Java: private String name;
来源：http://nt.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sc.hahajie.cn

Ruby: @name = "x"
来源：http://rh.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ho.hahajie.cn

[G04] 定义方法
来源：http://bd.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://hn.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mp.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://su.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://bh.shxzskj.cn

Java: String greet() { return name; }
来源：http://uc.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hd.colortex.cn

Ruby: def greet; @name; end
来源：http://nh.asd995.cn

C#:   public string Greet() => Name;
来源：http://bp.521024.cn

[G05] 继承
来源：http://ne.panjiajie.cn

Py:   class Admin(User): pass
来源：http://uj.szsharing.cn

PHP:  class Admin extends User {}
来源：http://jc.newstarts.cn

JS:   class Admin extends User {}
来源：http://fl.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://st.hahajie.cn

Java: class Admin extends User {}
来源：http://av.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zl.panjiajie.cn

Ruby: class Admin < User; end
来源：http://di.huixiangedu.cn

C#:   class Admin : User {}
来源：http://uq.gzmigu.cn

[G06] 重写方法
来源：http://ot.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://hj.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zf.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://oq.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://zb.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://ei.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ad.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://rl.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://cf.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://ii.colortex.cn

Py:   super().greet()
来源：http://vq.huanxung.cn

PHP:  parent::greet();
来源：http://yr.colortex.cn

JS:   super.greet();
来源：http://oe.521024.cn

TS:   super.greet();
来源：http://av.nicolike.cn

Java: super.greet();
来源：http://ox.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zb.9csxet.cn

Ruby: super
来源：http://we.huixinmuqiang.cn

C#:   base.Greet();
来源：http://ca.wgjwhj.cn

[G08] 静态方法与属性
来源：http://wy.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sw.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://ja.521024.cn

JS:   static f() {}
来源：http://jg.newstarts.cn

TS:   static f(): void {}
来源：http://qo.colortex.cn

Java: static void f() {}
来源：http://gb.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zy.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://ro.shxzukj.cn

C#:   public static void F() {}
来源：http://sk.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://qc.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://sn.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ij.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://on.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://nn.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://nl.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://eo.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kw.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://is.colortex.cn

[G10] 访问控制
来源：http://tp.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://rg.shxzukj.cn

PHP:  public / protected / private
来源：http://ux.newstarts.cn

JS:   #private 字段；其余公开
来源：http://nr.panjiajie.cn

TS:   public / protected / private
来源：http://qk.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://lu.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jd.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://hs.szxytkj.cn

C#:   public / protected / private / internal
来源：http://us.chemitech.net.cn

[G11] getter / setter
来源：http://kg.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://rg.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mt.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ae.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://pk.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://gu.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://by.shxzskj.cn

Ruby: attr_accessor :name
来源：http://pm.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://dc.haigaiapp.cn

[G12] 对象转字符串
来源：http://az.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://bs.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ec.nszjky.cn

JS:   toString() { return this.name; }
来源：http://ug.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://ml.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://lg.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kl.newstarts.cn

Ruby: def to_s; @name; end
来源：http://eh.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://iu.yuexingan06.cn

[G13] 判断对象类型
来源：http://fj.521024.cn

Py:   isinstance(u, User)
来源：http://fj.bjjhwx.cn

PHP:  $u instanceof User
来源：http://io.yuexingan06.cn

JS:   u instanceof User
来源：http://ij.yuntaijiaju.cn

TS:   u instanceof User
来源：http://rm.nszjky.cn

Java: u instanceof User
来源：http://wg.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://up.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://vg.muxihuayi.cn

C#:   u is User
来源：http://bx.szxytkj.cn

[G14] 数据类 / record
来源：http://la.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bm.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://ki.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lc.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://ll.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://sc.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://sw.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nm.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://yg.asd995.cn

[G15] 枚举
来源：http://bk.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mh.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mf.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vn.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ji.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://jl.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://re.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://jl.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hn.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://ho.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fq.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://fz.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://fs.asd995.cn

TS:   Object.entries(obj)
来源：http://wb.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ww.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rh.lnxyls.cn

Ruby: obj.instance_variables
来源：http://le.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://yb.huixiangedu.cn

================================================================================
来源：http://sd.bjjhwx.cn

H. 异常与错误处理
来源：http://iz.huixiangedu.cn

================================================================================
来源：http://wr.szxytkj.cn

[H01] try / catch 基础
来源：http://jk.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dk.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ll.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tv.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eh.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vp.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uc.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ev.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yh.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://vr.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://un.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ux.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wf.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mg.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qx.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ov.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qk.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mk.wgjwhj.cn

[H03] 主动抛出异常
来源：http://ly.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://ci.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zr.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://nb.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://ut.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vr.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pr.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kw.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cc.9csxet.cn

[H04] 自定义异常类型
来源：http://bh.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://ib.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uv.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://fu.newstarts.cn

TS:   class MyError extends Error {}
来源：http://ux.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://at.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ku.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://at.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://on.newstarts.cn

[H05] 捕获特定类型
来源：http://yj.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://fl.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://py.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://ts.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://kp.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://uo.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xh.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://ar.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nf.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://wc.newstarts.cn

Py:   value = d.get("k") or default
来源：http://qv.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qp.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pb.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cs.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ni.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xt.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://fs.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://cz.haigaiapp.cn

[H07] 断言
来源：http://yt.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://nd.nicolike.cn

PHP:  assert($x > 0);
来源：http://hy.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://vv.szsharing.cn

TS:   console.assert(x > 0);
来源：http://jl.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://jf.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jn.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qr.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://br.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://ux.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://fb.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uf.lnxyls.cn

JS:   e.message;  e.stack
来源：http://rq.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jg.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oc.panjiajie.cn

Go:   err.Error()
来源：http://tk.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://mg.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://ph.muxihuayi.cn

[H09] 带错误码的异常
来源：http://at.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ot.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lz.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yh.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vt.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ex.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://po.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ff.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oj.shtwfgs.cn

[H10] 资源自动释放
来源：http://zw.nszjky.cn


<!-- 参考信息 -->