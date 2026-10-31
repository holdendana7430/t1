代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qm.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hr.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ze.yuntaijiaju.cn

[F08] 遍历目录
来源：http://iv.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jd.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sm.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://te.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://vu.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ja.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bg.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://iu.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://xg.huanxung.cn

[F09] 获取文件大小
来源：http://ve.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://hv.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://bf.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://sn.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://lm.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kf.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://un.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://gn.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://dm.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://ym.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cd.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kx.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jq.colortex.cn

TS:   path.extname("a.txt")
来源：http://fa.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://in.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://km.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://du.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mu.yuexingan06.cn

[F11] 复制与移动文件
来源：http://iy.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ju.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vm.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dj.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xh.shxzskj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://np.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zj.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xk.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mp.hahajie.cn

[F12] CSV 读写
来源：http://wa.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vr.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zx.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fw.jianghongdianzi.cn

TS:   // 同上
来源：http://ir.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rx.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xm.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wt.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://od.newstarts.cn

================================================================================
来源：http://qc.asd995.cn

G. 面向对象
来源：http://xw.nicolike.cn

================================================================================
来源：http://nf.yuexingan06.cn

[G01] 定义类
来源：http://wx.haigaiapp.cn

Py:   class User: pass
来源：http://pa.gzmigu.cn

PHP:  class User {}
来源：http://ph.gzmigu.cn

JS:   class User {}
来源：http://lh.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://bp.521024.cn

Java: class User {}
来源：http://zq.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://qk.newstarts.cn

Ruby: class User; end
来源：http://cs.muxihuayi.cn

C#:   class User {}
来源：http://bh.nszjky.cn

[G02] 构造函数
来源：http://lc.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://ol.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://fj.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://hb.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://yy.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://jc.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nt.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://hg.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://wt.hnjuh.cn

[G03] 实例属性
来源：http://lr.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://cv.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://db.9csxet.cn

JS:   this.name = "x";
来源：http://ng.nicolike.cn

TS:   name: string = "x";
来源：http://sg.wgjwhj.cn

Java: private String name;
来源：http://vw.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mh.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://sc.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://re.shxzskj.cn

[G04] 定义方法
来源：http://xa.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://pv.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://at.nszjky.cn

JS:   greet() { return this.name; }
来源：http://aa.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://nq.hahajie.cn

Java: String greet() { return name; }
来源：http://od.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://do.szsharing.cn

Ruby: def greet; @name; end
来源：http://sh.nszjky.cn

C#:   public string Greet() => Name;
来源：http://td.hahajie.cn

[G05] 继承
来源：http://ww.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://no.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://bn.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://rr.521024.cn

TS:   class Admin extends User {}
来源：http://bq.asd995.cn

Java: class Admin extends User {}
来源：http://sd.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dc.shxzskj.cn

Ruby: class Admin < User; end
来源：http://ak.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://zb.nicolike.cn

[G06] 重写方法
来源：http://bj.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://wu.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ei.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ep.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://kg.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://nf.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fb.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://rq.521024.cn

C#:   public override string Greet() => "admin";
来源：http://zi.muxihuayi.cn

[G07] 调用父类方法
来源：http://pc.yuexingan06.cn

Py:   super().greet()
来源：http://yl.szsharing.cn

PHP:  parent::greet();
来源：http://vy.szsharing.cn

JS:   super.greet();
来源：http://bi.szxytkj.cn

TS:   super.greet();
来源：http://wo.yuexingan06.cn

Java: super.greet();
来源：http://kb.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ws.newstarts.cn

Ruby: super
来源：http://of.muxihuayi.cn

C#:   base.Greet();
来源：http://kk.shxzskj.cn

[G08] 静态方法与属性
来源：http://ep.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ld.hahajie.cn

PHP:  public static function f() {}
来源：http://bn.szxytkj.cn

JS:   static f() {}
来源：http://si.huanxung.cn

TS:   static f(): void {}
来源：http://la.wgjwhj.cn

Java: static void f() {}
来源：http://sy.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://om.wgjwhj.cn

Ruby: def self.f; end
来源：http://pj.szxytkj.cn

C#:   public static void F() {}
来源：http://ze.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://hi.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://yk.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sz.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sr.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://nl.colortex.cn

Java: interface Shape { double area(); }
来源：http://ck.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://sd.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qs.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://oe.asd995.cn

[G10] 访问控制
来源：http://rb.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://xa.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://ds.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://te.jctech888.com.cn

TS:   public / protected / private
来源：http://sw.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://it.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wl.szsharing.cn

Ruby: public / protected / private
来源：http://hj.gzmigu.cn

C#:   public / protected / private / internal
来源：http://dc.521024.cn

[G11] getter / setter
来源：http://el.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://pd.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://le.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://ui.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://lv.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://cq.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ip.nszjky.cn

Ruby: attr_accessor :name
来源：http://tf.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://hq.lnxyls.cn

[G12] 对象转字符串
来源：http://el.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://xl.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yp.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://st.521024.cn

TS:   toString(): string { return this.name; }
来源：http://xc.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://en.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bt.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://po.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://ot.lnxyls.cn

[G13] 判断对象类型
来源：http://uf.9csxet.cn

Py:   isinstance(u, User)
来源：http://jo.gzmigu.cn

PHP:  $u instanceof User
来源：http://sn.szsharing.cn

JS:   u instanceof User
来源：http://qw.9csxet.cn

TS:   u instanceof User
来源：http://oo.hnjuh.cn

Java: u instanceof User
来源：http://mi.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ea.colortex.cn

Ruby: u.is_a?(User)
来源：http://zd.muxihuayi.cn

C#:   u is User
来源：http://vz.huanxung.cn

[G14] 数据类 / record
来源：http://vp.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fl.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://ur.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iu.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://ge.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://jh.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://gv.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ao.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://hc.lnxyls.cn

[G15] 枚举
来源：http://xl.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ya.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qf.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ua.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://em.521024.cn

Java: enum Color { RED, GREEN }
来源：http://iy.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pj.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://ld.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hf.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://wi.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cx.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://xe.shxzukj.cn

JS:   Object.entries(obj)
来源：http://bd.szsharing.cn

TS:   Object.entries(obj)
来源：http://bl.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rv.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vr.panjiajie.cn

Ruby: obj.instance_variables
来源：http://jy.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://us.shxzskj.cn

================================================================================
来源：http://fi.chemitech.net.cn

H. 异常与错误处理
来源：http://oj.bjjhwx.cn

================================================================================
来源：http://hr.shtwfgs.cn

[H01] try / catch 基础
来源：http://dc.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lz.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vp.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qh.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zc.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rj.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iy.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ak.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uh.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://re.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qh.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jl.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://av.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xb.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wy.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kd.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://an.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vz.muxihuayi.cn

[H03] 主动抛出异常
来源：http://gq.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://hs.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rv.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://yo.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://xn.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yd.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fa.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xb.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lv.asd995.cn

[H04] 自定义异常类型
来源：http://bh.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://yj.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cl.szsharing.cn

JS:   class MyError extends Error {}
来源：http://vx.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://nb.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://zz.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vs.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://ol.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://cg.shxzukj.cn

[H05] 捕获特定类型
来源：http://px.jctech888.com.cn

Py:   except ValueError as e:
来源：http://gu.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zb.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://nn.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://ox.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://au.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://px.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://pc.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ts.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ec.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://aq.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zy.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tt.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cd.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pw.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://au.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://ji.521024.cn

C#:   obj?.A?.B ?? default
来源：http://cc.bjjhwx.cn

[H07] 断言
来源：http://bd.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://ck.521024.cn

PHP:  assert($x > 0);
来源：http://zg.asd995.cn

JS:   console.assert(x > 0);
来源：http://vh.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://sp.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://nk.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jn.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vy.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://cw.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://ct.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://lx.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ck.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://cz.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mb.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zm.shxzukj.cn

Go:   err.Error()
来源：http://st.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://zp.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://tr.hahajie.cn

[H09] 带错误码的异常
来源：http://fc.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://um.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://an.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pp.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wo.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rs.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ft.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://um.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hd.9csxet.cn

[H10] 资源自动释放
来源：http://xk.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://in.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://at.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sk.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fu.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fi.521024.cn

Go:   defer f.Close()
来源：http://ec.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bf.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://px.hnjuh.cn

================================================================================
来源：http://sr.asd995.cn

I. 正则表达式
来源：http://zl.newstarts.cn

================================================================================
来源：http://lr.huanxung.cn

[I01] 判断是否匹配
来源：http://fm.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cp.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ya.szsharing.cn

JS:   /\d+/.test(s)
来源：http://mv.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://mn.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oa.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uq.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://wx.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bm.panjiajie.cn


<!-- 参考信息 -->