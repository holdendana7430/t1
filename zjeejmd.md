代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dv.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pr.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jf.yuexingan06.cn

TS:   // 同上
来源：http://ai.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://am.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hr.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hg.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ot.wgjwhj.cn

================================================================================
来源：http://fx.bjjhwx.cn

G. 面向对象
来源：http://so.yuexingan06.cn

================================================================================
来源：http://ll.shtwfgs.cn

[G01] 定义类
来源：http://bo.asd995.cn

Py:   class User: pass
来源：http://zi.nicolike.cn

PHP:  class User {}
来源：http://ff.hahajie.cn

JS:   class User {}
来源：http://vv.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://yb.chemitech.net.cn

Java: class User {}
来源：http://qy.gzmigu.cn

Go:   type User struct { Name string }
来源：http://mw.colortex.cn

Ruby: class User; end
来源：http://uo.asd995.cn

C#:   class User {}
来源：http://ds.nicolike.cn

[G02] 构造函数
来源：http://fr.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://kc.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://vv.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://ny.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://os.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://mr.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dy.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gk.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://jq.9csxet.cn

[G03] 实例属性
来源：http://iz.jctech888.com.cn

Py:   self.name = "x"
来源：http://wj.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://tm.szsharing.cn

JS:   this.name = "x";
来源：http://ak.panjiajie.cn

TS:   name: string = "x";
来源：http://ej.asd995.cn

Java: private String name;
来源：http://pg.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rp.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://lv.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://xs.bjjhwx.cn

[G04] 定义方法
来源：http://rx.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://fa.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tc.9csxet.cn

JS:   greet() { return this.name; }
来源：http://dg.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://bs.bjjhwx.cn

Java: String greet() { return name; }
来源：http://nt.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wo.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://zo.nicolike.cn

C#:   public string Greet() => Name;
来源：http://vq.yuntaijiaju.cn

[G05] 继承
来源：http://ws.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://fb.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://fs.hahajie.cn

JS:   class Admin extends User {}
来源：http://lj.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://hm.gzmigu.cn

Java: class Admin extends User {}
来源：http://qe.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zs.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://rb.asd995.cn

C#:   class Admin : User {}
来源：http://mp.asd995.cn

[G06] 重写方法
来源：http://ad.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://ry.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bn.asd995.cn

JS:   greet() { return "admin"; }
来源：http://tp.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://pd.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://tm.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ga.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://bv.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://uc.shxzskj.cn

[G07] 调用父类方法
来源：http://td.jianghongdianzi.cn

Py:   super().greet()
来源：http://mb.shxzukj.cn

PHP:  parent::greet();
来源：http://wc.hahajie.cn

JS:   super.greet();
来源：http://ey.shxzukj.cn

TS:   super.greet();
来源：http://zi.hahajie.cn

Java: super.greet();
来源：http://fj.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sp.szxytkj.cn

Ruby: super
来源：http://uw.hahajie.cn

C#:   base.Greet();
来源：http://ii.shxzskj.cn

[G08] 静态方法与属性
来源：http://ax.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wn.colortex.cn

PHP:  public static function f() {}
来源：http://nx.huanxung.cn

JS:   static f() {}
来源：http://hz.bjjhwx.cn

TS:   static f(): void {}
来源：http://oi.nszjky.cn

Java: static void f() {}
来源：http://vo.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sj.muxihuayi.cn

Ruby: def self.f; end
来源：http://xa.asd995.cn

C#:   public static void F() {}
来源：http://ed.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://gy.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://lf.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ug.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kk.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://hv.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://sm.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://lb.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cl.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://hu.shtwfgs.cn

[G10] 访问控制
来源：http://wh.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://pq.nszjky.cn

PHP:  public / protected / private
来源：http://iq.521024.cn

JS:   #private 字段；其余公开
来源：http://uq.shtwfgs.cn

TS:   public / protected / private
来源：http://ur.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://br.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nt.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://oy.hnjuh.cn

C#:   public / protected / private / internal
来源：http://wu.colortex.cn

[G11] getter / setter
来源：http://tw.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://hp.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hr.colortex.cn

JS:   get name() { return this._name; }
来源：http://vo.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://xu.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://qa.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fq.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://th.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://pt.shxzskj.cn

[G12] 对象转字符串
来源：http://uv.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://kt.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uh.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://uc.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://vi.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://qr.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eb.521024.cn

Ruby: def to_s; @name; end
来源：http://it.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://ii.shxzukj.cn

[G13] 判断对象类型
来源：http://oj.nicolike.cn

Py:   isinstance(u, User)
来源：http://ao.huixiangedu.cn

PHP:  $u instanceof User
来源：http://ke.bjjhwx.cn

JS:   u instanceof User
来源：http://an.huanxung.cn

TS:   u instanceof User
来源：http://tt.gzmigu.cn

Java: u instanceof User
来源：http://et.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gu.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://rf.hnjuh.cn

C#:   u is User
来源：http://vw.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://nt.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yx.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://yc.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://so.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://tc.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://qx.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://jd.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wd.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://go.huanxung.cn

[G15] 枚举
来源：http://cy.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vz.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eo.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sr.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tn.521024.cn

Java: enum Color { RED, GREEN }
来源：http://cq.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fz.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://oi.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oi.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://cg.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pv.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://xj.hnjuh.cn

JS:   Object.entries(obj)
来源：http://em.asd995.cn

TS:   Object.entries(obj)
来源：http://ya.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ui.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yt.huanxung.cn

Ruby: obj.instance_variables
来源：http://cq.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://iq.szsharing.cn

================================================================================
来源：http://qa.haigaiapp.cn

H. 异常与错误处理
来源：http://ou.bookmarksfly.cn

================================================================================
来源：http://up.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://bq.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nx.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fc.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://va.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fy.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rt.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kk.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ou.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tx.newstarts.cn

[H02] finally / ensure 收尾
来源：http://fw.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vk.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yn.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eo.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ng.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lt.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pn.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ao.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jb.szxytkj.cn

[H03] 主动抛出异常
来源：http://pk.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://ok.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://td.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://kr.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://xg.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://of.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mw.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fq.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ay.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://yf.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://pe.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tq.nszjky.cn

JS:   class MyError extends Error {}
来源：http://ez.colortex.cn

TS:   class MyError extends Error {}
来源：http://pz.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://ak.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lt.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://dn.colortex.cn

C#:   class MyException : Exception {}
来源：http://ac.wgjwhj.cn

[H05] 捕获特定类型
来源：http://xb.bjjhwx.cn

Py:   except ValueError as e:
来源：http://ty.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bi.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://si.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://wo.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://wg.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mj.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://rz.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://os.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://kq.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://rj.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pp.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lu.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kk.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tb.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gm.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://au.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://jj.haigaiapp.cn

[H07] 断言
来源：http://mm.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://df.panjiajie.cn

PHP:  assert($x > 0);
来源：http://so.newstarts.cn

JS:   console.assert(x > 0);
来源：http://cx.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://hd.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://hf.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sm.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fq.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://kf.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://vj.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://kl.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ya.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://yo.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ir.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ge.szxytkj.cn

Go:   err.Error()
来源：http://my.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://hw.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://sm.yuexingan06.cn

[H09] 带错误码的异常
来源：http://yn.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vk.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://re.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://or.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ng.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zp.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wk.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bp.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ry.yuexingan06.cn

[H10] 资源自动释放
来源：http://ml.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bm.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vr.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fs.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mk.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nc.colortex.cn

Go:   defer f.Close()
来源：http://hr.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ft.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tt.colortex.cn

================================================================================
来源：http://fi.huanxung.cn

I. 正则表达式
来源：http://lx.bjjhwx.cn

================================================================================
来源：http://kh.wgjwhj.cn

[I01] 判断是否匹配
来源：http://zb.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yx.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gy.nszjky.cn

JS:   /\d+/.test(s)
来源：http://rb.szsharing.cn

TS:   /\d+/.test(s)
来源：http://xp.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nn.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nn.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://jg.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ev.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://ag.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://yw.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bk.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://in.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://wh.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bk.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ij.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://cs.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sl.huixiangedu.cn

[I03] 提取捕获分组
来源：http://dx.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gq.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jc.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fc.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gx.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jn.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://le.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uw.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iz.asd995.cn

[I04] 正则替换
来源：http://wc.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://at.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://el.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://im.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ge.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pv.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dt.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hu.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jl.yuexingan06.cn

[I05] 按正则拆分
来源：http://he.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bf.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pj.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ck.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://hd.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://fj.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://px.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ku.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wr.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wx.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bk.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jn.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.muxihuayi.cn


<!-- 参考信息 -->