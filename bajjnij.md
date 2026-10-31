代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://of.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://es.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cd.chemitech.net.cn

TS:   // 同上
来源：http://qt.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bo.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qj.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ie.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tw.jianghongdianzi.cn

================================================================================
来源：http://fa.chemitech.net.cn

G. 面向对象
来源：http://mv.bookmarksfly.cn

================================================================================
来源：http://pb.haigaiapp.cn

[G01] 定义类
来源：http://xv.asd995.cn

Py:   class User: pass
来源：http://uz.yuexingan06.cn

PHP:  class User {}
来源：http://wm.nszjky.cn

JS:   class User {}
来源：http://tr.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://lo.lnxyls.cn

Java: class User {}
来源：http://ze.panjiajie.cn

Go:   type User struct { Name string }
来源：http://vn.shtwfgs.cn

Ruby: class User; end
来源：http://wr.szsharing.cn

C#:   class User {}
来源：http://mx.newstarts.cn

[G02] 构造函数
来源：http://ob.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://tx.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://vv.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://tn.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://jt.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://xt.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kk.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://sn.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://mi.shxzskj.cn

[G03] 实例属性
来源：http://wg.huixiangedu.cn

Py:   self.name = "x"
来源：http://zf.newstarts.cn

PHP:  public string $name = "x";
来源：http://ma.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://rm.bjjhwx.cn

TS:   name: string = "x";
来源：http://js.nszjky.cn

Java: private String name;
来源：http://ce.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://od.newstarts.cn

Ruby: @name = "x"
来源：http://uc.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://wy.hnjuh.cn

[G04] 定义方法
来源：http://wq.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://jg.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pu.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://ry.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://fp.newstarts.cn

Java: String greet() { return name; }
来源：http://wy.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ev.huanxung.cn

Ruby: def greet; @name; end
来源：http://tv.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://xl.huixinmuqiang.cn

[G05] 继承
来源：http://tm.nszjky.cn

Py:   class Admin(User): pass
来源：http://qe.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://ml.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://qi.shxzskj.cn

TS:   class Admin extends User {}
来源：http://nw.nicolike.cn

Java: class Admin extends User {}
来源：http://qa.panjiajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ci.szxytkj.cn

Ruby: class Admin < User; end
来源：http://sd.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://ou.chemitech.net.cn

[G06] 重写方法
来源：http://hl.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://va.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ne.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://qw.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://hu.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://mb.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yo.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://bf.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://ei.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://pr.yuntaijiaju.cn

Py:   super().greet()
来源：http://rg.jctech888.com.cn

PHP:  parent::greet();
来源：http://od.nicolike.cn

JS:   super.greet();
来源：http://lz.asd995.cn

TS:   super.greet();
来源：http://tk.521024.cn

Java: super.greet();
来源：http://hn.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qo.huixiangedu.cn

Ruby: super
来源：http://sn.521024.cn

C#:   base.Greet();
来源：http://ju.szxytkj.cn

[G08] 静态方法与属性
来源：http://zx.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://js.bjjhwx.cn

PHP:  public static function f() {}
来源：http://mf.gzmigu.cn

JS:   static f() {}
来源：http://tx.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://ch.bjjhwx.cn

Java: static void f() {}
来源：http://ls.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ui.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://cw.asd995.cn

C#:   public static void F() {}
来源：http://ae.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://tf.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://pl.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uf.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tp.521024.cn

TS:   interface Shape { area(): number; }
来源：http://xz.9csxet.cn

Java: interface Shape { double area(); }
来源：http://mo.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://bs.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ye.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://ca.9csxet.cn

[G10] 访问控制
来源：http://kb.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://dy.bjjhwx.cn

PHP:  public / protected / private
来源：http://rm.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://bm.9csxet.cn

TS:   public / protected / private
来源：http://hw.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://az.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cv.bookmarksfly.cn

Ruby: public / protected / private
来源：http://ke.hahajie.cn

C#:   public / protected / private / internal
来源：http://ca.nicolike.cn

[G11] getter / setter
来源：http://aa.nszjky.cn

Py:   @property 与 @x.setter
来源：http://zg.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zg.hahajie.cn

JS:   get name() { return this._name; }
来源：http://az.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://sr.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://cq.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kl.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://vp.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://ps.szxytkj.cn

[G12] 对象转字符串
来源：http://kj.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://tw.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bj.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://wh.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://ez.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://gv.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rp.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://af.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://df.shtwfgs.cn

[G13] 判断对象类型
来源：http://sy.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://ek.huanxung.cn

PHP:  $u instanceof User
来源：http://rs.lnxyls.cn

JS:   u instanceof User
来源：http://he.shtwfgs.cn

TS:   u instanceof User
来源：http://ch.yuexingan06.cn

Java: u instanceof User
来源：http://so.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mx.colortex.cn

Ruby: u.is_a?(User)
来源：http://wx.hnjuh.cn

C#:   u is User
来源：http://nz.521024.cn

[G14] 数据类 / record
来源：http://ce.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kj.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://ba.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vc.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://hi.szsharing.cn

Java: record User(String name, int age) {}
来源：http://lx.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://nk.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://am.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://zp.gzmigu.cn

[G15] 枚举
来源：http://za.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fd.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://au.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kl.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zo.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://ig.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pr.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://hh.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kp.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://wh.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bb.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://vm.gzmigu.cn

JS:   Object.entries(obj)
来源：http://bn.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://vx.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gr.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tb.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://kd.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://hy.hnjuh.cn

================================================================================
来源：http://ov.jianghongdianzi.cn

H. 异常与错误处理
来源：http://no.shxzskj.cn

================================================================================
来源：http://gp.bookmarksfly.cn

[H01] try / catch 基础
来源：http://iy.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nz.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qd.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pi.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oz.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xd.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kp.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cu.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bu.nszjky.cn

[H02] finally / ensure 收尾
来源：http://hy.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ex.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://np.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://st.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ka.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ut.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cl.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://no.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rf.chemitech.net.cn

[H03] 主动抛出异常
来源：http://wx.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://iw.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mk.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://ir.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://gl.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://og.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hc.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zs.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ox.9csxet.cn

[H04] 自定义异常类型
来源：http://gz.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://um.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kb.hahajie.cn

JS:   class MyError extends Error {}
来源：http://dq.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://ac.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://my.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ed.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://yz.nszjky.cn

C#:   class MyException : Exception {}
来源：http://sz.huixiangedu.cn

[H05] 捕获特定类型
来源：http://rl.hahajie.cn

Py:   except ValueError as e:
来源：http://dx.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bs.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://ss.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://we.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://re.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ar.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://th.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cq.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://ft.nicolike.cn

Py:   value = d.get("k") or default
来源：http://sk.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wy.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jf.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tq.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tm.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mq.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://kx.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://hg.colortex.cn

[H07] 断言
来源：http://wd.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://yj.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://xp.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://kt.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://cw.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://al.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ib.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gy.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://jz.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://xp.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://hq.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cs.panjiajie.cn

JS:   e.message;  e.stack
来源：http://me.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nd.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nu.wgjwhj.cn

Go:   err.Error()
来源：http://xx.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://se.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://fg.szxytkj.cn

[H09] 带错误码的异常
来源：http://ws.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vm.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kl.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ky.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nt.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://na.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tz.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ju.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pj.newstarts.cn

[H10] 资源自动释放
来源：http://yp.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ib.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dx.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://po.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sl.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ep.9csxet.cn

Go:   defer f.Close()
来源：http://nt.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gs.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hw.newstarts.cn

================================================================================
来源：http://hk.huixiangedu.cn

I. 正则表达式
来源：http://wa.newstarts.cn

================================================================================
来源：http://fe.nszjky.cn

[I01] 判断是否匹配
来源：http://cy.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aa.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cq.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://et.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://mo.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gj.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vt.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://ud.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gg.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://ka.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://ua.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rp.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tn.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://ba.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fh.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lg.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://qf.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qx.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://fi.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tl.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bd.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pw.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ye.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cm.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mq.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://no.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lp.szxytkj.cn

[I04] 正则替换
来源：http://tz.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hm.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lm.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qj.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kz.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xi.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xq.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://df.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qp.521024.cn

[I05] 按正则拆分
来源：http://dg.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yr.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fx.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://zr.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://uf.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://it.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ag.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ky.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fr.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gh.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hu.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qm.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rq.shxzukj.cn


<!-- 参考信息 -->