代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://un.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zi.jctech888.com.cn

[F11] 复制与移动文件
来源：http://of.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iz.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tj.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wt.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://di.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vr.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ja.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eh.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rc.szxytkj.cn

[F12] CSV 读写
来源：http://iq.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kk.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hj.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pz.newstarts.cn

TS:   // 同上
来源：http://kp.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ev.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oh.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bs.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ko.shtwfgs.cn

================================================================================
来源：http://lp.shxzskj.cn

G. 面向对象
来源：http://np.shtwfgs.cn

================================================================================
来源：http://gi.nicolike.cn

[G01] 定义类
来源：http://es.bookmarksfly.cn

Py:   class User: pass
来源：http://vh.chemitech.net.cn

PHP:  class User {}
来源：http://sv.asd995.cn

JS:   class User {}
来源：http://ea.szsharing.cn

TS:   class User { name: string = ""; }
来源：http://ye.shtwfgs.cn

Java: class User {}
来源：http://yq.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://di.nszjky.cn

Ruby: class User; end
来源：http://gl.huixiangedu.cn

C#:   class User {}
来源：http://cj.chemitech.net.cn

[G02] 构造函数
来源：http://jx.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://pd.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://up.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://if.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://md.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://gx.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dj.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://ok.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://di.shxzukj.cn

[G03] 实例属性
来源：http://cv.nszjky.cn

Py:   self.name = "x"
来源：http://wn.colortex.cn

PHP:  public string $name = "x";
来源：http://ho.huixiangedu.cn

JS:   this.name = "x";
来源：http://ic.muxihuayi.cn

TS:   name: string = "x";
来源：http://jy.huixiangedu.cn

Java: private String name;
来源：http://tu.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ye.yuexingan06.cn

Ruby: @name = "x"
来源：http://sv.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://nc.shxzukj.cn

[G04] 定义方法
来源：http://lp.nszjky.cn

Py:   def greet(self): return self.name
来源：http://jr.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pf.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://sc.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://ik.9csxet.cn

Java: String greet() { return name; }
来源：http://wm.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yb.hnjuh.cn

Ruby: def greet; @name; end
来源：http://wl.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://of.jianghongdianzi.cn

[G05] 继承
来源：http://zy.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://lj.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://wn.asd995.cn

JS:   class Admin extends User {}
来源：http://pl.colortex.cn

TS:   class Admin extends User {}
来源：http://af.nicolike.cn

Java: class Admin extends User {}
来源：http://hj.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yo.szxytkj.cn

Ruby: class Admin < User; end
来源：http://mf.bjjhwx.cn

C#:   class Admin : User {}
来源：http://wg.newstarts.cn

[G06] 重写方法
来源：http://lm.asd995.cn

Py:   def greet(self): return "admin"
来源：http://an.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vv.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://bl.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://fj.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://rc.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dj.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://mh.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://mk.jctech888.com.cn

[G07] 调用父类方法
来源：http://iv.shtwfgs.cn

Py:   super().greet()
来源：http://mc.jctech888.com.cn

PHP:  parent::greet();
来源：http://kx.newstarts.cn

JS:   super.greet();
来源：http://ag.hahajie.cn

TS:   super.greet();
来源：http://tx.huixinmuqiang.cn

Java: super.greet();
来源：http://ll.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xp.haigaiapp.cn

Ruby: super
来源：http://js.szxytkj.cn

C#:   base.Greet();
来源：http://re.wgjwhj.cn

[G08] 静态方法与属性
来源：http://ar.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ep.nszjky.cn

PHP:  public static function f() {}
来源：http://ld.lnxyls.cn

JS:   static f() {}
来源：http://at.chemitech.net.cn

TS:   static f(): void {}
来源：http://ow.shxzskj.cn

Java: static void f() {}
来源：http://ux.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lm.shxzskj.cn

Ruby: def self.f; end
来源：http://qn.colortex.cn

C#:   public static void F() {}
来源：http://ym.nicolike.cn

[G09] 接口 / 抽象类
来源：http://kd.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://nw.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ma.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wa.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://ct.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://vc.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://sq.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fr.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://am.wgjwhj.cn

[G10] 访问控制
来源：http://gb.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://eg.9csxet.cn

PHP:  public / protected / private
来源：http://fq.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://ea.szxytkj.cn

TS:   public / protected / private
来源：http://ha.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://kw.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://me.lnxyls.cn

Ruby: public / protected / private
来源：http://ep.521024.cn

C#:   public / protected / private / internal
来源：http://su.huanxung.cn

[G11] getter / setter
来源：http://ss.9csxet.cn

Py:   @property 与 @x.setter
来源：http://xq.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://in.521024.cn

JS:   get name() { return this._name; }
来源：http://kf.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://wx.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ih.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cz.colortex.cn

Ruby: attr_accessor :name
来源：http://ud.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://sd.jctech888.com.cn

[G12] 对象转字符串
来源：http://uw.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://cr.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gi.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://bn.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://ym.521024.cn

Java: @Override public String toString() { return name; }
来源：http://zh.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qi.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://no.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://oo.newstarts.cn

[G13] 判断对象类型
来源：http://gp.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://bv.szxytkj.cn

PHP:  $u instanceof User
来源：http://jb.muxihuayi.cn

JS:   u instanceof User
来源：http://dd.yuntaijiaju.cn

TS:   u instanceof User
来源：http://lr.shxzukj.cn

Java: u instanceof User
来源：http://hd.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uc.9csxet.cn

Ruby: u.is_a?(User)
来源：http://cg.chemitech.net.cn

C#:   u is User
来源：http://ss.huixiangedu.cn

[G14] 数据类 / record
来源：http://tz.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cu.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://zm.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://li.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://yk.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://lp.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://qa.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wx.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://dh.muxihuayi.cn

[G15] 枚举
来源：http://gq.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ux.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ri.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yp.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gy.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://vp.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xv.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://nq.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://my.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://ns.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ci.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://zv.szsharing.cn

JS:   Object.entries(obj)
来源：http://tx.szxytkj.cn

TS:   Object.entries(obj)
来源：http://zl.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tr.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nx.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://hf.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://vk.yuexingan06.cn

================================================================================
来源：http://qn.huixiangedu.cn

H. 异常与错误处理
来源：http://zs.haigaiapp.cn

================================================================================
来源：http://oe.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://vp.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xf.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jy.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ks.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lf.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cs.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rd.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ah.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tw.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ph.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://su.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gk.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uo.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pt.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hr.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tp.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cp.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tz.lnxyls.cn

[H03] 主动抛出异常
来源：http://ue.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://qf.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dm.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://we.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://cs.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://np.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dc.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ip.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rv.wgjwhj.cn

[H04] 自定义异常类型
来源：http://hr.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://na.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qc.szsharing.cn

JS:   class MyError extends Error {}
来源：http://yn.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://cu.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://ld.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://si.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://ma.nicolike.cn

C#:   class MyException : Exception {}
来源：http://eu.nszjky.cn

[H05] 捕获特定类型
来源：http://id.haigaiapp.cn

Py:   except ValueError as e:
来源：http://tx.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ah.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://wa.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://fn.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://jf.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gf.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://al.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kv.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://et.asd995.cn

Py:   value = d.get("k") or default
来源：http://wl.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kl.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ni.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ix.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fi.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wb.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://bo.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://lw.521024.cn

[H07] 断言
来源：http://ka.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://cl.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://do.hahajie.cn

JS:   console.assert(x > 0);
来源：http://bb.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://rf.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://ic.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nw.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://it.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://lm.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://oq.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://gr.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://au.colortex.cn

JS:   e.message;  e.stack
来源：http://eu.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://co.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ik.gzmigu.cn

Go:   err.Error()
来源：http://mm.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://ns.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://eu.yuexingan06.cn

[H09] 带错误码的异常
来源：http://oi.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zw.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ll.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gy.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cu.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jc.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zj.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iq.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oy.szsharing.cn

[H10] 资源自动释放
来源：http://ih.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vs.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rf.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yj.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ac.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jm.panjiajie.cn

Go:   defer f.Close()
来源：http://iy.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ba.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qz.szsharing.cn

================================================================================
来源：http://bp.wgjwhj.cn

I. 正则表达式
来源：http://ed.muxihuayi.cn

================================================================================
来源：http://jx.newstarts.cn

[I01] 判断是否匹配
来源：http://uv.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tc.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xm.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://hg.szsharing.cn

TS:   /\d+/.test(s)
来源：http://nk.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jz.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xq.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://bt.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iw.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://dv.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://za.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://az.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ft.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://mq.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wv.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lo.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://yg.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ga.nicolike.cn

[I03] 提取捕获分组
来源：http://jm.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gz.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qh.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xf.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oa.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jm.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yh.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ih.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xs.panjiajie.cn

[I04] 正则替换
来源：http://if.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cd.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wp.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pl.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cn.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lw.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gj.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rc.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qf.nicolike.cn

[I05] 按正则拆分
来源：http://uq.panjiajie.cn


<!-- 参考信息 -->