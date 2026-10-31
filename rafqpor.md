代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://te.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ys.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vt.huixinmuqiang.cn

TS:   // 同上
来源：http://pp.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qr.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lq.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qj.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oc.panjiajie.cn

================================================================================
来源：http://bh.haigaiapp.cn

G. 面向对象
来源：http://on.gzmigu.cn

================================================================================
来源：http://dg.szsharing.cn

[G01] 定义类
来源：http://sc.wgjwhj.cn

Py:   class User: pass
来源：http://xr.9csxet.cn

PHP:  class User {}
来源：http://qt.szxytkj.cn

JS:   class User {}
来源：http://kl.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://zk.chemitech.net.cn

Java: class User {}
来源：http://mx.nicolike.cn

Go:   type User struct { Name string }
来源：http://lv.huanxung.cn

Ruby: class User; end
来源：http://hh.szsharing.cn

C#:   class User {}
来源：http://ik.szxytkj.cn

[G02] 构造函数
来源：http://lq.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://mw.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://yp.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://be.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://yk.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://et.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mu.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://wl.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://lu.colortex.cn

[G03] 实例属性
来源：http://fn.shtwfgs.cn

Py:   self.name = "x"
来源：http://iy.shxzukj.cn

PHP:  public string $name = "x";
来源：http://fj.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ji.huanxung.cn

TS:   name: string = "x";
来源：http://mu.521024.cn

Java: private String name;
来源：http://kp.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vl.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://zw.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://kq.haigaiapp.cn

[G04] 定义方法
来源：http://jy.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://kt.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zc.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://mj.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://xm.asd995.cn

Java: String greet() { return name; }
来源：http://bc.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ik.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://zd.huanxung.cn

C#:   public string Greet() => Name;
来源：http://lz.panjiajie.cn

[G05] 继承
来源：http://pl.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://hu.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://lu.9csxet.cn

JS:   class Admin extends User {}
来源：http://iw.gzmigu.cn

TS:   class Admin extends User {}
来源：http://pn.asd995.cn

Java: class Admin extends User {}
来源：http://tt.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oa.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://as.hahajie.cn

C#:   class Admin : User {}
来源：http://ap.lnxyls.cn

[G06] 重写方法
来源：http://dt.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://bh.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tq.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://qy.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://vn.hnjuh.cn

Java: @Override String greet() { return "admin"; }
来源：http://th.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://in.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://xg.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://zg.hnjuh.cn

[G07] 调用父类方法
来源：http://xf.szsharing.cn

Py:   super().greet()
来源：http://do.gzmigu.cn

PHP:  parent::greet();
来源：http://oq.shxzukj.cn

JS:   super.greet();
来源：http://vx.nicolike.cn

TS:   super.greet();
来源：http://we.shxzukj.cn

Java: super.greet();
来源：http://rd.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tk.colortex.cn

Ruby: super
来源：http://yv.huixiangedu.cn

C#:   base.Greet();
来源：http://dl.haigaiapp.cn

[G08] 静态方法与属性
来源：http://rd.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ur.hahajie.cn

PHP:  public static function f() {}
来源：http://tt.muxihuayi.cn

JS:   static f() {}
来源：http://bg.nicolike.cn

TS:   static f(): void {}
来源：http://ic.hnjuh.cn

Java: static void f() {}
来源：http://uo.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vv.shxzskj.cn

Ruby: def self.f; end
来源：http://zw.nszjky.cn

C#:   public static void F() {}
来源：http://iq.huanxung.cn

[G09] 接口 / 抽象类
来源：http://nm.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://jk.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dn.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://id.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://xu.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://en.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://kt.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xs.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://se.hahajie.cn

[G10] 访问控制
来源：http://ms.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://di.bookmarksfly.cn

PHP:  public / protected / private
来源：http://ts.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://wh.haigaiapp.cn

TS:   public / protected / private
来源：http://fv.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://im.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ka.muxihuayi.cn

Ruby: public / protected / private
来源：http://nf.panjiajie.cn

C#:   public / protected / private / internal
来源：http://pz.haigaiapp.cn

[G11] getter / setter
来源：http://lw.shtwfgs.cn

Py:   @property 与 @x.setter
来源：http://vh.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qp.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://zy.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://zp.newstarts.cn

Java: public String getName() { return name; }
来源：http://qi.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zq.521024.cn

Ruby: attr_accessor :name
来源：http://yy.nszjky.cn

C#:   public string Name { get; set; }
来源：http://fu.panjiajie.cn

[G12] 对象转字符串
来源：http://mm.521024.cn

Py:   def __str__(self): return self.name
来源：http://pn.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qe.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://lu.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://fs.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://tg.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://su.huanxung.cn

Ruby: def to_s; @name; end
来源：http://qb.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://ue.muxihuayi.cn

[G13] 判断对象类型
来源：http://lk.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://wz.szxytkj.cn

PHP:  $u instanceof User
来源：http://tb.haigaiapp.cn

JS:   u instanceof User
来源：http://ph.lnxyls.cn

TS:   u instanceof User
来源：http://wr.panjiajie.cn

Java: u instanceof User
来源：http://uz.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qc.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://tr.jctech888.com.cn

C#:   u is User
来源：http://sl.wgjwhj.cn

[G14] 数据类 / record
来源：http://ga.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lq.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://px.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rp.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ig.newstarts.cn

Java: record User(String name, int age) {}
来源：http://rq.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://ur.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vx.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://rl.jianghongdianzi.cn

[G15] 枚举
来源：http://gn.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://om.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hg.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lx.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fd.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://fs.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ik.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://ol.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xc.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://dz.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ft.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://ba.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://xg.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://lx.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aq.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ms.521024.cn

Ruby: obj.instance_variables
来源：http://du.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://fc.colortex.cn

================================================================================
来源：http://ej.521024.cn

H. 异常与错误处理
来源：http://gt.huixiangedu.cn

================================================================================
来源：http://dq.asd995.cn

[H01] try / catch 基础
来源：http://ao.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ve.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yh.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://up.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ze.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uo.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sr.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jt.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ko.newstarts.cn

[H02] finally / ensure 收尾
来源：http://fi.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wq.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lk.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wq.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://be.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jv.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iu.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://em.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://om.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://pc.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://uy.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cd.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://yf.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://sf.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ps.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ms.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zz.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pr.gzmigu.cn

[H04] 自定义异常类型
来源：http://tu.asd995.cn

Py:   class MyError(Exception): pass
来源：http://xr.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ua.newstarts.cn

JS:   class MyError extends Error {}
来源：http://ho.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://tn.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://yx.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fl.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://av.newstarts.cn

C#:   class MyException : Exception {}
来源：http://hy.jctech888.com.cn

[H05] 捕获特定类型
来源：http://xu.9csxet.cn

Py:   except ValueError as e:
来源：http://os.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fy.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://zv.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://zi.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://zi.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tv.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://dl.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qf.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://yk.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://so.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fq.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nf.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jo.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ji.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ez.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://vo.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://ik.jianghongdianzi.cn

[H07] 断言
来源：http://qj.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://pr.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://td.szsharing.cn

JS:   console.assert(x > 0);
来源：http://ve.szsharing.cn

TS:   console.assert(x > 0);
来源：http://su.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://mh.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gt.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ai.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://ru.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://qu.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://yo.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mh.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://bj.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kt.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wp.gzmigu.cn

Go:   err.Error()
来源：http://nr.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://cu.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://ad.colortex.cn

[H09] 带错误码的异常
来源：http://kn.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lw.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ra.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uh.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wi.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yg.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nl.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jo.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://td.nicolike.cn

[H10] 资源自动释放
来源：http://mo.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nl.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xp.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fl.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://py.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qj.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://ij.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bz.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ll.muxihuayi.cn

================================================================================
来源：http://zg.newstarts.cn

I. 正则表达式
来源：http://xk.huixinmuqiang.cn

================================================================================
来源：http://km.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://ov.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qr.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zo.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://ok.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://vm.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ls.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yg.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://zx.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ec.nszjky.cn

[I02] 提取所有匹配
来源：http://ys.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://za.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hm.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fk.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://je.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dn.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bz.521024.cn

Ruby: s.scan(/\d+/)
来源：http://vn.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bv.shtwfgs.cn

[I03] 提取捕获分组
来源：http://je.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gm.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oy.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ky.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xl.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wl.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wi.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ny.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tg.wgjwhj.cn

[I04] 正则替换
来源：http://gq.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ku.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zz.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eh.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sm.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wz.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://to.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wd.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://id.chemitech.net.cn

[I05] 按正则拆分
来源：http://uv.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ii.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iw.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://pk.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://cz.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://vj.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qu.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ry.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vk.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xw.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vo.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://no.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fu.muxihuayi.cn


<!-- 参考信息 -->