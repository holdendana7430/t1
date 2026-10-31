代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xq.hahajie.cn

TS:   path.extname("a.txt")
来源：http://ap.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sn.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wj.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vm.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bi.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://xd.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fg.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pb.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yb.521024.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pr.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://az.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ui.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lk.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rg.bookmarksfly.cn

[F12] CSV 读写
来源：http://bd.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://px.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dd.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lk.colortex.cn

TS:   // 同上
来源：http://bx.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cd.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ys.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bw.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fv.shxzskj.cn

================================================================================
来源：http://lh.newstarts.cn

G. 面向对象
来源：http://jp.shxzukj.cn

================================================================================
来源：http://op.szxytkj.cn

[G01] 定义类
来源：http://nd.yuexingan06.cn

Py:   class User: pass
来源：http://lc.shxzukj.cn

PHP:  class User {}
来源：http://yy.9csxet.cn

JS:   class User {}
来源：http://ty.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://ye.bookmarksfly.cn

Java: class User {}
来源：http://bz.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://gi.huixiangedu.cn

Ruby: class User; end
来源：http://aj.szxytkj.cn

C#:   class User {}
来源：http://bh.9csxet.cn

[G02] 构造函数
来源：http://ax.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://vf.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://hc.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://zx.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://ao.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://mm.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lx.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://lu.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://sg.yuntaijiaju.cn

[G03] 实例属性
来源：http://lc.lnxyls.cn

Py:   self.name = "x"
来源：http://ev.huanxung.cn

PHP:  public string $name = "x";
来源：http://lt.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://vw.hahajie.cn

TS:   name: string = "x";
来源：http://ns.szsharing.cn

Java: private String name;
来源：http://at.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gv.shxzskj.cn

Ruby: @name = "x"
来源：http://ro.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://sx.jianghongdianzi.cn

[G04] 定义方法
来源：http://fk.asd995.cn

Py:   def greet(self): return self.name
来源：http://fc.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jx.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://rc.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://tp.chemitech.net.cn

Java: String greet() { return name; }
来源：http://xl.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wu.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://fx.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://if.szsharing.cn

[G05] 继承
来源：http://lq.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://vj.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://br.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://id.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://go.shtwfgs.cn

Java: class Admin extends User {}
来源：http://bu.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://et.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://sx.newstarts.cn

C#:   class Admin : User {}
来源：http://ge.jianghongdianzi.cn

[G06] 重写方法
来源：http://ty.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://dv.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yv.521024.cn

JS:   greet() { return "admin"; }
来源：http://za.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://hn.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ym.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hr.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://sr.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://zh.huixiangedu.cn

[G07] 调用父类方法
来源：http://mg.9csxet.cn

Py:   super().greet()
来源：http://ew.gzmigu.cn

PHP:  parent::greet();
来源：http://go.gzmigu.cn

JS:   super.greet();
来源：http://zx.bookmarksfly.cn

TS:   super.greet();
来源：http://qt.hahajie.cn

Java: super.greet();
来源：http://jg.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zo.szxytkj.cn

Ruby: super
来源：http://cc.wgjwhj.cn

C#:   base.Greet();
来源：http://mc.colortex.cn

[G08] 静态方法与属性
来源：http://bs.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jn.wgjwhj.cn

PHP:  public static function f() {}
来源：http://dk.yuexingan06.cn

JS:   static f() {}
来源：http://uz.nicolike.cn

TS:   static f(): void {}
来源：http://pw.hahajie.cn

Java: static void f() {}
来源：http://hf.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gl.jctech888.com.cn

Ruby: def self.f; end
来源：http://yp.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://nn.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://he.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://kq.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tu.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ay.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://sy.9csxet.cn

Java: interface Shape { double area(); }
来源：http://cq.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ac.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sk.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://ey.colortex.cn

[G10] 访问控制
来源：http://ew.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://vn.haigaiapp.cn

PHP:  public / protected / private
来源：http://pe.huanxung.cn

JS:   #private 字段；其余公开
来源：http://wn.shxzskj.cn

TS:   public / protected / private
来源：http://jx.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://tm.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnjuh.cn

Ruby: public / protected / private
来源：http://ge.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://eo.shxzskj.cn

[G11] getter / setter
来源：http://pa.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://jx.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bx.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://bc.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://wh.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://kl.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vl.huanxung.cn

Ruby: attr_accessor :name
来源：http://br.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://lu.chemitech.net.cn

[G12] 对象转字符串
来源：http://ou.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://sc.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xs.newstarts.cn

JS:   toString() { return this.name; }
来源：http://wc.521024.cn

TS:   toString(): string { return this.name; }
来源：http://er.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://jj.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mx.huanxung.cn

Ruby: def to_s; @name; end
来源：http://fb.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://qb.haigaiapp.cn

[G13] 判断对象类型
来源：http://ei.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://aq.hnjuh.cn

PHP:  $u instanceof User
来源：http://vq.gzmigu.cn

JS:   u instanceof User
来源：http://uf.yuexingan06.cn

TS:   u instanceof User
来源：http://ui.chemitech.net.cn

Java: u instanceof User
来源：http://pe.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://de.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://ye.9csxet.cn

C#:   u is User
来源：http://wk.nszjky.cn

[G14] 数据类 / record
来源：http://dx.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://te.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://qe.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gm.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://mj.hahajie.cn

Java: record User(String name, int age) {}
来源：http://lt.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://qo.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pz.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://cp.shxzukj.cn

[G15] 枚举
来源：http://hb.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rv.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ik.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qg.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ov.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://pb.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vm.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://gc.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gs.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://ui.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ta.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://lj.asd995.cn

JS:   Object.entries(obj)
来源：http://zp.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://lf.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://so.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hg.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://zr.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://im.panjiajie.cn

================================================================================
来源：http://hq.szsharing.cn

H. 异常与错误处理
来源：http://jh.9csxet.cn

================================================================================
来源：http://kz.colortex.cn

[H01] try / catch 基础
来源：http://jk.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://si.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ws.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mv.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ku.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ud.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tt.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xf.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fq.asd995.cn

[H02] finally / ensure 收尾
来源：http://uc.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vy.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kr.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://va.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://db.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rv.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rl.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ry.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ft.hahajie.cn

[H03] 主动抛出异常
来源：http://ij.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://da.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cx.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://ks.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://xq.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zq.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pc.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oe.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://df.newstarts.cn

[H04] 自定义异常类型
来源：http://dd.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://cz.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ji.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://rd.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://pm.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://ft.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uc.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://yb.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://ab.wgjwhj.cn

[H05] 捕获特定类型
来源：http://ml.hahajie.cn

Py:   except ValueError as e:
来源：http://pa.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://er.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ga.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://in.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://hn.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dw.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://mw.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ip.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://zy.9csxet.cn

Py:   value = d.get("k") or default
来源：http://xa.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jc.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nb.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sp.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jd.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dr.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://sp.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://ds.hnjuh.cn

[H07] 断言
来源：http://eq.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://uc.szsharing.cn

PHP:  assert($x > 0);
来源：http://ky.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://cn.nicolike.cn

TS:   console.assert(x > 0);
来源：http://kj.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://jp.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ij.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yy.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ys.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://zs.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://ir.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sd.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://jy.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yp.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kb.shxzskj.cn

Go:   err.Error()
来源：http://mm.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://bc.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://ex.nszjky.cn

[H09] 带错误码的异常
来源：http://uo.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ms.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ye.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lo.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://be.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pl.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ym.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gw.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ei.huixiangedu.cn

[H10] 资源自动释放
来源：http://fh.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://su.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ho.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kf.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ti.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iz.muxihuayi.cn

Go:   defer f.Close()
来源：http://zs.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cn.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ug.haigaiapp.cn

================================================================================
来源：http://kq.yuntaijiaju.cn

I. 正则表达式
来源：http://hx.nicolike.cn

================================================================================
来源：http://uw.huanxung.cn

[I01] 判断是否匹配
来源：http://ds.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ru.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ma.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://uk.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://pf.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://li.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jb.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://mx.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jf.nicolike.cn

[I02] 提取所有匹配
来源：http://dr.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://rw.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xb.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mp.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://ta.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tu.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wo.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://lv.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://py.hahajie.cn

[I03] 提取捕获分组
来源：http://od.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aj.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tw.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rv.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sf.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cr.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ok.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fv.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kx.lnxyls.cn

[I04] 正则替换
来源：http://bq.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qk.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lj.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rb.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oy.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ge.nicolike.cn


<!-- 参考信息 -->