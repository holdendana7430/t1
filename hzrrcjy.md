代发 wailian999

Ruby: File.delete("a.txt")
来源：http://bf.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://bh.nicolike.cn

[F07] 创建目录（含多级）
来源：http://hu.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xc.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pf.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bw.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zw.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rd.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jm.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bk.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mo.huanxung.cn

[F08] 遍历目录
来源：http://zh.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://co.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pz.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://gx.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://jl.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ks.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lk.newstarts.cn

Ruby: Dir.children("dir")
来源：http://cv.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://kz.nszjky.cn

[F09] 获取文件大小
来源：http://zd.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://jf.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://ax.521024.cn

JS:   fs.statSync("a.txt").size
来源：http://qj.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://al.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nc.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://av.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://wh.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://rn.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://du.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://si.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ap.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ho.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://eb.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pz.hahajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dz.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hi.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://do.shtwfgs.cn

[F11] 复制与移动文件
来源：http://lw.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://it.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://el.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nx.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://um.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xt.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://we.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hd.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rg.szxytkj.cn

[F12] CSV 读写
来源：http://qm.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hh.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gy.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xv.nszjky.cn

TS:   // 同上
来源：http://qk.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zj.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pw.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ug.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pa.huanxung.cn

================================================================================
来源：http://tj.jianghongdianzi.cn

G. 面向对象
来源：http://ee.jianghongdianzi.cn

================================================================================
来源：http://eg.bookmarksfly.cn

[G01] 定义类
来源：http://bi.newstarts.cn

Py:   class User: pass
来源：http://cv.huanxung.cn

PHP:  class User {}
来源：http://zh.szsharing.cn

JS:   class User {}
来源：http://rv.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://kk.huanxung.cn

Java: class User {}
来源：http://tl.521024.cn

Go:   type User struct { Name string }
来源：http://an.yuntaijiaju.cn

Ruby: class User; end
来源：http://uh.521024.cn

C#:   class User {}
来源：http://bu.huixinmuqiang.cn

[G02] 构造函数
来源：http://jl.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://gu.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://dh.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://sf.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://rt.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://qm.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ya.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://vi.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://yl.gzmigu.cn

[G03] 实例属性
来源：http://vg.hahajie.cn

Py:   self.name = "x"
来源：http://cc.asd995.cn

PHP:  public string $name = "x";
来源：http://be.newstarts.cn

JS:   this.name = "x";
来源：http://ev.bookmarksfly.cn

TS:   name: string = "x";
来源：http://xd.szxytkj.cn

Java: private String name;
来源：http://tk.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dl.colortex.cn

Ruby: @name = "x"
来源：http://rf.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://zq.panjiajie.cn

[G04] 定义方法
来源：http://ik.colortex.cn

Py:   def greet(self): return self.name
来源：http://xu.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fm.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://ok.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://zt.nicolike.cn

Java: String greet() { return name; }
来源：http://jv.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ip.gzmigu.cn

Ruby: def greet; @name; end
来源：http://hh.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://lu.panjiajie.cn

[G05] 继承
来源：http://og.521024.cn

Py:   class Admin(User): pass
来源：http://qu.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://gs.521024.cn

JS:   class Admin extends User {}
来源：http://ar.szsharing.cn

TS:   class Admin extends User {}
来源：http://up.hahajie.cn

Java: class Admin extends User {}
来源：http://pt.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pe.9csxet.cn

Ruby: class Admin < User; end
来源：http://rb.muxihuayi.cn

C#:   class Admin : User {}
来源：http://zy.chemitech.net.cn

[G06] 重写方法
来源：http://om.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://lj.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xh.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://cd.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ls.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://fa.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qu.521024.cn

Ruby: def greet; "admin"; end
来源：http://yb.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://ds.hahajie.cn

[G07] 调用父类方法
来源：http://do.jctech888.com.cn

Py:   super().greet()
来源：http://wc.panjiajie.cn

PHP:  parent::greet();
来源：http://rh.yuexingan06.cn

JS:   super.greet();
来源：http://nv.gzmigu.cn

TS:   super.greet();
来源：http://mc.nicolike.cn

Java: super.greet();
来源：http://zp.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nl.bookmarksfly.cn

Ruby: super
来源：http://sz.bookmarksfly.cn

C#:   base.Greet();
来源：http://si.521024.cn

[G08] 静态方法与属性
来源：http://pn.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hr.hahajie.cn

PHP:  public static function f() {}
来源：http://uf.shxzukj.cn

JS:   static f() {}
来源：http://mp.colortex.cn

TS:   static f(): void {}
来源：http://tt.huixinmuqiang.cn

Java: static void f() {}
来源：http://ss.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aj.shtwfgs.cn

Ruby: def self.f; end
来源：http://sx.jctech888.com.cn

C#:   public static void F() {}
来源：http://xl.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://rc.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://hd.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://js.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rx.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://yl.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://yf.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ek.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ch.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://wk.asd995.cn

[G10] 访问控制
来源：http://le.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://kn.wgjwhj.cn

PHP:  public / protected / private
来源：http://jg.nszjky.cn

JS:   #private 字段；其余公开
来源：http://am.szxytkj.cn

TS:   public / protected / private
来源：http://av.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://cf.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ox.newstarts.cn

Ruby: public / protected / private
来源：http://ut.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://hw.huixiangedu.cn

[G11] getter / setter
来源：http://vd.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://mc.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zv.szsharing.cn

JS:   get name() { return this._name; }
来源：http://wf.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://bd.szxytkj.cn

Java: public String getName() { return name; }
来源：http://ih.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rh.shxzskj.cn

Ruby: attr_accessor :name
来源：http://zb.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://dp.colortex.cn

[G12] 对象转字符串
来源：http://pq.colortex.cn

Py:   def __str__(self): return self.name
来源：http://mf.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vq.nicolike.cn

JS:   toString() { return this.name; }
来源：http://sy.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://ia.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://bt.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zx.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://gn.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://yn.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://zk.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://dp.haigaiapp.cn

PHP:  $u instanceof User
来源：http://ti.gzmigu.cn

JS:   u instanceof User
来源：http://yo.huixiangedu.cn

TS:   u instanceof User
来源：http://lf.521024.cn

Java: u instanceof User
来源：http://aw.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ds.nszjky.cn

Ruby: u.is_a?(User)
来源：http://ah.huixinmuqiang.cn

C#:   u is User
来源：http://li.newstarts.cn

[G14] 数据类 / record
来源：http://le.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sc.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://as.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aj.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://wo.asd995.cn

Java: record User(String name, int age) {}
来源：http://zt.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://mw.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rp.colortex.cn

C#:   record User(string Name, int Age);
来源：http://ob.lnxyls.cn

[G15] 枚举
来源：http://yv.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fj.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oi.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ob.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zg.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://me.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xn.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://ej.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pv.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://aa.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ob.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://ib.szsharing.cn

JS:   Object.entries(obj)
来源：http://me.panjiajie.cn

TS:   Object.entries(obj)
来源：http://tm.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cz.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://of.huanxung.cn

Ruby: obj.instance_variables
来源：http://si.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://ys.bookmarksfly.cn

================================================================================
来源：http://qm.jctech888.com.cn

H. 异常与错误处理
来源：http://ej.gzmigu.cn

================================================================================
来源：http://xm.yuexingan06.cn

[H01] try / catch 基础
来源：http://ut.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tn.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cu.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yc.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cv.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ww.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ft.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yf.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oo.asd995.cn

[H02] finally / ensure 收尾
来源：http://br.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ie.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rs.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tb.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hs.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zi.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yw.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wn.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jt.wgjwhj.cn

[H03] 主动抛出异常
来源：http://wv.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://oj.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bw.521024.cn

JS:   throw new Error("错误信息");
来源：http://po.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://pe.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dc.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://it.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wv.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://os.jctech888.com.cn

[H04] 自定义异常类型
来源：http://wx.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://vi.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kw.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://ia.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://yg.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://px.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://et.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://qz.hahajie.cn

C#:   class MyException : Exception {}
来源：http://go.shtwfgs.cn

[H05] 捕获特定类型
来源：http://de.hnjuh.cn

Py:   except ValueError as e:
来源：http://az.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zk.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://pp.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://mv.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://or.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gu.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://co.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gz.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://xt.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://sv.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hl.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://si.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ky.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bn.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://re.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://tt.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://xm.521024.cn

[H07] 断言
来源：http://vp.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://an.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://lm.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://ts.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://jx.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://kx.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cw.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://np.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://em.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://yx.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://er.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mw.nicolike.cn

JS:   e.message;  e.stack
来源：http://aa.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://re.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tg.jctech888.com.cn

Go:   err.Error()
来源：http://zh.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://cc.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://gy.yuexingan06.cn

[H09] 带错误码的异常
来源：http://bv.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pt.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://il.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hj.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://in.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xb.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ua.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pw.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aj.newstarts.cn

[H10] 资源自动释放
来源：http://jg.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://do.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fu.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pa.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jg.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oi.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://yf.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fo.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pd.nszjky.cn

================================================================================
来源：http://tk.panjiajie.cn

I. 正则表达式
来源：http://yu.yuntaijiaju.cn

================================================================================
来源：http://kn.haigaiapp.cn

[I01] 判断是否匹配
来源：http://gz.szsharing.cn


<!-- 参考信息 -->