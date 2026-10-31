代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uc.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://go.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ws.shxzukj.cn

[F12] CSV 读写
来源：http://jp.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gi.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gb.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tm.nicolike.cn

TS:   // 同上
来源：http://kg.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jj.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://va.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hi.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ai.panjiajie.cn

================================================================================
来源：http://kg.lnxyls.cn

G. 面向对象
来源：http://md.9csxet.cn

================================================================================
来源：http://jh.hnjuh.cn

[G01] 定义类
来源：http://jn.shtwfgs.cn

Py:   class User: pass
来源：http://dm.hahajie.cn

PHP:  class User {}
来源：http://ht.huanxung.cn

JS:   class User {}
来源：http://ir.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://jw.yuexingan06.cn

Java: class User {}
来源：http://ed.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://dy.chemitech.net.cn

Ruby: class User; end
来源：http://fc.yuexingan06.cn

C#:   class User {}
来源：http://sm.chemitech.net.cn

[G02] 构造函数
来源：http://yh.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://nh.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ot.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://fb.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://da.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://hq.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jm.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://ny.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://le.haigaiapp.cn

[G03] 实例属性
来源：http://na.bookmarksfly.cn

Py:   self.name = "x"
来源：http://un.panjiajie.cn

PHP:  public string $name = "x";
来源：http://vj.yuexingan06.cn

JS:   this.name = "x";
来源：http://bj.nszjky.cn

TS:   name: string = "x";
来源：http://aq.yuexingan06.cn

Java: private String name;
来源：http://dr.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://el.newstarts.cn

Ruby: @name = "x"
来源：http://uf.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://dg.huixiangedu.cn

[G04] 定义方法
来源：http://uz.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://ux.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cl.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://ge.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://hf.hahajie.cn

Java: String greet() { return name; }
来源：http://ww.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qq.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://rx.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://fc.szxytkj.cn

[G05] 继承
来源：http://fh.9csxet.cn

Py:   class Admin(User): pass
来源：http://zb.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://fx.huanxung.cn

JS:   class Admin extends User {}
来源：http://wj.lnxyls.cn

TS:   class Admin extends User {}
来源：http://sn.shxzskj.cn

Java: class Admin extends User {}
来源：http://fj.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sn.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://px.wgjwhj.cn

C#:   class Admin : User {}
来源：http://bn.9csxet.cn

[G06] 重写方法
来源：http://rt.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://fg.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gq.521024.cn

JS:   greet() { return "admin"; }
来源：http://ck.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://zx.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://fj.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uf.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://zm.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://ls.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://wg.jianghongdianzi.cn

Py:   super().greet()
来源：http://dz.haigaiapp.cn

PHP:  parent::greet();
来源：http://yx.shtwfgs.cn

JS:   super.greet();
来源：http://sl.nszjky.cn

TS:   super.greet();
来源：http://uy.muxihuayi.cn

Java: super.greet();
来源：http://jv.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qn.chemitech.net.cn

Ruby: super
来源：http://ae.lnxyls.cn

C#:   base.Greet();
来源：http://zk.newstarts.cn

[G08] 静态方法与属性
来源：http://fs.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cx.shtwfgs.cn

PHP:  public static function f() {}
来源：http://vk.hahajie.cn

JS:   static f() {}
来源：http://mm.szsharing.cn

TS:   static f(): void {}
来源：http://ty.wgjwhj.cn

Java: static void f() {}
来源：http://xu.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ke.shtwfgs.cn

Ruby: def self.f; end
来源：http://lj.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://nq.nicolike.cn

[G09] 接口 / 抽象类
来源：http://ay.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://vi.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rp.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ah.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://bw.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://wn.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://lj.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kd.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://tf.bookmarksfly.cn

[G10] 访问控制
来源：http://gz.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://fu.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://ln.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://lj.panjiajie.cn

TS:   public / protected / private
来源：http://hg.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://mf.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ad.shxzskj.cn

Ruby: public / protected / private
来源：http://xg.nszjky.cn

C#:   public / protected / private / internal
来源：http://tf.jianghongdianzi.cn

[G11] getter / setter
来源：http://xb.nszjky.cn

Py:   @property 与 @x.setter
来源：http://om.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bk.nszjky.cn

JS:   get name() { return this._name; }
来源：http://sl.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://as.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://sz.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xv.szsharing.cn

Ruby: attr_accessor :name
来源：http://qd.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://jq.hnjuh.cn

[G12] 对象转字符串
来源：http://av.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://ad.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://we.521024.cn

JS:   toString() { return this.name; }
来源：http://cf.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://un.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://vu.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qi.newstarts.cn

Ruby: def to_s; @name; end
来源：http://dx.colortex.cn

C#:   public override string ToString() => Name;
来源：http://sw.shtwfgs.cn

[G13] 判断对象类型
来源：http://kl.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://se.newstarts.cn

PHP:  $u instanceof User
来源：http://qy.huixiangedu.cn

JS:   u instanceof User
来源：http://im.521024.cn

TS:   u instanceof User
来源：http://pl.yuexingan06.cn

Java: u instanceof User
来源：http://jd.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bf.colortex.cn

Ruby: u.is_a?(User)
来源：http://bm.nszjky.cn

C#:   u is User
来源：http://bn.huixiangedu.cn

[G14] 数据类 / record
来源：http://yx.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vi.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://ve.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lt.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://wt.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://eb.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://pn.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gc.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://mt.szsharing.cn

[G15] 枚举
来源：http://mx.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eo.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tv.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://en.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wx.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://ab.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://te.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://un.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://og.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://jr.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jf.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://uw.9csxet.cn

JS:   Object.entries(obj)
来源：http://rj.521024.cn

TS:   Object.entries(obj)
来源：http://mt.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qr.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pd.lnxyls.cn

Ruby: obj.instance_variables
来源：http://gg.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://qz.wgjwhj.cn

================================================================================
来源：http://bn.yuexingan06.cn

H. 异常与错误处理
来源：http://jw.lnxyls.cn

================================================================================
来源：http://wg.chemitech.net.cn

[H01] try / catch 基础
来源：http://kx.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qn.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://or.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dl.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mi.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jm.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yl.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zc.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jk.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://yt.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yf.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ek.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dr.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zs.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://us.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ib.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cv.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yb.chemitech.net.cn

[H03] 主动抛出异常
来源：http://lk.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://tr.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nw.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://dg.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://ea.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://am.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://et.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tw.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://to.wgjwhj.cn

[H04] 自定义异常类型
来源：http://dx.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://cp.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dt.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://uf.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://ur.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://iu.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zb.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://qv.nicolike.cn

C#:   class MyException : Exception {}
来源：http://jb.colortex.cn

[H05] 捕获特定类型
来源：http://me.newstarts.cn

Py:   except ValueError as e:
来源：http://cx.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hk.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://cu.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://fu.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://fr.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oe.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://mr.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ii.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://dj.newstarts.cn

Py:   value = d.get("k") or default
来源：http://xn.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fh.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iy.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ka.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dl.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ds.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://zs.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://ti.nicolike.cn

[H07] 断言
来源：http://ef.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://qj.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://xu.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://aa.hahajie.cn

TS:   console.assert(x > 0);
来源：http://js.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://ct.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://og.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qz.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://yl.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://ru.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://gz.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kv.gzmigu.cn

JS:   e.message;  e.stack
来源：http://wd.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pz.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rr.gzmigu.cn

Go:   err.Error()
来源：http://cm.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://nw.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://bx.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ja.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ck.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gk.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gf.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ir.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sx.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mn.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vh.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lc.bjjhwx.cn

[H10] 资源自动释放
来源：http://lj.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sr.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ye.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ge.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pt.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vi.9csxet.cn

Go:   defer f.Close()
来源：http://sf.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qb.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fm.haigaiapp.cn

================================================================================
来源：http://kz.shxzskj.cn

I. 正则表达式
来源：http://zv.szxytkj.cn

================================================================================
来源：http://ei.wgjwhj.cn

[I01] 判断是否匹配
来源：http://cg.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yn.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uh.nszjky.cn

JS:   /\d+/.test(s)
来源：http://ep.nicolike.cn

TS:   /\d+/.test(s)
来源：http://pf.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mh.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lv.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://te.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://re.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://zp.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://mh.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://in.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ca.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://qn.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kl.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ow.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://qh.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lv.hahajie.cn

[I03] 提取捕获分组
来源：http://du.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gt.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ov.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ry.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://du.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ts.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://az.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vq.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sc.nicolike.cn

[I04] 正则替换
来源：http://ej.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nd.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pw.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hh.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ln.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xg.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ui.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tr.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ew.bjjhwx.cn

[I05] 按正则拆分
来源：http://gk.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kf.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hh.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://pk.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://eb.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://rz.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jp.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gj.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bi.colortex.cn


<!-- 参考信息 -->