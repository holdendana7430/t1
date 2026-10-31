代发 wailian999

Ruby: File.delete("a.txt")
来源：http://xd.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://oe.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://rk.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ck.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://or.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rt.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bt.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ur.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vt.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sf.shxzukj.cn

[F08] 遍历目录
来源：http://ev.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ow.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wl.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://ki.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://na.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pf.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ld.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://ch.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://nu.521024.cn

[F09] 获取文件大小
来源：http://nk.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://fl.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://he.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://kn.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://vf.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yt.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gn.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://rv.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://uz.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://mv.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jv.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zt.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rj.asd995.cn

TS:   path.extname("a.txt")
来源：http://ow.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fe.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://em.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jx.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uj.hnjuh.cn

[F11] 复制与移动文件
来源：http://lv.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ls.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sk.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wg.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cy.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hf.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xp.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://at.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fh.panjiajie.cn

[F12] CSV 读写
来源：http://wd.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ai.nicolike.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://em.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oa.hnjuh.cn

TS:   // 同上
来源：http://wu.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ou.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tn.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gp.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qv.yuexingan06.cn

================================================================================
来源：http://zx.huixinmuqiang.cn

G. 面向对象
来源：http://hk.newstarts.cn

================================================================================
来源：http://ls.gzmigu.cn

[G01] 定义类
来源：http://rb.nszjky.cn

Py:   class User: pass
来源：http://cg.panjiajie.cn

PHP:  class User {}
来源：http://kw.hnjuh.cn

JS:   class User {}
来源：http://xh.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://jk.bjjhwx.cn

Java: class User {}
来源：http://nn.asd995.cn

Go:   type User struct { Name string }
来源：http://wc.szxytkj.cn

Ruby: class User; end
来源：http://la.hahajie.cn

C#:   class User {}
来源：http://vm.colortex.cn

[G02] 构造函数
来源：http://yv.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://lh.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://uo.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://ps.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://yw.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://tu.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://to.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ze.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://hh.9csxet.cn

[G03] 实例属性
来源：http://pv.nicolike.cn

Py:   self.name = "x"
来源：http://qv.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://cp.lnxyls.cn

JS:   this.name = "x";
来源：http://su.hahajie.cn

TS:   name: string = "x";
来源：http://oc.hahajie.cn

Java: private String name;
来源：http://gr.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ip.yuexingan06.cn

Ruby: @name = "x"
来源：http://tw.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://pn.chemitech.net.cn

[G04] 定义方法
来源：http://px.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://gs.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sk.szsharing.cn

JS:   greet() { return this.name; }
来源：http://pk.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://hv.huixiangedu.cn

Java: String greet() { return name; }
来源：http://uu.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xy.shxzukj.cn

Ruby: def greet; @name; end
来源：http://oi.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://up.9csxet.cn

[G05] 继承
来源：http://ml.szsharing.cn

Py:   class Admin(User): pass
来源：http://lx.521024.cn

PHP:  class Admin extends User {}
来源：http://kc.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://yz.newstarts.cn

TS:   class Admin extends User {}
来源：http://vz.colortex.cn

Java: class Admin extends User {}
来源：http://te.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dm.shxzskj.cn

Ruby: class Admin < User; end
来源：http://nv.shxzukj.cn

C#:   class Admin : User {}
来源：http://bv.muxihuayi.cn

[G06] 重写方法
来源：http://fo.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://ve.lnxyls.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hm.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ku.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://su.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://hd.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nx.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://sb.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://kq.9csxet.cn

[G07] 调用父类方法
来源：http://qm.yuexingan06.cn

Py:   super().greet()
来源：http://qz.lnxyls.cn

PHP:  parent::greet();
来源：http://da.muxihuayi.cn

JS:   super.greet();
来源：http://za.yuntaijiaju.cn

TS:   super.greet();
来源：http://gw.521024.cn

Java: super.greet();
来源：http://dk.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jj.gzmigu.cn

Ruby: super
来源：http://ds.shtwfgs.cn

C#:   base.Greet();
来源：http://px.szsharing.cn

[G08] 静态方法与属性
来源：http://zl.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bw.szxytkj.cn

PHP:  public static function f() {}
来源：http://qn.newstarts.cn

JS:   static f() {}
来源：http://zt.hahajie.cn

TS:   static f(): void {}
来源：http://nw.colortex.cn

Java: static void f() {}
来源：http://sq.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nf.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://zq.asd995.cn

C#:   public static void F() {}
来源：http://hg.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://cl.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://pc.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fv.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ck.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://ao.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://um.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://iw.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sm.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://gi.newstarts.cn

[G10] 访问控制
来源：http://fq.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://mk.hahajie.cn

PHP:  public / protected / private
来源：http://fw.newstarts.cn

JS:   #private 字段；其余公开
来源：http://eb.521024.cn

TS:   public / protected / private
来源：http://wa.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://cf.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zs.colortex.cn

Ruby: public / protected / private
来源：http://ap.lnxyls.cn

C#:   public / protected / private / internal
来源：http://sa.chemitech.net.cn

[G11] getter / setter
来源：http://jm.hahajie.cn

Py:   @property 与 @x.setter
来源：http://bw.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xt.521024.cn

JS:   get name() { return this._name; }
来源：http://ew.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://xv.nszjky.cn

Java: public String getName() { return name; }
来源：http://yf.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qc.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://fy.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://wi.asd995.cn

[G12] 对象转字符串
来源：http://yx.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://uz.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://td.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://wn.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://cq.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://qd.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://al.newstarts.cn

Ruby: def to_s; @name; end
来源：http://zk.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://iw.muxihuayi.cn

[G13] 判断对象类型
来源：http://yn.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://rr.asd995.cn

PHP:  $u instanceof User
来源：http://sr.lnxyls.cn

JS:   u instanceof User
来源：http://mf.jianghongdianzi.cn

TS:   u instanceof User
来源：http://vc.nszjky.cn

Java: u instanceof User
来源：http://lu.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wp.szsharing.cn

Ruby: u.is_a?(User)
来源：http://qr.lnxyls.cn

C#:   u is User
来源：http://ah.shxzskj.cn

[G14] 数据类 / record
来源：http://tm.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uo.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://sn.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gb.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://qs.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://gz.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://br.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vr.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://se.chemitech.net.cn

[G15] 枚举
来源：http://lj.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nz.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://he.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mv.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tg.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://ca.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yk.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://st.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://en.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://hf.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gr.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://vk.szsharing.cn

JS:   Object.entries(obj)
来源：http://du.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://cf.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lw.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vx.szsharing.cn

Ruby: obj.instance_variables
来源：http://am.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ml.colortex.cn

================================================================================
来源：http://ct.yuexingan06.cn

H. 异常与错误处理
来源：http://qz.szsharing.cn

================================================================================
来源：http://zq.panjiajie.cn

[H01] try / catch 基础
来源：http://qx.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://my.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vw.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qv.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mk.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yn.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ws.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ir.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zh.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://vd.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zf.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mg.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ro.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lt.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kf.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zn.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wz.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ot.shxzukj.cn

[H03] 主动抛出异常
来源：http://vp.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://hc.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ql.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://gl.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://uz.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ng.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aq.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pl.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hm.nicolike.cn

[H04] 自定义异常类型
来源：http://jo.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://lc.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://km.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://ev.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://rc.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://ui.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wr.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://pw.huanxung.cn

C#:   class MyException : Exception {}
来源：http://hk.gzmigu.cn

[H05] 捕获特定类型
来源：http://ic.newstarts.cn

Py:   except ValueError as e:
来源：http://ok.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gv.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://xx.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://mf.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://qk.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lg.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://pt.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pt.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://hr.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://bz.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dx.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tm.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xs.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oi.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kc.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://yj.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://wk.nicolike.cn

[H07] 断言
来源：http://ok.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://ev.9csxet.cn

PHP:  assert($x > 0);
来源：http://px.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://ma.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://kr.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://ca.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vu.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://um.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://ap.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://kl.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://mb.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yn.huanxung.cn

JS:   e.message;  e.stack
来源：http://ue.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jj.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jt.muxihuayi.cn

Go:   err.Error()
来源：http://dg.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://xn.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://mu.newstarts.cn

[H09] 带错误码的异常
来源：http://qx.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rq.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://la.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://st.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dt.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gq.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xp.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wp.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wb.bookmarksfly.cn

[H10] 资源自动释放
来源：http://in.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pd.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pk.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pw.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ih.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wf.shtwfgs.cn

Go:   defer f.Close()
来源：http://fk.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uq.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ep.chemitech.net.cn

================================================================================
来源：http://vh.521024.cn

I. 正则表达式
来源：http://xj.hahajie.cn

================================================================================
来源：http://pe.szxytkj.cn

[I01] 判断是否匹配
来源：http://wc.szsharing.cn


<!-- 参考信息 -->