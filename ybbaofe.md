代发 wailian999

Ruby: File.delete("a.txt")
来源：http://pd.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://es.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://uo.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://np.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kg.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bn.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ey.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fi.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bw.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lq.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fc.huanxung.cn

[F08] 遍历目录
来源：http://rg.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gm.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ea.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ih.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://kn.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gj.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dd.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://ge.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://gw.lnxyls.cn

[F09] 获取文件大小
来源：http://uf.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://bu.nszjky.cn

PHP:  filesize("a.txt");
来源：http://zz.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://nt.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://uo.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pc.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xd.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://hp.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://mx.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://rp.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://od.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ns.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ag.nszjky.cn

TS:   path.extname("a.txt")
来源：http://gj.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lp.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zg.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wi.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ma.haigaiapp.cn

[F11] 复制与移动文件
来源：http://yt.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zh.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mz.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://av.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ai.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nu.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cn.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wn.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kn.521024.cn

[F12] CSV 读写
来源：http://eh.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cs.gzmigu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zp.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tq.szxytkj.cn

TS:   // 同上
来源：http://ru.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ke.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lv.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yf.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ka.9csxet.cn

================================================================================
来源：http://hd.huanxung.cn

G. 面向对象
来源：http://wx.jctech888.com.cn

================================================================================
来源：http://ck.huixinmuqiang.cn

[G01] 定义类
来源：http://td.shxzukj.cn

Py:   class User: pass
来源：http://fd.szsharing.cn

PHP:  class User {}
来源：http://xy.hnjuh.cn

JS:   class User {}
来源：http://mq.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://cd.huanxung.cn

Java: class User {}
来源：http://wu.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://ea.bookmarksfly.cn

Ruby: class User; end
来源：http://at.szsharing.cn

C#:   class User {}
来源：http://po.shxzskj.cn

[G02] 构造函数
来源：http://qm.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://wp.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://ln.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://qd.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://zo.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://wi.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xf.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://vg.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://bw.lnxyls.cn

[G03] 实例属性
来源：http://pl.huixiangedu.cn

Py:   self.name = "x"
来源：http://oc.asd995.cn

PHP:  public string $name = "x";
来源：http://ry.jctech888.com.cn

JS:   this.name = "x";
来源：http://bc.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://mq.huixiangedu.cn

Java: private String name;
来源：http://op.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ti.gzmigu.cn

Ruby: @name = "x"
来源：http://ru.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://oa.szxytkj.cn

[G04] 定义方法
来源：http://uo.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://ur.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iz.9csxet.cn

JS:   greet() { return this.name; }
来源：http://tr.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://pg.asd995.cn

Java: String greet() { return name; }
来源：http://yw.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tq.huanxung.cn

Ruby: def greet; @name; end
来源：http://cb.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://wd.colortex.cn

[G05] 继承
来源：http://sw.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://jy.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://rc.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://cw.huanxung.cn

TS:   class Admin extends User {}
来源：http://hf.haigaiapp.cn

Java: class Admin extends User {}
来源：http://jm.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sp.gzmigu.cn

Ruby: class Admin < User; end
来源：http://ze.huixiangedu.cn

C#:   class Admin : User {}
来源：http://vi.shxzskj.cn

[G06] 重写方法
来源：http://gr.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://ll.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mi.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://ql.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://mk.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://qr.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wy.colortex.cn

Ruby: def greet; "admin"; end
来源：http://az.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://xk.colortex.cn

[G07] 调用父类方法
来源：http://va.szsharing.cn

Py:   super().greet()
来源：http://pi.szxytkj.cn

PHP:  parent::greet();
来源：http://dv.shxzskj.cn

JS:   super.greet();
来源：http://az.panjiajie.cn

TS:   super.greet();
来源：http://lh.muxihuayi.cn

Java: super.greet();
来源：http://hz.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bu.newstarts.cn

Ruby: super
来源：http://st.bjjhwx.cn

C#:   base.Greet();
来源：http://ec.panjiajie.cn

[G08] 静态方法与属性
来源：http://ub.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bw.asd995.cn

PHP:  public static function f() {}
来源：http://dz.shtwfgs.cn

JS:   static f() {}
来源：http://al.asd995.cn

TS:   static f(): void {}
来源：http://dx.bookmarksfly.cn

Java: static void f() {}
来源：http://tx.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://za.wgjwhj.cn

Ruby: def self.f; end
来源：http://wt.hahajie.cn

C#:   public static void F() {}
来源：http://mq.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://vo.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://zw.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ka.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://od.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://wq.nicolike.cn

Java: interface Shape { double area(); }
来源：http://rg.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://si.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cx.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://gt.asd995.cn

[G10] 访问控制
来源：http://cr.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://rj.wgjwhj.cn

PHP:  public / protected / private
来源：http://by.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://ki.gzmigu.cn

TS:   public / protected / private
来源：http://as.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://ey.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://de.haigaiapp.cn

Ruby: public / protected / private
来源：http://dd.shxzskj.cn

C#:   public / protected / private / internal
来源：http://ud.wgjwhj.cn

[G11] getter / setter
来源：http://zs.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://gd.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qa.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://nk.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://cn.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://dk.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ex.nicolike.cn

Ruby: attr_accessor :name
来源：http://px.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ik.szxytkj.cn

[G12] 对象转字符串
来源：http://iz.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://vs.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kv.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://di.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://gj.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://gx.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mr.szsharing.cn

Ruby: def to_s; @name; end
来源：http://nf.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://wj.shxzskj.cn

[G13] 判断对象类型
来源：http://ie.9csxet.cn

Py:   isinstance(u, User)
来源：http://fz.panjiajie.cn

PHP:  $u instanceof User
来源：http://yo.panjiajie.cn

JS:   u instanceof User
来源：http://tk.huixiangedu.cn

TS:   u instanceof User
来源：http://on.haigaiapp.cn

Java: u instanceof User
来源：http://sx.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ub.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://zi.huixinmuqiang.cn

C#:   u is User
来源：http://oc.bjjhwx.cn

[G14] 数据类 / record
来源：http://mn.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://me.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://dv.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dh.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://bm.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://ta.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://xb.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xy.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://eh.huanxung.cn

[G15] 枚举
来源：http://oz.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zx.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wk.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fl.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ul.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://vq.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iv.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://wz.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://df.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://md.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hv.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://ab.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://pj.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://jp.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iw.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dn.huanxung.cn

Ruby: obj.instance_variables
来源：http://bh.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://bk.asd995.cn

================================================================================
来源：http://ml.huanxung.cn

H. 异常与错误处理
来源：http://ng.newstarts.cn

================================================================================
来源：http://vy.bookmarksfly.cn

[H01] try / catch 基础
来源：http://rp.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sh.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://is.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gl.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ne.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pf.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bl.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uw.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kl.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://zv.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rs.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rr.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lu.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ny.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ug.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vg.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pe.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hu.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://qs.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://pv.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wu.521024.cn

JS:   throw new Error("错误信息");
来源：http://qw.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://ir.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zt.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gb.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ig.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xf.jctech888.com.cn

[H04] 自定义异常类型
来源：http://rm.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://vg.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eo.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://wn.nicolike.cn

TS:   class MyError extends Error {}
来源：http://km.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://kz.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lf.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://xk.asd995.cn

C#:   class MyException : Exception {}
来源：http://ca.huixiangedu.cn

[H05] 捕获特定类型
来源：http://my.shtwfgs.cn

Py:   except ValueError as e:
来源：http://nx.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ws.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ri.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://pu.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://yc.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bh.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://mu.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jj.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://tz.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://sh.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uv.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nk.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vd.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tf.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://od.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://of.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://un.yuexingan06.cn

[H07] 断言
来源：http://gl.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://fy.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://bk.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://eu.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://hr.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://zc.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cp.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://al.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://xp.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://zt.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://jy.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rh.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://no.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://di.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ze.colortex.cn

Go:   err.Error()
来源：http://bm.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://qb.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://fy.yuexingan06.cn

[H09] 带错误码的异常
来源：http://vb.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mn.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://je.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wy.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ft.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fz.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yr.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://so.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oq.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://ro.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pz.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ta.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pv.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sc.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uv.colortex.cn

Go:   defer f.Close()
来源：http://xv.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hs.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ki.nszjky.cn

================================================================================
来源：http://ab.9csxet.cn

I. 正则表达式
来源：http://by.hahajie.cn

================================================================================
来源：http://vt.521024.cn

[I01] 判断是否匹配
来源：http://je.huixinmuqiang.cn


<!-- 参考信息 -->