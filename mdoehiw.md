代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://ey.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://np.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qb.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://kw.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://my.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://yf.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://wx.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://da.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lw.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jo.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://al.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sy.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ir.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wi.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yv.jctech888.com.cn

[F08] 遍历目录
来源：http://bq.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pp.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ua.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://au.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://rf.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cj.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bw.asd995.cn

Ruby: Dir.children("dir")
来源：http://wp.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ss.yuexingan06.cn

[F09] 获取文件大小
来源：http://bf.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://wj.9csxet.cn

PHP:  filesize("a.txt");
来源：http://bh.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://oh.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://sf.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://be.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ir.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://lw.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://kc.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://wl.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hq.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sc.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sd.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://te.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rj.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zo.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qo.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fm.bjjhwx.cn

[F11] 复制与移动文件
来源：http://ya.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sb.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://th.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wp.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://an.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nm.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://es.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ju.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oh.jianghongdianzi.cn

[F12] CSV 读写
来源：http://vr.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mc.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yd.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bn.521024.cn

TS:   // 同上
来源：http://yx.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://se.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xu.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rg.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://or.shxzskj.cn

================================================================================
来源：http://ix.bookmarksfly.cn

G. 面向对象
来源：http://it.9csxet.cn

================================================================================
来源：http://bj.huanxung.cn

[G01] 定义类
来源：http://ev.lnxyls.cn

Py:   class User: pass
来源：http://wl.shxzukj.cn

PHP:  class User {}
来源：http://tp.nicolike.cn

JS:   class User {}
来源：http://yq.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://ih.colortex.cn

Java: class User {}
来源：http://vv.shxzskj.cn

Go:   type User struct { Name string }
来源：http://bi.hahajie.cn

Ruby: class User; end
来源：http://xu.panjiajie.cn

C#:   class User {}
来源：http://rr.huanxung.cn

[G02] 构造函数
来源：http://ks.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://zr.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://sl.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://mt.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://qb.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://ep.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fk.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://ke.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://wq.panjiajie.cn

[G03] 实例属性
来源：http://pp.szxytkj.cn

Py:   self.name = "x"
来源：http://eu.hahajie.cn

PHP:  public string $name = "x";
来源：http://vl.szsharing.cn

JS:   this.name = "x";
来源：http://cg.szxytkj.cn

TS:   name: string = "x";
来源：http://bd.jctech888.com.cn

Java: private String name;
来源：http://ai.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ua.nicolike.cn

Ruby: @name = "x"
来源：http://af.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://dp.nicolike.cn

[G04] 定义方法
来源：http://du.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://kp.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ee.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://et.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://iz.jctech888.com.cn

Java: String greet() { return name; }
来源：http://zr.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zn.huanxung.cn

Ruby: def greet; @name; end
来源：http://le.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://yg.lnxyls.cn

[G05] 继承
来源：http://ep.shxzskj.cn

Py:   class Admin(User): pass
来源：http://gz.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://zv.hahajie.cn

JS:   class Admin extends User {}
来源：http://em.szxytkj.cn

TS:   class Admin extends User {}
来源：http://ti.huanxung.cn

Java: class Admin extends User {}
来源：http://ti.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ww.hahajie.cn

Ruby: class Admin < User; end
来源：http://qf.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://nh.huanxung.cn

[G06] 重写方法
来源：http://nj.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://ro.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fx.asd995.cn

JS:   greet() { return "admin"; }
来源：http://lu.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://bn.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://xi.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oy.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://fc.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://vc.chemitech.net.cn

[G07] 调用父类方法
来源：http://xo.haigaiapp.cn

Py:   super().greet()
来源：http://qn.bjjhwx.cn

PHP:  parent::greet();
来源：http://jg.newstarts.cn

JS:   super.greet();
来源：http://py.nszjky.cn

TS:   super.greet();
来源：http://nh.shxzukj.cn

Java: super.greet();
来源：http://pq.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cc.wgjwhj.cn

Ruby: super
来源：http://zl.jianghongdianzi.cn

C#:   base.Greet();
来源：http://ge.hnjuh.cn

[G08] 静态方法与属性
来源：http://ro.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xw.huanxung.cn

PHP:  public static function f() {}
来源：http://ay.gzmigu.cn

JS:   static f() {}
来源：http://px.szsharing.cn

TS:   static f(): void {}
来源：http://tu.shtwfgs.cn

Java: static void f() {}
来源：http://bq.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://et.newstarts.cn

Ruby: def self.f; end
来源：http://lv.muxihuayi.cn

C#:   public static void F() {}
来源：http://sn.nszjky.cn

[G09] 接口 / 抽象类
来源：http://cw.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://ey.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hm.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rb.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://nq.hahajie.cn

Java: interface Shape { double area(); }
来源：http://wf.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://hu.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fq.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://ym.gzmigu.cn

[G10] 访问控制
来源：http://ex.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://yd.shxzskj.cn

PHP:  public / protected / private
来源：http://fr.hahajie.cn

JS:   #private 字段；其余公开
来源：http://fy.huixiangedu.cn

TS:   public / protected / private
来源：http://ya.colortex.cn

Java: public / protected / private / 默认包级
来源：http://hn.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bq.nszjky.cn

Ruby: public / protected / private
来源：http://vn.asd995.cn

C#:   public / protected / private / internal
来源：http://nc.hahajie.cn

[G11] getter / setter
来源：http://td.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://oz.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gg.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://sp.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://bd.shxzskj.cn

Java: public String getName() { return name; }
来源：http://fd.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ug.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://wh.521024.cn

C#:   public string Name { get; set; }
来源：http://wo.nicolike.cn

[G12] 对象转字符串
来源：http://jd.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://gx.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xt.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://ga.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://mr.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://nh.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://at.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://ch.asd995.cn

C#:   public override string ToString() => Name;
来源：http://ss.chemitech.net.cn

[G13] 判断对象类型
来源：http://dt.szsharing.cn

Py:   isinstance(u, User)
来源：http://wr.521024.cn

PHP:  $u instanceof User
来源：http://df.huanxung.cn

JS:   u instanceof User
来源：http://vx.szxytkj.cn

TS:   u instanceof User
来源：http://wz.nicolike.cn

Java: u instanceof User
来源：http://ts.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fe.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://sd.hahajie.cn

C#:   u is User
来源：http://xt.huixiangedu.cn

[G14] 数据类 / record
来源：http://lm.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ft.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://vj.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hw.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://nk.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://tz.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://rw.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fo.521024.cn

C#:   record User(string Name, int Age);
来源：http://hj.jctech888.com.cn

[G15] 枚举
来源：http://zx.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://io.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://la.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qp.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cp.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://wy.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nj.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://ca.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oy.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://ka.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gj.521024.cn

PHP:  get_object_vars($obj);
来源：http://xo.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://gu.newstarts.cn

TS:   Object.entries(obj)
来源：http://xg.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tg.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ue.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://ok.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://gu.szsharing.cn

================================================================================
来源：http://pr.shxzskj.cn

H. 异常与错误处理
来源：http://er.chemitech.net.cn

================================================================================
来源：http://lv.bookmarksfly.cn

[H01] try / catch 基础
来源：http://lo.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pj.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gj.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sj.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ma.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xw.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jq.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wq.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vd.huanxung.cn

[H02] finally / ensure 收尾
来源：http://sz.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vq.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://us.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vp.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qe.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dr.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ph.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ja.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sd.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://gf.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://dl.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://no.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://gj.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://mx.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ok.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://le.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://po.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lc.huanxung.cn

[H04] 自定义异常类型
来源：http://py.521024.cn

Py:   class MyError(Exception): pass
来源：http://jq.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nc.hahajie.cn

JS:   class MyError extends Error {}
来源：http://qd.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://pu.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://jo.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yt.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ii.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://bo.nszjky.cn

[H05] 捕获特定类型
来源：http://tv.hnjuh.cn

Py:   except ValueError as e:
来源：http://xn.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gf.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://xh.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://gs.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://yo.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vr.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://st.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xu.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://pm.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://bs.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://an.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bi.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ht.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qu.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ni.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ex.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://au.huanxung.cn

[H07] 断言
来源：http://bo.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://xw.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://gc.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://lh.9csxet.cn

TS:   console.assert(x > 0);
来源：http://hy.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://zx.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pw.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nb.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://vg.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://ir.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://qc.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yt.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://on.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ub.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lw.9csxet.cn

Go:   err.Error()
来源：http://yw.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://su.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://bc.haigaiapp.cn

[H09] 带错误码的异常
来源：http://wy.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uu.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zc.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vn.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://po.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://st.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://za.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://na.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cb.shxzskj.cn

[H10] 资源自动释放
来源：http://id.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yt.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kc.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hp.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pt.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qv.shxzukj.cn

Go:   defer f.Close()
来源：http://oe.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rv.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ul.huanxung.cn


<!-- 参考信息 -->