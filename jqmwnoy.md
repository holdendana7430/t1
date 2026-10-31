代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pd.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qr.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ll.huixinmuqiang.cn

TS:   // 同上
来源：http://vo.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xb.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xv.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://br.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bj.wgjwhj.cn

================================================================================
来源：http://uo.nszjky.cn

G. 面向对象
来源：http://ge.newstarts.cn

================================================================================
来源：http://kz.shxzskj.cn

[G01] 定义类
来源：http://do.haigaiapp.cn

Py:   class User: pass
来源：http://qp.jctech888.com.cn

PHP:  class User {}
来源：http://yo.521024.cn

JS:   class User {}
来源：http://vn.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://mp.szsharing.cn

Java: class User {}
来源：http://eu.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://sc.chemitech.net.cn

Ruby: class User; end
来源：http://qf.wgjwhj.cn

C#:   class User {}
来源：http://br.asd995.cn

[G02] 构造函数
来源：http://fy.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://lh.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://fg.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://rp.chemitech.net.cn

TS:   constructor(public name: string) {}
来源：http://hp.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://fm.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ga.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ry.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://hy.yuntaijiaju.cn

[G03] 实例属性
来源：http://th.bookmarksfly.cn

Py:   self.name = "x"
来源：http://jd.panjiajie.cn

PHP:  public string $name = "x";
来源：http://nw.muxihuayi.cn

JS:   this.name = "x";
来源：http://rd.lnxyls.cn

TS:   name: string = "x";
来源：http://ss.yuntaijiaju.cn

Java: private String name;
来源：http://sc.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nr.jctech888.com.cn

Ruby: @name = "x"
来源：http://qe.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://iz.yuexingan06.cn

[G04] 定义方法
来源：http://du.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://kg.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sq.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://uj.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://pn.bjjhwx.cn

Java: String greet() { return name; }
来源：http://qz.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bf.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://vb.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://jf.shxzskj.cn

[G05] 继承
来源：http://jh.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://qj.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://ri.szxytkj.cn

JS:   class Admin extends User {}
来源：http://fv.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://ef.shxzskj.cn

Java: class Admin extends User {}
来源：http://qr.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gc.asd995.cn

Ruby: class Admin < User; end
来源：http://dy.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://ku.yuexingan06.cn

[G06] 重写方法
来源：http://rq.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://rt.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gn.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://zl.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://vp.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://xm.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://at.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://ba.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://rd.nicolike.cn

[G07] 调用父类方法
来源：http://vv.shtwfgs.cn

Py:   super().greet()
来源：http://bm.shxzskj.cn

PHP:  parent::greet();
来源：http://xv.hnjuh.cn

JS:   super.greet();
来源：http://kw.hnjuh.cn

TS:   super.greet();
来源：http://rs.szxytkj.cn

Java: super.greet();
来源：http://lr.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://je.huixiangedu.cn

Ruby: super
来源：http://xs.huanxung.cn

C#:   base.Greet();
来源：http://of.hnjuh.cn

[G08] 静态方法与属性
来源：http://zv.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tp.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://nh.nicolike.cn

JS:   static f() {}
来源：http://hx.shxzukj.cn

TS:   static f(): void {}
来源：http://vx.newstarts.cn

Java: static void f() {}
来源：http://sm.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ec.huanxung.cn

Ruby: def self.f; end
来源：http://du.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://mz.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://wb.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://uj.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mn.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ri.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://hl.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://pg.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://mg.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sa.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://nu.lnxyls.cn

[G10] 访问控制
来源：http://eb.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://nx.nicolike.cn

PHP:  public / protected / private
来源：http://hj.nicolike.cn

JS:   #private 字段；其余公开
来源：http://ku.gzmigu.cn

TS:   public / protected / private
来源：http://io.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://lk.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ui.bjjhwx.cn

Ruby: public / protected / private
来源：http://oq.szsharing.cn

C#:   public / protected / private / internal
来源：http://mp.huixinmuqiang.cn

[G11] getter / setter
来源：http://us.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://vp.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wx.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://fn.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://dc.colortex.cn

Java: public String getName() { return name; }
来源：http://ry.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dv.9csxet.cn

Ruby: attr_accessor :name
来源：http://dy.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://cr.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://pk.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ok.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jz.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://xv.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://uo.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://us.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kl.asd995.cn

Ruby: def to_s; @name; end
来源：http://el.asd995.cn

C#:   public override string ToString() => Name;
来源：http://ca.haigaiapp.cn

[G13] 判断对象类型
来源：http://vd.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://vp.newstarts.cn

PHP:  $u instanceof User
来源：http://hr.hnjuh.cn

JS:   u instanceof User
来源：http://yl.huanxung.cn

TS:   u instanceof User
来源：http://ya.gzmigu.cn

Java: u instanceof User
来源：http://la.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qq.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://jq.jctech888.com.cn

C#:   u is User
来源：http://ve.shxzskj.cn

[G14] 数据类 / record
来源：http://zw.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tn.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ya.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xl.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://on.hahajie.cn

Java: record User(String name, int age) {}
来源：http://eg.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://ju.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wx.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://nl.jianghongdianzi.cn

[G15] 枚举
来源：http://bk.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iq.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rm.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mp.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wg.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://lp.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iw.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://xz.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yi.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://wf.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fw.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://ih.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://of.huanxung.cn

TS:   Object.entries(obj)
来源：http://ri.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cw.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gj.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://jb.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://zi.huixinmuqiang.cn

================================================================================
来源：http://oc.bookmarksfly.cn

H. 异常与错误处理
来源：http://xt.gzmigu.cn

================================================================================
来源：http://ex.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://ec.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://em.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mw.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pu.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vi.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mz.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ai.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tu.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nt.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://od.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lt.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ju.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ai.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ws.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wg.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ne.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://os.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jl.shxzukj.cn

[H03] 主动抛出异常
来源：http://ii.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://wd.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jy.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://jo.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://zb.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rb.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cs.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ju.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kt.shxzskj.cn

[H04] 自定义异常类型
来源：http://tk.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://cq.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ne.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://wq.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ud.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://vo.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vr.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://tk.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://xt.huixiangedu.cn

[H05] 捕获特定类型
来源：http://hx.shtwfgs.cn

Py:   except ValueError as e:
来源：http://sl.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fm.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://pg.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://rv.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://nb.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oz.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://cm.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://go.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://lj.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://ez.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pa.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dz.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jd.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nb.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ar.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://oq.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://dh.hnjuh.cn

[H07] 断言
来源：http://hc.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://eg.nicolike.cn

PHP:  assert($x > 0);
来源：http://pn.newstarts.cn

JS:   console.assert(x > 0);
来源：http://ph.hahajie.cn

TS:   console.assert(x > 0);
来源：http://ra.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://wl.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://db.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://la.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://av.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://co.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://nr.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hw.lnxyls.cn

JS:   e.message;  e.stack
来源：http://dc.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jg.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://og.haigaiapp.cn

Go:   err.Error()
来源：http://xm.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://os.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://lk.lnxyls.cn

[H09] 带错误码的异常
来源：http://ql.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rx.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ps.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qd.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://es.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bh.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ew.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xu.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xo.wgjwhj.cn

[H10] 资源自动释放
来源：http://bb.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oh.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vq.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ac.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rg.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aw.yuexingan06.cn

Go:   defer f.Close()
来源：http://bd.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fh.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hd.521024.cn

================================================================================
来源：http://ak.szsharing.cn

I. 正则表达式
来源：http://oy.hahajie.cn

================================================================================
来源：http://ed.9csxet.cn

[I01] 判断是否匹配
来源：http://bf.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oa.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lf.asd995.cn

JS:   /\d+/.test(s)
来源：http://ss.colortex.cn

TS:   /\d+/.test(s)
来源：http://lt.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rq.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oh.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://fh.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://je.asd995.cn

[I02] 提取所有匹配
来源：http://un.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://qv.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nv.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ce.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://wu.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bm.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uc.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://aw.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jq.shxzukj.cn

[I03] 提取捕获分组
来源：http://io.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qi.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wc.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ji.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ov.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yb.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hg.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dm.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nt.jianghongdianzi.cn

[I04] 正则替换
来源：http://ua.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hc.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ms.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cp.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vi.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bw.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qx.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cm.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sv.gzmigu.cn

[I05] 按正则拆分
来源：http://yw.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jq.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rb.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://zf.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://qv.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://aq.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gz.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://aa.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nc.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gy.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://et.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://py.jianghongdianzi.cn


<!-- 参考信息 -->