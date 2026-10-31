代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ao.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ob.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ix.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://na.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ny.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ja.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gz.huixiangedu.cn

[F08] 遍历目录
来源：http://md.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vp.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ja.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://lb.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://as.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jc.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zw.shxzskj.cn

Ruby: Dir.children("dir")
来源：http://ud.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://ua.chemitech.net.cn

[F09] 获取文件大小
来源：http://uq.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ic.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://fr.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://pf.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://sb.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tx.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://es.asd995.cn

Ruby: File.size("a.txt")
来源：http://nk.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://ml.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://fp.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xy.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uy.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dr.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://fd.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kv.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yc.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tg.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jc.hnjuh.cn

[F11] 复制与移动文件
来源：http://vn.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cm.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mw.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yv.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fz.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://go.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ot.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qk.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yx.hnjuh.cn

[F12] CSV 读写
来源：http://tf.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zg.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gy.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kq.jianghongdianzi.cn

TS:   // 同上
来源：http://zb.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aq.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://up.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rx.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hq.huanxung.cn

================================================================================
来源：http://nd.jctech888.com.cn

G. 面向对象
来源：http://bx.huanxung.cn

================================================================================
来源：http://wy.hahajie.cn

[G01] 定义类
来源：http://oj.yuntaijiaju.cn

Py:   class User: pass
来源：http://lr.521024.cn

PHP:  class User {}
来源：http://rw.jctech888.com.cn

JS:   class User {}
来源：http://hz.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://al.bjjhwx.cn

Java: class User {}
来源：http://ol.panjiajie.cn

Go:   type User struct { Name string }
来源：http://dd.9csxet.cn

Ruby: class User; end
来源：http://lx.bookmarksfly.cn

C#:   class User {}
来源：http://pd.nicolike.cn

[G02] 构造函数
来源：http://ao.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://du.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://gp.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://ew.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://fr.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://ej.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lz.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://za.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://yx.chemitech.net.cn

[G03] 实例属性
来源：http://za.nicolike.cn

Py:   self.name = "x"
来源：http://mm.colortex.cn

PHP:  public string $name = "x";
来源：http://cl.shxzukj.cn

JS:   this.name = "x";
来源：http://ln.yuexingan06.cn

TS:   name: string = "x";
来源：http://km.521024.cn

Java: private String name;
来源：http://gz.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nh.521024.cn

Ruby: @name = "x"
来源：http://bx.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://eq.newstarts.cn

[G04] 定义方法
来源：http://bl.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://jb.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nv.nicolike.cn

JS:   greet() { return this.name; }
来源：http://ym.521024.cn

TS:   greet(): string { return this.name; }
来源：http://cn.hahajie.cn

Java: String greet() { return name; }
来源：http://ak.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kn.szsharing.cn

Ruby: def greet; @name; end
来源：http://ld.nicolike.cn

C#:   public string Greet() => Name;
来源：http://zo.chemitech.net.cn

[G05] 继承
来源：http://tm.shxzukj.cn

Py:   class Admin(User): pass
来源：http://uq.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://wf.hahajie.cn

JS:   class Admin extends User {}
来源：http://uk.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://nk.yuexingan06.cn

Java: class Admin extends User {}
来源：http://fu.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yz.hahajie.cn

Ruby: class Admin < User; end
来源：http://an.lnxyls.cn

C#:   class Admin : User {}
来源：http://ux.lnxyls.cn

[G06] 重写方法
来源：http://ou.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://aa.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jt.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://yo.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://qu.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://by.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pj.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://ff.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://bz.shtwfgs.cn

[G07] 调用父类方法
来源：http://ef.huixinmuqiang.cn

Py:   super().greet()
来源：http://yi.9csxet.cn

PHP:  parent::greet();
来源：http://wk.jianghongdianzi.cn

JS:   super.greet();
来源：http://hn.huixiangedu.cn

TS:   super.greet();
来源：http://ea.huixiangedu.cn

Java: super.greet();
来源：http://cw.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vo.yuexingan06.cn

Ruby: super
来源：http://sk.huixinmuqiang.cn

C#:   base.Greet();
来源：http://qy.haigaiapp.cn

[G08] 静态方法与属性
来源：http://wb.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://du.colortex.cn

PHP:  public static function f() {}
来源：http://os.huanxung.cn

JS:   static f() {}
来源：http://pb.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://bb.bookmarksfly.cn

Java: static void f() {}
来源：http://rb.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gw.muxihuayi.cn

Ruby: def self.f; end
来源：http://st.nszjky.cn

C#:   public static void F() {}
来源：http://hx.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://yq.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://fx.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ws.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vf.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://ae.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://nc.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ug.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pl.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://yx.muxihuayi.cn

[G10] 访问控制
来源：http://zo.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://qj.lnxyls.cn

PHP:  public / protected / private
来源：http://em.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://oc.gzmigu.cn

TS:   public / protected / private
来源：http://wt.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://xa.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://he.nicolike.cn

Ruby: public / protected / private
来源：http://nu.colortex.cn

C#:   public / protected / private / internal
来源：http://xe.panjiajie.cn

[G11] getter / setter
来源：http://xw.huanxung.cn

Py:   @property 与 @x.setter
来源：http://wl.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hm.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://ya.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://et.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://iw.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://re.szsharing.cn

Ruby: attr_accessor :name
来源：http://dw.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://lv.yuexingan06.cn

[G12] 对象转字符串
来源：http://ha.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://qh.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://so.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://mo.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://kb.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://dx.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oe.colortex.cn

Ruby: def to_s; @name; end
来源：http://bm.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://bu.panjiajie.cn

[G13] 判断对象类型
来源：http://ti.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://kt.hahajie.cn

PHP:  $u instanceof User
来源：http://me.521024.cn

JS:   u instanceof User
来源：http://dh.muxihuayi.cn

TS:   u instanceof User
来源：http://nx.nicolike.cn

Java: u instanceof User
来源：http://pd.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hi.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://va.muxihuayi.cn

C#:   u is User
来源：http://ld.szxytkj.cn

[G14] 数据类 / record
来源：http://zb.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ww.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://tw.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zv.521024.cn

TS:   type User = { name: string; age: number };
来源：http://wc.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://ix.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://fy.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cn.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://fo.nszjky.cn

[G15] 枚举
来源：http://cf.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qw.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qc.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ou.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uz.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://lk.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hw.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://gy.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fk.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ll.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ft.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://li.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://jg.nszjky.cn

TS:   Object.entries(obj)
来源：http://ic.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ty.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ak.shxzukj.cn

Ruby: obj.instance_variables
来源：http://cn.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://bw.asd995.cn

================================================================================
来源：http://iv.huanxung.cn

H. 异常与错误处理
来源：http://wr.nszjky.cn

================================================================================
来源：http://ce.9csxet.cn

[H01] try / catch 基础
来源：http://en.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yn.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ny.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oo.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lh.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tt.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tj.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jg.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dm.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://rp.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://st.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gb.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bu.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://up.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xq.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tw.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rc.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wl.asd995.cn

[H03] 主动抛出异常
来源：http://uy.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://fb.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ev.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://cn.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://du.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fl.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ie.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lo.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tv.jctech888.com.cn

[H04] 自定义异常类型
来源：http://ru.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://uf.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xe.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://fa.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://qc.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://fq.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ro.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://cw.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://jk.szxytkj.cn

[H05] 捕获特定类型
来源：http://od.9csxet.cn

Py:   except ValueError as e:
来源：http://ci.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eo.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://pd.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://xb.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://in.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vc.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://st.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cm.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://xp.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://xn.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://je.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qo.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ra.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kf.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qq.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://el.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://dh.huanxung.cn

[H07] 断言
来源：http://aa.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://ty.gzmigu.cn

PHP:  assert($x > 0);
来源：http://yg.521024.cn

JS:   console.assert(x > 0);
来源：http://hn.szsharing.cn

TS:   console.assert(x > 0);
来源：http://nw.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://dr.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ff.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ej.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://vu.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://iq.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://wh.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bt.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://ud.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://on.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cl.shxzukj.cn

Go:   err.Error()
来源：http://su.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://tg.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://ir.nicolike.cn

[H09] 带错误码的异常
来源：http://ki.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hf.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pc.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jf.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dm.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ce.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zy.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://we.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ps.521024.cn

[H10] 资源自动释放
来源：http://xj.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://of.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://og.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gs.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oq.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pw.lnxyls.cn

Go:   defer f.Close()
来源：http://xc.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bh.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ss.panjiajie.cn

================================================================================
来源：http://vm.bjjhwx.cn

I. 正则表达式
来源：http://oc.hahajie.cn

================================================================================
来源：http://et.jctech888.com.cn

[I01] 判断是否匹配
来源：http://cp.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ic.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gx.szsharing.cn

JS:   /\d+/.test(s)
来源：http://jv.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://ng.haigaiapp.cn


<!-- 参考信息 -->