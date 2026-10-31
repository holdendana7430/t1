代发 wailian999

C#:   File.Exists("a.txt")
来源：http://wr.szxytkj.cn

[F06] 删除文件
来源：http://ml.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://ds.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://ym.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hr.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://eg.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kl.nicolike.cn

Go:   os.Remove("a.txt")
来源：http://ti.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://bm.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://ha.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://as.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gk.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://je.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zu.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vy.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sn.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xw.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pu.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cl.panjiajie.cn

[F08] 遍历目录
来源：http://cc.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://em.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pl.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://mv.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://vl.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dy.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bl.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://zn.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ff.asd995.cn

[F09] 获取文件大小
来源：http://el.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://kz.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://hh.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://op.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://ev.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sk.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tv.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://wd.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://lv.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://sa.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gl.huanxung.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pd.haigaiapp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ve.9csxet.cn

TS:   path.extname("a.txt")
来源：http://wr.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qx.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fv.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://th.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wi.wgjwhj.cn

[F11] 复制与移动文件
来源：http://ia.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ng.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hx.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zw.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hy.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ge.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pl.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ys.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gp.huixinmuqiang.cn

[F12] CSV 读写
来源：http://ex.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fj.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ql.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dt.521024.cn

TS:   // 同上
来源：http://gu.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ki.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uw.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zc.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hl.bjjhwx.cn

================================================================================
来源：http://ng.shxzukj.cn

G. 面向对象
来源：http://oy.panjiajie.cn

================================================================================
来源：http://sh.newstarts.cn

[G01] 定义类
来源：http://sg.hahajie.cn

Py:   class User: pass
来源：http://mv.haigaiapp.cn

PHP:  class User {}
来源：http://ix.hnjuh.cn

JS:   class User {}
来源：http://br.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://tt.huixinmuqiang.cn

Java: class User {}
来源：http://fk.nszjky.cn

Go:   type User struct { Name string }
来源：http://xs.bjjhwx.cn

Ruby: class User; end
来源：http://pi.yuntaijiaju.cn

C#:   class User {}
来源：http://um.hahajie.cn

[G02] 构造函数
来源：http://gv.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://np.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://ov.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://ac.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://mz.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://qe.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pa.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://lh.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://dx.huixiangedu.cn

[G03] 实例属性
来源：http://cm.jctech888.com.cn

Py:   self.name = "x"
来源：http://ez.9csxet.cn

PHP:  public string $name = "x";
来源：http://bd.shtwfgs.cn

JS:   this.name = "x";
来源：http://gf.colortex.cn

TS:   name: string = "x";
来源：http://cp.szxytkj.cn

Java: private String name;
来源：http://co.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ys.muxihuayi.cn

Ruby: @name = "x"
来源：http://xg.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ce.bjjhwx.cn

[G04] 定义方法
来源：http://hz.colortex.cn

Py:   def greet(self): return self.name
来源：http://fj.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ut.nicolike.cn

JS:   greet() { return this.name; }
来源：http://tz.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://el.hahajie.cn

Java: String greet() { return name; }
来源：http://tk.wgjwhj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yj.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://dw.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://dz.nszjky.cn

[G05] 继承
来源：http://rl.colortex.cn

Py:   class Admin(User): pass
来源：http://re.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://tr.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://yd.shxzskj.cn

TS:   class Admin extends User {}
来源：http://pv.shtwfgs.cn

Java: class Admin extends User {}
来源：http://qc.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lo.9csxet.cn

Ruby: class Admin < User; end
来源：http://lu.yuexingan06.cn

C#:   class Admin : User {}
来源：http://gi.jctech888.com.cn

[G06] 重写方法
来源：http://kl.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://on.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kg.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://up.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://zt.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://pu.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://is.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://mr.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://id.muxihuayi.cn

[G07] 调用父类方法
来源：http://gy.haigaiapp.cn

Py:   super().greet()
来源：http://tk.newstarts.cn

PHP:  parent::greet();
来源：http://qu.haigaiapp.cn

JS:   super.greet();
来源：http://rk.shtwfgs.cn

TS:   super.greet();
来源：http://fh.huanxung.cn

Java: super.greet();
来源：http://bk.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sv.nszjky.cn

Ruby: super
来源：http://oa.wgjwhj.cn

C#:   base.Greet();
来源：http://ho.shxzskj.cn

[G08] 静态方法与属性
来源：http://so.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ly.shxzukj.cn

PHP:  public static function f() {}
来源：http://ky.hnjuh.cn

JS:   static f() {}
来源：http://iz.asd995.cn

TS:   static f(): void {}
来源：http://sh.nicolike.cn

Java: static void f() {}
来源：http://tb.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pe.shxzukj.cn

Ruby: def self.f; end
来源：http://cg.huixiangedu.cn

C#:   public static void F() {}
来源：http://an.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://wj.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://gm.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vh.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xo.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://yp.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://bu.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://zs.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sn.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ee.shxzskj.cn

[G10] 访问控制
来源：http://sg.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://fc.bookmarksfly.cn

PHP:  public / protected / private
来源：http://gz.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://km.newstarts.cn

TS:   public / protected / private
来源：http://ub.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://cs.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ci.shtwfgs.cn

Ruby: public / protected / private
来源：http://jh.huanxung.cn

C#:   public / protected / private / internal
来源：http://do.panjiajie.cn

[G11] getter / setter
来源：http://pb.asd995.cn

Py:   @property 与 @x.setter
来源：http://pl.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ag.nicolike.cn

JS:   get name() { return this._name; }
来源：http://ca.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://to.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://rg.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://be.shxzukj.cn

Ruby: attr_accessor :name
来源：http://rf.nszjky.cn

C#:   public string Name { get; set; }
来源：http://ju.newstarts.cn

[G12] 对象转字符串
来源：http://mq.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://br.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hx.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://dj.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://vv.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://fv.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mk.521024.cn

Ruby: def to_s; @name; end
来源：http://ss.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://ok.newstarts.cn

[G13] 判断对象类型
来源：http://df.9csxet.cn

Py:   isinstance(u, User)
来源：http://dp.lnxyls.cn

PHP:  $u instanceof User
来源：http://gy.haigaiapp.cn

JS:   u instanceof User
来源：http://rd.9csxet.cn

TS:   u instanceof User
来源：http://db.gzmigu.cn

Java: u instanceof User
来源：http://xc.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ff.asd995.cn

Ruby: u.is_a?(User)
来源：http://aj.shtwfgs.cn

C#:   u is User
来源：http://je.huanxung.cn

[G14] 数据类 / record
来源：http://ch.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://up.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://qq.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eu.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://vj.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://aj.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://zn.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tn.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://ii.nszjky.cn

[G15] 枚举
来源：http://gw.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lo.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gm.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mw.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hv.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://ek.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://og.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://ep.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ph.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://tj.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kh.asd995.cn

PHP:  get_object_vars($obj);
来源：http://ec.nszjky.cn

JS:   Object.entries(obj)
来源：http://lu.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://gh.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rs.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zx.nicolike.cn

Ruby: obj.instance_variables
来源：http://qb.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://ry.newstarts.cn

================================================================================
来源：http://oh.huanxung.cn

H. 异常与错误处理
来源：http://eb.panjiajie.cn

================================================================================
来源：http://vi.szsharing.cn

[H01] try / catch 基础
来源：http://qy.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ov.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://am.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ll.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oc.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vx.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mv.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fp.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vp.nszjky.cn

[H02] finally / ensure 收尾
来源：http://sr.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://it.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nz.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iu.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vx.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lt.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zj.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ce.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://py.newstarts.cn

[H03] 主动抛出异常
来源：http://wk.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://xp.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xq.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://gm.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://za.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bq.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eg.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lw.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ec.muxihuayi.cn

[H04] 自定义异常类型
来源：http://gw.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://ba.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ec.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://rh.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://kv.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://gi.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gh.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ev.colortex.cn

C#:   class MyException : Exception {}
来源：http://ur.hahajie.cn

[H05] 捕获特定类型
来源：http://yb.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://io.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wp.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://nr.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://ri.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://rp.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jl.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://ob.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pj.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://ze.521024.cn

Py:   value = d.get("k") or default
来源：http://tf.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fw.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ep.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sc.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xg.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yp.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://ea.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://wx.9csxet.cn

[H07] 断言
来源：http://wh.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://eh.szsharing.cn

PHP:  assert($x > 0);
来源：http://er.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://we.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://yd.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://xo.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oq.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ah.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://dz.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://yc.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://ap.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ag.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://nc.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://on.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jq.wgjwhj.cn

Go:   err.Error()
来源：http://pn.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://lx.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://jo.nszjky.cn

[H09] 带错误码的异常
来源：http://la.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hf.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hs.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bh.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bi.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hr.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cq.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jn.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bz.bjjhwx.cn

[H10] 资源自动释放
来源：http://ti.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ig.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yr.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ia.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wm.panjiajie.cn


<!-- 参考信息 -->