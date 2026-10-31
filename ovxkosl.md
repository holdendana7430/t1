代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wy.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lv.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gc.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ab.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ip.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ta.yuntaijiaju.cn

[F12] CSV 读写
来源：http://su.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hr.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://om.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bw.hnjuh.cn

TS:   // 同上
来源：http://it.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eq.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sv.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mp.yuexingan06.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nt.yuexingan06.cn

================================================================================
来源：http://ik.bookmarksfly.cn

G. 面向对象
来源：http://cl.jianghongdianzi.cn

================================================================================
来源：http://yb.jianghongdianzi.cn

[G01] 定义类
来源：http://ts.haigaiapp.cn

Py:   class User: pass
来源：http://nl.szsharing.cn

PHP:  class User {}
来源：http://lr.colortex.cn

JS:   class User {}
来源：http://ji.colortex.cn

TS:   class User { name: string = ""; }
来源：http://zm.shxzskj.cn

Java: class User {}
来源：http://wr.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://wo.shtwfgs.cn

Ruby: class User; end
来源：http://ic.bjjhwx.cn

C#:   class User {}
来源：http://ub.9csxet.cn

[G02] 构造函数
来源：http://cf.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://oh.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://qx.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://zh.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://cn.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://eb.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bz.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://yv.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://hb.gzmigu.cn

[G03] 实例属性
来源：http://gz.asd995.cn

Py:   self.name = "x"
来源：http://xk.newstarts.cn

PHP:  public string $name = "x";
来源：http://ke.colortex.cn

JS:   this.name = "x";
来源：http://zu.gzmigu.cn

TS:   name: string = "x";
来源：http://yg.jctech888.com.cn

Java: private String name;
来源：http://dw.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hf.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://wu.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://jp.shxzskj.cn

[G04] 定义方法
来源：http://cc.colortex.cn

Py:   def greet(self): return self.name
来源：http://nh.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ax.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://vy.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://za.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://xp.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ap.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://qh.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://zy.nszjky.cn

[G05] 继承
来源：http://oo.hahajie.cn

Py:   class Admin(User): pass
来源：http://tb.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://jy.szxytkj.cn

JS:   class Admin extends User {}
来源：http://jk.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ui.huixiangedu.cn

Java: class Admin extends User {}
来源：http://hv.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nm.hnjuh.cn

Ruby: class Admin < User; end
来源：http://kq.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://mq.yuntaijiaju.cn

[G06] 重写方法
来源：http://vw.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://xr.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ya.colortex.cn

JS:   greet() { return "admin"; }
来源：http://kr.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://do.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://dj.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://on.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://qh.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://ql.colortex.cn

[G07] 调用父类方法
来源：http://lj.chemitech.net.cn

Py:   super().greet()
来源：http://jp.muxihuayi.cn

PHP:  parent::greet();
来源：http://cr.shxzukj.cn

JS:   super.greet();
来源：http://id.hnjuh.cn

TS:   super.greet();
来源：http://jq.nicolike.cn

Java: super.greet();
来源：http://ld.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jx.jianghongdianzi.cn

Ruby: super
来源：http://eq.asd995.cn

C#:   base.Greet();
来源：http://st.shxzskj.cn

[G08] 静态方法与属性
来源：http://ts.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://go.nicolike.cn

PHP:  public static function f() {}
来源：http://cv.haigaiapp.cn

JS:   static f() {}
来源：http://wr.haigaiapp.cn

TS:   static f(): void {}
来源：http://cw.asd995.cn

Java: static void f() {}
来源：http://aa.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wm.hahajie.cn

Ruby: def self.f; end
来源：http://gg.muxihuayi.cn

C#:   public static void F() {}
来源：http://ho.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://tz.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://el.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rg.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nz.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://nk.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://ew.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://qj.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uq.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://jx.hnjuh.cn

[G10] 访问控制
来源：http://be.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://sa.jctech888.com.cn

PHP:  public / protected / private
来源：http://ls.nicolike.cn

JS:   #private 字段；其余公开
来源：http://lq.huanxung.cn

TS:   public / protected / private
来源：http://zb.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://wu.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xg.szsharing.cn

Ruby: public / protected / private
来源：http://se.shxzskj.cn

C#:   public / protected / private / internal
来源：http://wg.shxzukj.cn

[G11] getter / setter
来源：http://vq.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://ul.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uo.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://gh.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://kv.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://vv.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ys.szsharing.cn

Ruby: attr_accessor :name
来源：http://us.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://hz.shtwfgs.cn

[G12] 对象转字符串
来源：http://fx.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://ve.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pk.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://sa.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://vr.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://xz.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gk.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://he.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://zy.shxzukj.cn

[G13] 判断对象类型
来源：http://ov.szxytkj.cn

Py:   isinstance(u, User)
来源：http://ct.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ld.huanxung.cn

JS:   u instanceof User
来源：http://zs.wgjwhj.cn

TS:   u instanceof User
来源：http://em.hnjuh.cn

Java: u instanceof User
来源：http://gq.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nv.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://qz.panjiajie.cn

C#:   u is User
来源：http://dy.521024.cn

[G14] 数据类 / record
来源：http://el.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ep.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://dk.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cc.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://xd.9csxet.cn

Java: record User(String name, int age) {}
来源：http://vs.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://vn.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://un.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://yt.yuntaijiaju.cn

[G15] 枚举
来源：http://qp.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ha.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uq.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gp.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hu.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://ea.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uc.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://gx.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sw.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://qv.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zn.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://dn.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://fa.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ed.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://me.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uz.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://kg.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://af.huixiangedu.cn

================================================================================
来源：http://ww.bjjhwx.cn

H. 异常与错误处理
来源：http://kj.yuexingan06.cn

================================================================================
来源：http://zj.jctech888.com.cn

[H01] try / catch 基础
来源：http://hj.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ww.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://px.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wx.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tm.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gg.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zp.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kd.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uy.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://ux.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ay.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://un.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hf.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tx.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://na.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kz.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sp.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ex.shxzukj.cn

[H03] 主动抛出异常
来源：http://kn.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://jx.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://au.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://fb.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://zl.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ee.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qr.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qp.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xy.szsharing.cn

[H04] 自定义异常类型
来源：http://an.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://nh.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mc.asd995.cn

JS:   class MyError extends Error {}
来源：http://ab.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://su.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://fl.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hb.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://hx.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://qg.panjiajie.cn

[H05] 捕获特定类型
来源：http://ab.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://rk.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ja.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://xe.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://mn.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://de.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rj.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://vb.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://go.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://gs.huanxung.cn

Py:   value = d.get("k") or default
来源：http://dj.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kf.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ac.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pj.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vc.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hk.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://uy.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://pn.hahajie.cn

[H07] 断言
来源：http://er.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://hp.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://uu.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://qz.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://cl.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://bm.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yo.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ud.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://jc.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://pl.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://un.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fd.521024.cn

JS:   e.message;  e.stack
来源：http://bn.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jb.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xs.shtwfgs.cn

Go:   err.Error()
来源：http://yb.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://nr.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://bs.gzmigu.cn

[H09] 带错误码的异常
来源：http://vc.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ep.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://or.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qc.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fp.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uy.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jc.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ws.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://az.asd995.cn

[H10] 资源自动释放
来源：http://xk.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gk.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dt.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ie.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qy.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nr.jctech888.com.cn

Go:   defer f.Close()
来源：http://or.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sa.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yc.hahajie.cn

================================================================================
来源：http://ia.lnxyls.cn

I. 正则表达式
来源：http://pa.hnjuh.cn

================================================================================
来源：http://vf.shxzukj.cn

[I01] 判断是否匹配
来源：http://so.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zu.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fe.huanxung.cn

JS:   /\d+/.test(s)
来源：http://fe.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://es.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nk.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aw.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://uz.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://as.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://yq.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://cs.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rn.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vq.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://ue.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lm.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fn.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://ha.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zr.wgjwhj.cn

[I03] 提取捕获分组
来源：http://ap.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jb.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fv.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mz.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pz.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://av.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ri.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uj.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hj.chemitech.net.cn

[I04] 正则替换
来源：http://ml.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zg.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qe.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vo.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oc.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uj.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jx.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ho.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://he.wgjwhj.cn

[I05] 按正则拆分
来源：http://xk.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qv.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ha.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://tq.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://jw.jctech888.com.cn


<!-- 参考信息 -->