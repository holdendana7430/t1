代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nf.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://al.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vt.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kt.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ll.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bm.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://po.shxzukj.cn

[F08] 遍历目录
来源：http://ih.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ko.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://de.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://ka.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://ph.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ow.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://my.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://yf.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://iz.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://iq.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://ty.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://qe.wgjwhj.cn

JS:   fs.statSync("a.txt").size
来源：http://ry.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://hi.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://co.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mi.hahajie.cn

Ruby: File.size("a.txt")
来源：http://iq.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://qk.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://ko.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cf.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gd.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://se.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://bp.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://be.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tl.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pe.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://az.hahajie.cn

[F11] 复制与移动文件
来源：http://fn.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nq.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tz.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fu.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sn.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mh.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://it.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ye.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gi.gzmigu.cn

[F12] CSV 读写
来源：http://cz.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iv.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ge.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kn.chemitech.net.cn

TS:   // 同上
来源：http://nd.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mv.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mx.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vl.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wp.521024.cn

================================================================================
来源：http://kb.wgjwhj.cn

G. 面向对象
来源：http://hs.nszjky.cn

================================================================================
来源：http://od.lnxyls.cn

[G01] 定义类
来源：http://ox.bookmarksfly.cn

Py:   class User: pass
来源：http://if.hahajie.cn

PHP:  class User {}
来源：http://nv.nicolike.cn

JS:   class User {}
来源：http://ag.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://oc.gzmigu.cn

Java: class User {}
来源：http://rv.lnxyls.cn

Go:   type User struct { Name string }
来源：http://wy.newstarts.cn

Ruby: class User; end
来源：http://wr.colortex.cn

C#:   class User {}
来源：http://bp.gzmigu.cn

[G02] 构造函数
来源：http://ou.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://gr.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://yc.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://si.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://yd.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://yt.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sj.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://et.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://eq.chemitech.net.cn

[G03] 实例属性
来源：http://my.bookmarksfly.cn

Py:   self.name = "x"
来源：http://ul.asd995.cn

PHP:  public string $name = "x";
来源：http://cb.szxytkj.cn

JS:   this.name = "x";
来源：http://dd.nicolike.cn

TS:   name: string = "x";
来源：http://mr.huixinmuqiang.cn

Java: private String name;
来源：http://dw.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ar.bjjhwx.cn

Ruby: @name = "x"
来源：http://bo.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://vz.hahajie.cn

[G04] 定义方法
来源：http://tr.nszjky.cn

Py:   def greet(self): return self.name
来源：http://jv.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kw.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://of.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://dw.muxihuayi.cn

Java: String greet() { return name; }
来源：http://im.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fl.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://tf.521024.cn

C#:   public string Greet() => Name;
来源：http://ku.chemitech.net.cn

[G05] 继承
来源：http://lc.hahajie.cn

Py:   class Admin(User): pass
来源：http://iv.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://zt.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://nn.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ej.521024.cn

Java: class Admin extends User {}
来源：http://sd.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zv.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://sr.hahajie.cn

C#:   class Admin : User {}
来源：http://fz.colortex.cn

[G06] 重写方法
来源：http://li.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://gn.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bb.521024.cn

JS:   greet() { return "admin"; }
来源：http://pe.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://zn.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://od.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pz.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://lj.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://xu.haigaiapp.cn

[G07] 调用父类方法
来源：http://br.huanxung.cn

Py:   super().greet()
来源：http://sd.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://em.hahajie.cn

JS:   super.greet();
来源：http://gr.hahajie.cn

TS:   super.greet();
来源：http://np.shtwfgs.cn

Java: super.greet();
来源：http://dn.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ef.szsharing.cn

Ruby: super
来源：http://nu.shtwfgs.cn

C#:   base.Greet();
来源：http://gs.bjjhwx.cn

[G08] 静态方法与属性
来源：http://ed.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fm.yuexingan06.cn

PHP:  public static function f() {}
来源：http://mq.yuexingan06.cn

JS:   static f() {}
来源：http://tf.nszjky.cn

TS:   static f(): void {}
来源：http://qa.haigaiapp.cn

Java: static void f() {}
来源：http://kn.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aq.newstarts.cn

Ruby: def self.f; end
来源：http://zz.huixiangedu.cn

C#:   public static void F() {}
来源：http://ru.521024.cn

[G09] 接口 / 抽象类
来源：http://sd.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://dc.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tb.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bu.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://el.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://ho.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://qa.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ph.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://cg.szsharing.cn

[G10] 访问控制
来源：http://tq.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://ci.shxzukj.cn

PHP:  public / protected / private
来源：http://hd.hahajie.cn

JS:   #private 字段；其余公开
来源：http://lc.yuexingan06.cn

TS:   public / protected / private
来源：http://vz.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://yv.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cb.shxzukj.cn

Ruby: public / protected / private
来源：http://ph.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://wk.huanxung.cn

[G11] getter / setter
来源：http://dy.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://cl.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qj.newstarts.cn

JS:   get name() { return this._name; }
来源：http://za.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://zc.gzmigu.cn

Java: public String getName() { return name; }
来源：http://hq.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ra.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://gy.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://gx.wgjwhj.cn

[G12] 对象转字符串
来源：http://km.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://yx.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vc.colortex.cn

JS:   toString() { return this.name; }
来源：http://vy.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://au.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://im.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bs.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://xi.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://ne.shxzskj.cn

[G13] 判断对象类型
来源：http://ev.huanxung.cn

Py:   isinstance(u, User)
来源：http://bj.huixiangedu.cn

PHP:  $u instanceof User
来源：http://ej.hnjuh.cn

JS:   u instanceof User
来源：http://wf.yuexingan06.cn

TS:   u instanceof User
来源：http://ws.szsharing.cn

Java: u instanceof User
来源：http://bn.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ow.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://fv.bookmarksfly.cn

C#:   u is User
来源：http://ar.521024.cn

[G14] 数据类 / record
来源：http://wk.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mj.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://fd.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ct.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://hm.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://vi.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://wt.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yv.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://iz.hnjuh.cn

[G15] 枚举
来源：http://if.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xl.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zi.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vq.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uo.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://pv.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://an.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://ul.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hd.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://ra.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://by.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://by.newstarts.cn

JS:   Object.entries(obj)
来源：http://at.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://xq.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://li.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://om.gzmigu.cn

Ruby: obj.instance_variables
来源：http://ji.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://es.521024.cn

================================================================================
来源：http://rp.nszjky.cn

H. 异常与错误处理
来源：http://yx.muxihuayi.cn

================================================================================
来源：http://mn.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://pn.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wl.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eg.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://in.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tn.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://al.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pa.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://he.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xm.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://kc.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lu.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pr.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yj.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jp.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zf.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qv.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yq.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ju.shxzukj.cn

[H03] 主动抛出异常
来源：http://th.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://ln.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ot.521024.cn

JS:   throw new Error("错误信息");
来源：http://kz.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://bf.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iq.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xv.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mf.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yr.newstarts.cn

[H04] 自定义异常类型
来源：http://gk.521024.cn

Py:   class MyError(Exception): pass
来源：http://sv.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nk.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://xu.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://xq.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://sf.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hv.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://is.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://py.panjiajie.cn

[H05] 捕获特定类型
来源：http://kv.haigaiapp.cn

Py:   except ValueError as e:
来源：http://mc.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yj.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://al.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://xd.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://vr.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zq.521024.cn

Ruby: rescue ArgumentError => e
来源：http://aq.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qe.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://gy.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://jk.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qv.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hc.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dw.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ha.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ig.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://as.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://tu.huixinmuqiang.cn

[H07] 断言
来源：http://pc.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ol.9csxet.cn

PHP:  assert($x > 0);
来源：http://sk.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://qj.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://we.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://qm.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bj.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ec.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://ip.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://kr.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://yq.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://go.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://zn.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ia.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ys.jianghongdianzi.cn

Go:   err.Error()
来源：http://nw.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://go.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://ya.shxzukj.cn

[H09] 带错误码的异常
来源：http://uz.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pq.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ja.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qx.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jx.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qa.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zy.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bz.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fq.wgjwhj.cn

[H10] 资源自动释放
来源：http://tq.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xg.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fr.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sg.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vu.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ia.hnjuh.cn

Go:   defer f.Close()
来源：http://qm.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uc.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ex.yuexingan06.cn

================================================================================
来源：http://bk.haigaiapp.cn

I. 正则表达式
来源：http://ji.521024.cn

================================================================================
来源：http://wj.521024.cn

[I01] 判断是否匹配
来源：http://fu.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lt.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dn.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://pd.colortex.cn

TS:   /\d+/.test(s)
来源：http://re.huixinmuqiang.cn


<!-- 参考信息 -->