代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zv.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uy.colortex.cn

[F11] 复制与移动文件
来源：http://zf.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vr.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ij.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qc.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mx.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ow.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fd.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xd.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oz.521024.cn

[F12] CSV 读写
来源：http://hx.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yn.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eb.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mb.haigaiapp.cn

TS:   // 同上
来源：http://fp.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qi.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uk.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cq.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ps.gzmigu.cn

================================================================================
来源：http://jh.shxzskj.cn

G. 面向对象
来源：http://rd.hahajie.cn

================================================================================
来源：http://zz.shtwfgs.cn

[G01] 定义类
来源：http://fh.huixinmuqiang.cn

Py:   class User: pass
来源：http://sa.9csxet.cn

PHP:  class User {}
来源：http://vy.shxzukj.cn

JS:   class User {}
来源：http://wm.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ng.yuntaijiaju.cn

Java: class User {}
来源：http://lp.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://xy.lnxyls.cn

Ruby: class User; end
来源：http://fz.newstarts.cn

C#:   class User {}
来源：http://pk.nicolike.cn

[G02] 构造函数
来源：http://zc.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://pu.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://ob.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://og.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://yl.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://gg.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nc.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://fw.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://mi.panjiajie.cn

[G03] 实例属性
来源：http://lq.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://if.newstarts.cn

PHP:  public string $name = "x";
来源：http://ev.shxzukj.cn

JS:   this.name = "x";
来源：http://di.521024.cn

TS:   name: string = "x";
来源：http://tc.wgjwhj.cn

Java: private String name;
来源：http://ru.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xd.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://ox.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://ii.huixinmuqiang.cn

[G04] 定义方法
来源：http://do.521024.cn

Py:   def greet(self): return self.name
来源：http://ef.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fg.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://xc.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://rz.nszjky.cn

Java: String greet() { return name; }
来源：http://kj.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bd.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://zy.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://wt.colortex.cn

[G05] 继承
来源：http://jj.szxytkj.cn

Py:   class Admin(User): pass
来源：http://dr.9csxet.cn

PHP:  class Admin extends User {}
来源：http://hd.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://yj.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://cw.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ov.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://db.asd995.cn

Ruby: class Admin < User; end
来源：http://yh.shxzukj.cn

C#:   class Admin : User {}
来源：http://de.huixinmuqiang.cn

[G06] 重写方法
来源：http://mh.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://mj.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oi.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://oc.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://jt.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ai.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gr.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://bw.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://dl.colortex.cn

[G07] 调用父类方法
来源：http://xf.lnxyls.cn

Py:   super().greet()
来源：http://gj.nszjky.cn

PHP:  parent::greet();
来源：http://ti.shxzskj.cn

JS:   super.greet();
来源：http://yf.nicolike.cn

TS:   super.greet();
来源：http://du.colortex.cn

Java: super.greet();
来源：http://ni.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ag.yuexingan06.cn

Ruby: super
来源：http://yj.gzmigu.cn

C#:   base.Greet();
来源：http://jz.wgjwhj.cn

[G08] 静态方法与属性
来源：http://xu.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kd.shxzukj.cn

PHP:  public static function f() {}
来源：http://dn.gzmigu.cn

JS:   static f() {}
来源：http://ep.lnxyls.cn

TS:   static f(): void {}
来源：http://cp.shxzukj.cn

Java: static void f() {}
来源：http://dp.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ji.hnjuh.cn

Ruby: def self.f; end
来源：http://dz.jctech888.com.cn

C#:   public static void F() {}
来源：http://xy.asd995.cn

[G09] 接口 / 抽象类
来源：http://kk.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://in.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tu.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jq.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://bw.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://gh.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://vd.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ru.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://zb.colortex.cn

[G10] 访问控制
来源：http://ir.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://vv.hahajie.cn

PHP:  public / protected / private
来源：http://kp.colortex.cn

JS:   #private 字段；其余公开
来源：http://mw.gzmigu.cn

TS:   public / protected / private
来源：http://we.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://zq.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tl.haigaiapp.cn

Ruby: public / protected / private
来源：http://uu.gzmigu.cn

C#:   public / protected / private / internal
来源：http://fi.yuexingan06.cn

[G11] getter / setter
来源：http://ou.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://cp.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ew.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://iv.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://dc.hnjuh.cn

Java: public String getName() { return name; }
来源：http://jv.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kc.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://xp.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://qk.shxzukj.cn

[G12] 对象转字符串
来源：http://bn.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://fi.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ow.nszjky.cn

JS:   toString() { return this.name; }
来源：http://gm.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://vl.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://lk.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gs.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://pw.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://wf.huanxung.cn

[G13] 判断对象类型
来源：http://eg.shxzskj.cn

Py:   isinstance(u, User)
来源：http://ui.shtwfgs.cn

PHP:  $u instanceof User
来源：http://pp.huixiangedu.cn

JS:   u instanceof User
来源：http://dj.panjiajie.cn

TS:   u instanceof User
来源：http://tp.9csxet.cn

Java: u instanceof User
来源：http://ey.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://na.nicolike.cn

Ruby: u.is_a?(User)
来源：http://oq.hahajie.cn

C#:   u is User
来源：http://ne.9csxet.cn

[G14] 数据类 / record
来源：http://ad.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lw.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://am.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://op.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://sf.nszjky.cn

Java: record User(String name, int age) {}
来源：http://em.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://aj.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://do.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://kb.asd995.cn

[G15] 枚举
来源：http://wt.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bd.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wq.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://un.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lu.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://tw.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tr.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://di.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tq.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://ny.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ou.521024.cn

PHP:  get_object_vars($obj);
来源：http://ft.521024.cn

JS:   Object.entries(obj)
来源：http://vm.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://gs.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pm.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fe.521024.cn

Ruby: obj.instance_variables
来源：http://jn.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://sg.yuexingan06.cn

================================================================================
来源：http://zn.9csxet.cn

H. 异常与错误处理
来源：http://ka.szsharing.cn

================================================================================
来源：http://pz.asd995.cn

[H01] try / catch 基础
来源：http://qs.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pb.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ow.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ug.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tq.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pd.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nh.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ud.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ai.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://nk.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ok.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ze.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wb.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yd.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ko.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qn.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hg.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bf.asd995.cn

[H03] 主动抛出异常
来源：http://ck.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://kk.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bq.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://gz.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://kw.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ml.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iq.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vm.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gi.shxzskj.cn

[H04] 自定义异常类型
来源：http://ly.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://ky.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dk.szsharing.cn

JS:   class MyError extends Error {}
来源：http://fz.9csxet.cn

TS:   class MyError extends Error {}
来源：http://re.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://fh.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dv.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://fy.huanxung.cn

C#:   class MyException : Exception {}
来源：http://ru.chemitech.net.cn

[H05] 捕获特定类型
来源：http://zy.bjjhwx.cn

Py:   except ValueError as e:
来源：http://km.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jm.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://fi.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ap.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://va.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mv.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://mu.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dw.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://no.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://xt.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sz.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zl.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qh.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ec.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://in.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://kr.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://nt.shxzukj.cn

[H07] 断言
来源：http://mb.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://pm.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://zh.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://gx.hahajie.cn

TS:   console.assert(x > 0);
来源：http://vl.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://su.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xg.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wy.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://nw.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://pc.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://hg.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bp.shxzukj.cn

JS:   e.message;  e.stack
来源：http://pj.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vf.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ua.nicolike.cn

Go:   err.Error()
来源：http://xd.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://fn.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://th.szsharing.cn

[H09] 带错误码的异常
来源：http://rh.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zu.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bt.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bw.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bq.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://np.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gl.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xj.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hh.huanxung.cn

[H10] 资源自动释放
来源：http://yk.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xw.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zx.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ij.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bv.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cg.wgjwhj.cn

Go:   defer f.Close()
来源：http://nn.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gw.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ef.panjiajie.cn

================================================================================
来源：http://mg.szsharing.cn

I. 正则表达式
来源：http://xf.colortex.cn

================================================================================
来源：http://sm.szxytkj.cn

[I01] 判断是否匹配
来源：http://xd.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dc.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xq.colortex.cn

JS:   /\d+/.test(s)
来源：http://ok.nicolike.cn

TS:   /\d+/.test(s)
来源：http://jp.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://by.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eb.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://rd.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nm.muxihuayi.cn

[I02] 提取所有匹配
来源：http://hk.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://qr.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://al.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pa.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://pn.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://is.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yt.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://on.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iq.nicolike.cn

[I03] 提取捕获分组
来源：http://au.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ji.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xd.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bs.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kt.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dd.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://is.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mf.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://an.muxihuayi.cn

[I04] 正则替换
来源：http://mh.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xz.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://za.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ne.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ya.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fb.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://je.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ex.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ab.panjiajie.cn

[I05] 按正则拆分
来源：http://xq.huixiangedu.cn


<!-- 参考信息 -->