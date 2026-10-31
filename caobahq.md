代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kz.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rh.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ud.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vz.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tv.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ng.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bn.asd995.cn

[F08] 遍历目录
来源：http://qz.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vc.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lu.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://on.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://do.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://od.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://es.asd995.cn

Ruby: Dir.children("dir")
来源：http://zw.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://aa.nicolike.cn

[F09] 获取文件大小
来源：http://mi.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://vw.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://hj.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://ec.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://sc.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ar.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ie.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://bh.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://hy.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://gb.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jq.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cj.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fa.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://iz.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gl.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bg.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://px.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ly.panjiajie.cn

[F11] 复制与移动文件
来源：http://hm.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bi.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wl.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zz.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://im.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://no.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fj.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wg.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wz.haigaiapp.cn

[F12] CSV 读写
来源：http://dr.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eh.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uu.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ne.yuntaijiaju.cn

TS:   // 同上
来源：http://hg.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jk.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gl.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kv.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lk.nszjky.cn

================================================================================
来源：http://zd.muxihuayi.cn

G. 面向对象
来源：http://nv.chemitech.net.cn

================================================================================
来源：http://vy.9csxet.cn

[G01] 定义类
来源：http://tz.szxytkj.cn

Py:   class User: pass
来源：http://li.nicolike.cn

PHP:  class User {}
来源：http://xf.bookmarksfly.cn

JS:   class User {}
来源：http://wg.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://sw.9csxet.cn

Java: class User {}
来源：http://lu.szsharing.cn

Go:   type User struct { Name string }
来源：http://yn.panjiajie.cn

Ruby: class User; end
来源：http://xw.jctech888.com.cn

C#:   class User {}
来源：http://xr.wgjwhj.cn

[G02] 构造函数
来源：http://lf.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://ka.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://jw.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://kj.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://mq.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://go.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vr.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://vd.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://pg.nszjky.cn

[G03] 实例属性
来源：http://tc.hahajie.cn

Py:   self.name = "x"
来源：http://xa.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://qh.huanxung.cn

JS:   this.name = "x";
来源：http://yq.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://qb.hahajie.cn

Java: private String name;
来源：http://uv.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cy.huanxung.cn

Ruby: @name = "x"
来源：http://fo.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://sn.jianghongdianzi.cn

[G04] 定义方法
来源：http://rm.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://xd.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oq.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://uu.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://ij.asd995.cn

Java: String greet() { return name; }
来源：http://bb.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qa.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://hv.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://uh.yuexingan06.cn

[G05] 继承
来源：http://ni.hnjuh.cn

Py:   class Admin(User): pass
来源：http://ps.huanxung.cn

PHP:  class Admin extends User {}
来源：http://lt.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://wq.colortex.cn

TS:   class Admin extends User {}
来源：http://ji.hnjuh.cn

Java: class Admin extends User {}
来源：http://co.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zp.asd995.cn

Ruby: class Admin < User; end
来源：http://vh.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://mu.yuntaijiaju.cn

[G06] 重写方法
来源：http://ri.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://hu.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wo.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://nt.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://bb.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://hw.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ra.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://nx.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://vu.panjiajie.cn

[G07] 调用父类方法
来源：http://vp.szxytkj.cn

Py:   super().greet()
来源：http://hi.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://gg.nszjky.cn

JS:   super.greet();
来源：http://eg.szxytkj.cn

TS:   super.greet();
来源：http://sb.yuntaijiaju.cn

Java: super.greet();
来源：http://dr.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ov.huixinmuqiang.cn

Ruby: super
来源：http://kl.9csxet.cn

C#:   base.Greet();
来源：http://mz.hahajie.cn

[G08] 静态方法与属性
来源：http://ar.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wd.gzmigu.cn

PHP:  public static function f() {}
来源：http://ln.shxzskj.cn

JS:   static f() {}
来源：http://mp.panjiajie.cn

TS:   static f(): void {}
来源：http://jo.gzmigu.cn

Java: static void f() {}
来源：http://fz.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jz.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://af.lnxyls.cn

C#:   public static void F() {}
来源：http://ur.nszjky.cn

[G09] 接口 / 抽象类
来源：http://av.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://di.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pk.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ck.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://pt.9csxet.cn

Java: interface Shape { double area(); }
来源：http://lc.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://el.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fb.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://xx.panjiajie.cn

[G10] 访问控制
来源：http://uo.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://fb.haigaiapp.cn

PHP:  public / protected / private
来源：http://dp.huanxung.cn

JS:   #private 字段；其余公开
来源：http://yu.lnxyls.cn

TS:   public / protected / private
来源：http://zy.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://bt.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://of.haigaiapp.cn

Ruby: public / protected / private
来源：http://fx.521024.cn

C#:   public / protected / private / internal
来源：http://gv.haigaiapp.cn

[G11] getter / setter
来源：http://bh.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://zf.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zj.asd995.cn

JS:   get name() { return this._name; }
来源：http://dr.521024.cn

TS:   get name(): string { return this._name; }
来源：http://er.asd995.cn

Java: public String getName() { return name; }
来源：http://hv.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ap.nicolike.cn

Ruby: attr_accessor :name
来源：http://fw.szsharing.cn

C#:   public string Name { get; set; }
来源：http://wb.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://ix.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://qw.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ll.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://zj.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://qf.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://ox.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nr.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://tb.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://hi.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://th.panjiajie.cn

Py:   isinstance(u, User)
来源：http://ef.panjiajie.cn

PHP:  $u instanceof User
来源：http://rl.asd995.cn

JS:   u instanceof User
来源：http://zl.shxzukj.cn

TS:   u instanceof User
来源：http://vx.gzmigu.cn

Java: u instanceof User
来源：http://jp.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vr.asd995.cn

Ruby: u.is_a?(User)
来源：http://ay.bookmarksfly.cn

C#:   u is User
来源：http://uo.szsharing.cn

[G14] 数据类 / record
来源：http://jh.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jn.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://jz.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lp.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://ex.colortex.cn

Java: record User(String name, int age) {}
来源：http://jk.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://hg.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pf.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://mf.nszjky.cn

[G15] 枚举
来源：http://qb.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ff.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tc.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wh.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://si.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://qk.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://je.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://ps.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dd.asd995.cn

[G16] 对象转数组 / 字典
来源：http://qm.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tn.colortex.cn

PHP:  get_object_vars($obj);
来源：http://op.hahajie.cn

JS:   Object.entries(obj)
来源：http://ee.gzmigu.cn

TS:   Object.entries(obj)
来源：http://wo.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zj.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ex.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://lu.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://hx.nicolike.cn

================================================================================
来源：http://zj.bjjhwx.cn

H. 异常与错误处理
来源：http://zl.huanxung.cn

================================================================================
来源：http://nl.lnxyls.cn

[H01] try / catch 基础
来源：http://lq.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qq.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gz.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yi.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zb.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pu.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mm.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xl.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://id.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://rf.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pr.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xe.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xg.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rk.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uq.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hr.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ax.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rg.jctech888.com.cn

[H03] 主动抛出异常
来源：http://ep.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://hi.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mu.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://ka.521024.cn

TS:   throw new Error("错误信息");
来源：http://ic.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vf.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jf.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ny.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://df.lnxyls.cn

[H04] 自定义异常类型
来源：http://sz.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://uu.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ym.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ar.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ac.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://wo.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yn.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://kj.9csxet.cn

C#:   class MyException : Exception {}
来源：http://nt.9csxet.cn

[H05] 捕获特定类型
来源：http://no.colortex.cn

Py:   except ValueError as e:
来源：http://ib.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wy.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://lz.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://cb.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://rb.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xg.521024.cn

Ruby: rescue ArgumentError => e
来源：http://oi.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uu.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://nf.nicolike.cn

Py:   value = d.get("k") or default
来源：http://or.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qf.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qn.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pm.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://es.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eh.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://ct.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://hq.hnjuh.cn

[H07] 断言
来源：http://gy.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://et.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://og.nicolike.cn

JS:   console.assert(x > 0);
来源：http://fv.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://og.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://ir.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kq.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ob.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://el.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://lu.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://wc.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bv.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://mt.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ft.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hx.lnxyls.cn

Go:   err.Error()
来源：http://cm.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://tm.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://gq.szsharing.cn

[H09] 带错误码的异常
来源：http://df.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vu.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sv.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uo.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gc.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nh.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://un.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pk.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nh.muxihuayi.cn

[H10] 资源自动释放
来源：http://mo.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sy.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ks.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dz.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ma.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bk.chemitech.net.cn

Go:   defer f.Close()
来源：http://mu.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kk.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pm.nszjky.cn

================================================================================
来源：http://pl.huanxung.cn

I. 正则表达式
来源：http://nj.gzmigu.cn

================================================================================
来源：http://mq.haigaiapp.cn

[I01] 判断是否匹配
来源：http://kq.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vc.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bi.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://wk.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://pb.bookmarksfly.cn


<!-- 参考信息 -->