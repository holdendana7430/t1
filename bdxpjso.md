代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mj.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://up.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qa.shtwfgs.cn

[F12] CSV 读写
来源：http://xm.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bq.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bx.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ut.muxihuayi.cn

TS:   // 同上
来源：http://gf.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hk.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cq.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ae.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ug.haigaiapp.cn

================================================================================
来源：http://nf.yuexingan06.cn

G. 面向对象
来源：http://ik.huixiangedu.cn

================================================================================
来源：http://lk.hahajie.cn

[G01] 定义类
来源：http://ro.9csxet.cn

Py:   class User: pass
来源：http://ab.hahajie.cn

PHP:  class User {}
来源：http://wq.szxytkj.cn

JS:   class User {}
来源：http://bt.colortex.cn

TS:   class User { name: string = ""; }
来源：http://il.521024.cn

Java: class User {}
来源：http://fe.szxytkj.cn

Go:   type User struct { Name string }
来源：http://cj.haigaiapp.cn

Ruby: class User; end
来源：http://yn.huanxung.cn

C#:   class User {}
来源：http://zj.huixinmuqiang.cn

[G02] 构造函数
来源：http://hm.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://bs.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://fs.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://ao.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://za.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://rr.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://if.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://qx.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://ye.yuntaijiaju.cn

[G03] 实例属性
来源：http://qr.bookmarksfly.cn

Py:   self.name = "x"
来源：http://ew.colortex.cn

PHP:  public string $name = "x";
来源：http://ie.newstarts.cn

JS:   this.name = "x";
来源：http://md.wgjwhj.cn

TS:   name: string = "x";
来源：http://dq.hahajie.cn

Java: private String name;
来源：http://li.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rw.gzmigu.cn

Ruby: @name = "x"
来源：http://by.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://rz.szsharing.cn

[G04] 定义方法
来源：http://ur.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://hp.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hc.szsharing.cn

JS:   greet() { return this.name; }
来源：http://ea.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://go.newstarts.cn

Java: String greet() { return name; }
来源：http://zr.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ma.shxzukj.cn

Ruby: def greet; @name; end
来源：http://od.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://ws.bjjhwx.cn

[G05] 继承
来源：http://xs.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://gj.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://lc.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://zk.nicolike.cn

TS:   class Admin extends User {}
来源：http://tg.nicolike.cn

Java: class Admin extends User {}
来源：http://rr.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tk.9csxet.cn

Ruby: class Admin < User; end
来源：http://lo.hahajie.cn

C#:   class Admin : User {}
来源：http://xm.huanxung.cn

[G06] 重写方法
来源：http://ld.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://fl.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://em.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://tj.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://ij.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ud.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gq.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://vy.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://py.9csxet.cn

[G07] 调用父类方法
来源：http://mr.gzmigu.cn

Py:   super().greet()
来源：http://aa.bookmarksfly.cn

PHP:  parent::greet();
来源：http://aq.asd995.cn

JS:   super.greet();
来源：http://om.bookmarksfly.cn

TS:   super.greet();
来源：http://pc.panjiajie.cn

Java: super.greet();
来源：http://js.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jo.huixiangedu.cn

Ruby: super
来源：http://zj.colortex.cn

C#:   base.Greet();
来源：http://sf.jctech888.com.cn

[G08] 静态方法与属性
来源：http://pn.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sw.panjiajie.cn

PHP:  public static function f() {}
来源：http://jy.yuexingan06.cn

JS:   static f() {}
来源：http://vn.colortex.cn

TS:   static f(): void {}
来源：http://pl.bjjhwx.cn

Java: static void f() {}
来源：http://nq.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://up.muxihuayi.cn

Ruby: def self.f; end
来源：http://fl.shtwfgs.cn

C#:   public static void F() {}
来源：http://lh.newstarts.cn

[G09] 接口 / 抽象类
来源：http://it.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://mm.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ia.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bk.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://qw.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://sz.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://sd.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nc.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://np.yuexingan06.cn

[G10] 访问控制
来源：http://ns.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://wq.haigaiapp.cn

PHP:  public / protected / private
来源：http://uo.colortex.cn

JS:   #private 字段；其余公开
来源：http://xd.lnxyls.cn

TS:   public / protected / private
来源：http://jh.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://rk.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ib.bjjhwx.cn

Ruby: public / protected / private
来源：http://ss.hnjuh.cn

C#:   public / protected / private / internal
来源：http://cv.yuexingan06.cn

[G11] getter / setter
来源：http://qd.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://lc.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vo.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://so.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://qs.hnjuh.cn

Java: public String getName() { return name; }
来源：http://ny.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nc.huanxung.cn

Ruby: attr_accessor :name
来源：http://kc.huanxung.cn

C#:   public string Name { get; set; }
来源：http://zb.bjjhwx.cn

[G12] 对象转字符串
来源：http://rt.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://bz.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pz.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://iu.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://gq.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://lw.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yg.asd995.cn

Ruby: def to_s; @name; end
来源：http://sc.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://nt.wgjwhj.cn

[G13] 判断对象类型
来源：http://xf.panjiajie.cn

Py:   isinstance(u, User)
来源：http://eo.hahajie.cn

PHP:  $u instanceof User
来源：http://da.hnjuh.cn

JS:   u instanceof User
来源：http://cy.yuntaijiaju.cn

TS:   u instanceof User
来源：http://lw.bookmarksfly.cn

Java: u instanceof User
来源：http://bt.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tn.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://lm.szxytkj.cn

C#:   u is User
来源：http://yi.huanxung.cn

[G14] 数据类 / record
来源：http://ay.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jd.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://dm.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jd.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://sy.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://ve.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://gf.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ed.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://bx.nicolike.cn

[G15] 枚举
来源：http://kb.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dq.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rb.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kg.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mv.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://ec.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ur.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://fu.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ua.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://tu.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ko.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://yo.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://pv.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://qv.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rd.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://id.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://bg.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://xx.gzmigu.cn

================================================================================
来源：http://ea.szxytkj.cn

H. 异常与错误处理
来源：http://cl.huanxung.cn

================================================================================
来源：http://bs.jctech888.com.cn

[H01] try / catch 基础
来源：http://kc.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pt.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cq.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xx.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://th.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nt.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lz.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lz.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://wm.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yw.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ul.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wh.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://st.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iu.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ft.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sy.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ng.jctech888.com.cn

[H03] 主动抛出异常
来源：http://td.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://kf.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mi.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://sa.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://xw.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ey.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rc.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ey.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://di.gzmigu.cn

[H04] 自定义异常类型
来源：http://ys.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://hz.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lo.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://yo.nszjky.cn

TS:   class MyError extends Error {}
来源：http://mv.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://nk.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cw.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://hc.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://ff.jctech888.com.cn

[H05] 捕获特定类型
来源：http://zi.shtwfgs.cn

Py:   except ValueError as e:
来源：http://ww.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ew.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://bq.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://rm.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://dq.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ye.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://ei.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cd.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://gg.hahajie.cn

Py:   value = d.get("k") or default
来源：http://qr.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qq.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tb.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tq.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tz.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fx.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://nf.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://lh.gzmigu.cn

[H07] 断言
来源：http://zt.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ot.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://lz.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://oq.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://zg.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://ol.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sd.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lo.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://ne.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://nu.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://pz.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ie.newstarts.cn

JS:   e.message;  e.stack
来源：http://pf.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://on.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cd.yuexingan06.cn

Go:   err.Error()
来源：http://fk.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://cb.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://te.hnjuh.cn

[H09] 带错误码的异常
来源：http://gg.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://st.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iw.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ut.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bf.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ar.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://za.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pm.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dm.nicolike.cn

[H10] 资源自动释放
来源：http://sq.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ug.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rb.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ma.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tq.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hh.newstarts.cn

Go:   defer f.Close()
来源：http://dy.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bq.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lw.colortex.cn

================================================================================
来源：http://zw.nicolike.cn

I. 正则表达式
来源：http://eb.shxzukj.cn

================================================================================
来源：http://fo.yuexingan06.cn

[I01] 判断是否匹配
来源：http://pe.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oz.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eq.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://pg.nicolike.cn

TS:   /\d+/.test(s)
来源：http://gq.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mh.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nb.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://mi.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wc.jctech888.com.cn

[I02] 提取所有匹配
来源：http://pg.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://nn.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vc.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zj.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://uy.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oi.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cw.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://sq.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ni.hahajie.cn

[I03] 提取捕获分组
来源：http://az.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gc.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sv.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ll.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mn.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oc.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lf.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bd.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dt.panjiajie.cn

[I04] 正则替换
来源：http://xz.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ws.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rf.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zw.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rb.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mc.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wt.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sh.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dw.9csxet.cn

[I05] 按正则拆分
来源：http://fj.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pd.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sk.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://ey.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://si.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://bx.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xt.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cz.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kw.521024.cn


<!-- 参考信息 -->