代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mz.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pp.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dm.521024.cn

[F12] CSV 读写
来源：http://nk.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bv.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qt.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bi.colortex.cn

TS:   // 同上
来源：http://fx.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ie.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ew.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fy.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iz.wgjwhj.cn

================================================================================
来源：http://om.huixiangedu.cn

G. 面向对象
来源：http://gu.newstarts.cn

================================================================================
来源：http://gi.szxytkj.cn

[G01] 定义类
来源：http://js.nszjky.cn

Py:   class User: pass
来源：http://lp.shxzukj.cn

PHP:  class User {}
来源：http://zw.szsharing.cn

JS:   class User {}
来源：http://nl.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://kk.gzmigu.cn

Java: class User {}
来源：http://wf.nicolike.cn

Go:   type User struct { Name string }
来源：http://qu.huixinmuqiang.cn

Ruby: class User; end
来源：http://rm.colortex.cn

C#:   class User {}
来源：http://co.szxytkj.cn

[G02] 构造函数
来源：http://cj.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://rf.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://mt.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://vt.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://rl.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://fu.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ut.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://qi.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ik.colortex.cn

[G03] 实例属性
来源：http://er.gzmigu.cn

Py:   self.name = "x"
来源：http://gq.hahajie.cn

PHP:  public string $name = "x";
来源：http://kq.nicolike.cn

JS:   this.name = "x";
来源：http://sf.szxytkj.cn

TS:   name: string = "x";
来源：http://qs.yuexingan06.cn

Java: private String name;
来源：http://tb.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pj.muxihuayi.cn

Ruby: @name = "x"
来源：http://ty.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://bv.hnjuh.cn

[G04] 定义方法
来源：http://wk.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://vj.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nl.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://qj.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://ke.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://tk.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ht.lnxyls.cn

Ruby: def greet; @name; end
来源：http://mu.nicolike.cn

C#:   public string Greet() => Name;
来源：http://mr.panjiajie.cn

[G05] 继承
来源：http://qq.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ub.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://oq.lnxyls.cn

JS:   class Admin extends User {}
来源：http://eu.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://oq.szsharing.cn

Java: class Admin extends User {}
来源：http://jj.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fc.newstarts.cn

Ruby: class Admin < User; end
来源：http://pe.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://yf.huixiangedu.cn

[G06] 重写方法
来源：http://ke.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://mi.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kf.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://mq.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://ta.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://mp.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bh.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://rl.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://wa.hahajie.cn

[G07] 调用父类方法
来源：http://rb.9csxet.cn

Py:   super().greet()
来源：http://nc.shxzskj.cn

PHP:  parent::greet();
来源：http://nc.bookmarksfly.cn

JS:   super.greet();
来源：http://jp.yuntaijiaju.cn

TS:   super.greet();
来源：http://ep.chemitech.net.cn

Java: super.greet();
来源：http://mc.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jz.bjjhwx.cn

Ruby: super
来源：http://yv.gzmigu.cn

C#:   base.Greet();
来源：http://hg.shtwfgs.cn

[G08] 静态方法与属性
来源：http://iw.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rx.nicolike.cn

PHP:  public static function f() {}
来源：http://ie.haigaiapp.cn

JS:   static f() {}
来源：http://vd.newstarts.cn

TS:   static f(): void {}
来源：http://ah.gzmigu.cn

Java: static void f() {}
来源：http://od.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://an.shxzukj.cn

Ruby: def self.f; end
来源：http://nz.gzmigu.cn

C#:   public static void F() {}
来源：http://wk.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://mf.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://mf.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lo.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jr.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://xw.9csxet.cn

Java: interface Shape { double area(); }
来源：http://zl.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://mt.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tm.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://zb.nszjky.cn

[G10] 访问控制
来源：http://vn.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://bn.wgjwhj.cn

PHP:  public / protected / private
来源：http://pp.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://au.bookmarksfly.cn

TS:   public / protected / private
来源：http://ec.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://og.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yx.hnjuh.cn

Ruby: public / protected / private
来源：http://br.hnjuh.cn

C#:   public / protected / private / internal
来源：http://ur.shxzskj.cn

[G11] getter / setter
来源：http://ym.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://hh.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ta.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://cy.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://yo.9csxet.cn

Java: public String getName() { return name; }
来源：http://tw.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jx.colortex.cn

Ruby: attr_accessor :name
来源：http://oy.szsharing.cn

C#:   public string Name { get; set; }
来源：http://lm.nicolike.cn

[G12] 对象转字符串
来源：http://mn.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://rs.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vv.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://pq.521024.cn

TS:   toString(): string { return this.name; }
来源：http://zy.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://da.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ch.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://gr.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://lr.bookmarksfly.cn

[G13] 判断对象类型
来源：http://ll.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://uc.szsharing.cn

PHP:  $u instanceof User
来源：http://lh.colortex.cn

JS:   u instanceof User
来源：http://xb.hnjuh.cn

TS:   u instanceof User
来源：http://nt.chemitech.net.cn

Java: u instanceof User
来源：http://rx.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ej.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://nz.huixinmuqiang.cn

C#:   u is User
来源：http://hx.huixiangedu.cn

[G14] 数据类 / record
来源：http://gf.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lf.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://nl.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sc.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://tq.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://tk.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://bb.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vq.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://od.bjjhwx.cn

[G15] 枚举
来源：http://wb.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yz.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hi.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hg.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gm.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://kt.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gn.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://hy.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kj.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ly.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mp.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://wz.hahajie.cn

JS:   Object.entries(obj)
来源：http://ak.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://pj.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pt.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nk.hnjuh.cn

Ruby: obj.instance_variables
来源：http://xe.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://kk.yuexingan06.cn

================================================================================
来源：http://he.szxytkj.cn

H. 异常与错误处理
来源：http://px.shxzskj.cn

================================================================================
来源：http://xs.colortex.cn

[H01] try / catch 基础
来源：http://vz.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ub.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rf.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ba.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sm.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bx.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gt.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ic.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ph.nszjky.cn

[H02] finally / ensure 收尾
来源：http://kf.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vg.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ot.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ff.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mu.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mu.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hb.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://am.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gk.panjiajie.cn

[H03] 主动抛出异常
来源：http://rq.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://pu.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gu.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://rt.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://em.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ma.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ib.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hp.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kv.chemitech.net.cn

[H04] 自定义异常类型
来源：http://ar.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://ds.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ai.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://zn.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://qi.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://ux.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ab.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://ev.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://cm.shxzukj.cn

[H05] 捕获特定类型
来源：http://sb.lnxyls.cn

Py:   except ValueError as e:
来源：http://qj.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ql.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://rr.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://we.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://dv.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hh.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://la.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hv.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://nu.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://tm.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gk.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fs.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sd.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wp.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yd.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://as.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://lr.nszjky.cn

[H07] 断言
来源：http://bg.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://ui.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://rv.9csxet.cn

JS:   console.assert(x > 0);
来源：http://lr.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://qx.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://vx.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uk.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jq.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://mh.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://py.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://hs.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://go.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://zt.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://en.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dc.huanxung.cn

Go:   err.Error()
来源：http://cx.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://oe.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ua.wgjwhj.cn

[H09] 带错误码的异常
来源：http://vw.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wi.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qs.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iv.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fk.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xc.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ig.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tg.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gi.nicolike.cn

[H10] 资源自动释放
来源：http://zx.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ps.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aa.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gh.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yz.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ix.wgjwhj.cn

Go:   defer f.Close()
来源：http://yp.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vj.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lo.gzmigu.cn

================================================================================
来源：http://to.haigaiapp.cn

I. 正则表达式
来源：http://ez.haigaiapp.cn

================================================================================
来源：http://rt.asd995.cn

[I01] 判断是否匹配
来源：http://lr.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ys.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jj.asd995.cn

JS:   /\d+/.test(s)
来源：http://gb.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://kj.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ge.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vb.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://nf.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gs.521024.cn

[I02] 提取所有匹配
来源：http://ci.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://tp.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ud.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hr.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://nk.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gl.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ug.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://cv.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tu.haigaiapp.cn

[I03] 提取捕获分组
来源：http://ux.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nc.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://in.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ck.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://le.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://et.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xj.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fu.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ci.yuntaijiaju.cn

[I04] 正则替换
来源：http://gd.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dv.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jv.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fm.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://os.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ki.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://by.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jv.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ni.9csxet.cn

[I05] 按正则拆分
来源：http://tq.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nw.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rg.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://nt.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ws.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://jl.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eh.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lk.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nl.muxihuayi.cn


<!-- 参考信息 -->