代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://ca.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ul.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ci.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://qd.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://lv.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://rw.szsharing.cn

[F07] 创建目录（含多级）
来源：http://km.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gw.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://km.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pm.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xl.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ib.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uy.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xh.yuexingan06.cn

[F08] 遍历目录
来源：http://dr.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://km.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yh.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://zd.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://ea.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tw.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dd.nszjky.cn

Ruby: Dir.children("dir")
来源：http://fw.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://iu.yuexingan06.cn

[F09] 获取文件大小
来源：http://pf.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://iv.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://qc.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://sv.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://xn.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://an.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zi.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://zn.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://mi.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://fe.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vb.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tl.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dw.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://jr.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ra.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://on.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cd.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wy.huanxung.cn

[F11] 复制与移动文件
来源：http://ay.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ab.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lc.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nh.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://to.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nb.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ff.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vd.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://is.colortex.cn

[F12] CSV 读写
来源：http://ib.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qm.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sw.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zg.yuntaijiaju.cn

TS:   // 同上
来源：http://ix.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iv.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rq.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cr.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zo.huixinmuqiang.cn

================================================================================
来源：http://kc.panjiajie.cn

G. 面向对象
来源：http://rn.gzmigu.cn

================================================================================
来源：http://sq.shxzukj.cn

[G01] 定义类
来源：http://iu.muxihuayi.cn

Py:   class User: pass
来源：http://ki.yuexingan06.cn

PHP:  class User {}
来源：http://xd.nszjky.cn

JS:   class User {}
来源：http://sr.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://sv.huixiangedu.cn

Java: class User {}
来源：http://cn.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://ev.huixiangedu.cn

Ruby: class User; end
来源：http://dv.jianghongdianzi.cn

C#:   class User {}
来源：http://tf.521024.cn

[G02] 构造函数
来源：http://zb.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://hq.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://mm.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ee.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://af.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://hc.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xs.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://dx.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://yw.asd995.cn

[G03] 实例属性
来源：http://vz.yuexingan06.cn

Py:   self.name = "x"
来源：http://bp.lnxyls.cn

PHP:  public string $name = "x";
来源：http://ib.9csxet.cn

JS:   this.name = "x";
来源：http://im.521024.cn

TS:   name: string = "x";
来源：http://tg.szsharing.cn

Java: private String name;
来源：http://cw.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tl.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://ds.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://et.jianghongdianzi.cn

[G04] 定义方法
来源：http://um.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://jm.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ix.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://tr.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://hs.hahajie.cn

Java: String greet() { return name; }
来源：http://nw.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ce.huanxung.cn

Ruby: def greet; @name; end
来源：http://dm.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://qo.huixiangedu.cn

[G05] 继承
来源：http://ni.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://xt.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://wm.szsharing.cn

JS:   class Admin extends User {}
来源：http://ha.asd995.cn

TS:   class Admin extends User {}
来源：http://bi.muxihuayi.cn

Java: class Admin extends User {}
来源：http://vz.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mz.colortex.cn

Ruby: class Admin < User; end
来源：http://or.szsharing.cn

C#:   class Admin : User {}
来源：http://ip.huixiangedu.cn

[G06] 重写方法
来源：http://we.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://yo.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sw.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://qy.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://ia.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://om.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://co.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://qd.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://ek.9csxet.cn

[G07] 调用父类方法
来源：http://gq.bookmarksfly.cn

Py:   super().greet()
来源：http://yc.shtwfgs.cn

PHP:  parent::greet();
来源：http://xs.yuntaijiaju.cn

JS:   super.greet();
来源：http://bx.lnxyls.cn

TS:   super.greet();
来源：http://ll.521024.cn

Java: super.greet();
来源：http://od.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fz.asd995.cn

Ruby: super
来源：http://oc.jianghongdianzi.cn

C#:   base.Greet();
来源：http://ff.bjjhwx.cn

[G08] 静态方法与属性
来源：http://jk.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wh.huanxung.cn

PHP:  public static function f() {}
来源：http://jj.bookmarksfly.cn

JS:   static f() {}
来源：http://xn.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://zy.521024.cn

Java: static void f() {}
来源：http://ge.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pj.bjjhwx.cn

Ruby: def self.f; end
来源：http://zj.9csxet.cn

C#:   public static void F() {}
来源：http://mf.colortex.cn

[G09] 接口 / 抽象类
来源：http://dk.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://vu.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ry.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://of.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://ec.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://wc.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://lc.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cp.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://cu.yuntaijiaju.cn

[G10] 访问控制
来源：http://aj.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://gz.szxytkj.cn

PHP:  public / protected / private
来源：http://pd.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://qm.huanxung.cn

TS:   public / protected / private
来源：http://xj.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://dz.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ez.521024.cn

Ruby: public / protected / private
来源：http://jk.nszjky.cn

C#:   public / protected / private / internal
来源：http://xy.nszjky.cn

[G11] getter / setter
来源：http://qo.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://ql.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ul.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://lo.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ye.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://sc.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zq.panjiajie.cn

Ruby: attr_accessor :name
来源：http://pc.nicolike.cn

C#:   public string Name { get; set; }
来源：http://xu.bookmarksfly.cn

[G12] 对象转字符串
来源：http://vv.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://em.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cs.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://an.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://qm.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://tu.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qq.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://vz.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://xm.wgjwhj.cn

[G13] 判断对象类型
来源：http://so.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://nn.chemitech.net.cn

PHP:  $u instanceof User
来源：http://iy.huixiangedu.cn

JS:   u instanceof User
来源：http://rm.szxytkj.cn

TS:   u instanceof User
来源：http://hz.wgjwhj.cn

Java: u instanceof User
来源：http://if.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qj.newstarts.cn

Ruby: u.is_a?(User)
来源：http://bp.huanxung.cn

C#:   u is User
来源：http://bl.huixiangedu.cn

[G14] 数据类 / record
来源：http://jv.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tg.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://fs.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aw.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://pw.colortex.cn

Java: record User(String name, int age) {}
来源：http://da.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://tu.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ju.521024.cn

C#:   record User(string Name, int Age);
来源：http://wr.panjiajie.cn

[G15] 枚举
来源：http://gl.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://au.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fr.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qa.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fk.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://tn.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kb.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://sq.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kh.asd995.cn

[G16] 对象转数组 / 字典
来源：http://xb.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bi.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://qw.huanxung.cn

JS:   Object.entries(obj)
来源：http://zt.huanxung.cn

TS:   Object.entries(obj)
来源：http://vl.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kk.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gw.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://mn.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://bz.nicolike.cn

================================================================================
来源：http://ck.nszjky.cn

H. 异常与错误处理
来源：http://jc.shxzukj.cn

================================================================================
来源：http://qo.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://wo.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lz.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qo.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ng.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ih.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wa.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ed.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uw.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wq.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://vr.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://al.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kl.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://on.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fw.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://df.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ri.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vp.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jw.haigaiapp.cn

[H03] 主动抛出异常
来源：http://ho.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://ep.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ym.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://aw.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://ga.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qy.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ws.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kz.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lg.hnjuh.cn

[H04] 自定义异常类型
来源：http://vp.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://ef.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://we.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://zd.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://bj.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://tf.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tl.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://be.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://mo.shxzukj.cn

[H05] 捕获特定类型
来源：http://yk.shtwfgs.cn

Py:   except ValueError as e:
来源：http://tq.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yk.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://rl.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://ea.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://lm.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yz.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://pe.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://on.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://dj.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://vi.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pk.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oa.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lo.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xg.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jn.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://pp.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://oz.haigaiapp.cn

[H07] 断言
来源：http://la.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://wn.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://xb.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://fm.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://jp.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://hp.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kt.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iz.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ze.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://or.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://le.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uz.panjiajie.cn

JS:   e.message;  e.stack
来源：http://jt.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ax.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ql.huixiangedu.cn

Go:   err.Error()
来源：http://pc.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://qx.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://pg.9csxet.cn

[H09] 带错误码的异常
来源：http://xw.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eu.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vz.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cu.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wq.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jg.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ec.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jc.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qq.9csxet.cn

[H10] 资源自动释放
来源：http://lb.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vu.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qi.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pd.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kr.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uk.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://gn.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gf.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lu.colortex.cn


<!-- 参考信息 -->