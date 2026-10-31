代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kg.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ev.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ch.muxihuayi.cn

TS:   // 同上
来源：http://di.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tl.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://si.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mi.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://eb.yuexingan06.cn

================================================================================
来源：http://vc.shtwfgs.cn

G. 面向对象
来源：http://uv.panjiajie.cn

================================================================================
来源：http://nm.yuexingan06.cn

[G01] 定义类
来源：http://zx.muxihuayi.cn

Py:   class User: pass
来源：http://rh.nszjky.cn

PHP:  class User {}
来源：http://zh.wgjwhj.cn

JS:   class User {}
来源：http://ao.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://qt.wgjwhj.cn

Java: class User {}
来源：http://ml.asd995.cn

Go:   type User struct { Name string }
来源：http://mo.521024.cn

Ruby: class User; end
来源：http://qu.haigaiapp.cn

C#:   class User {}
来源：http://rs.nicolike.cn

[G02] 构造函数
来源：http://an.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://qn.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ll.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://el.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://vn.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://as.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nv.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://na.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://gt.yuexingan06.cn

[G03] 实例属性
来源：http://lq.huanxung.cn

Py:   self.name = "x"
来源：http://zr.hnjuh.cn

PHP:  public string $name = "x";
来源：http://cq.haigaiapp.cn

JS:   this.name = "x";
来源：http://wy.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://ri.huanxung.cn

Java: private String name;
来源：http://yh.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kk.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://vn.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://dt.newstarts.cn

[G04] 定义方法
来源：http://hv.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://ut.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ls.9csxet.cn

JS:   greet() { return this.name; }
来源：http://qs.gzmigu.cn

TS:   greet(): string { return this.name; }
来源：http://rv.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://ec.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tf.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://ku.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://ps.nicolike.cn

[G05] 继承
来源：http://rc.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://be.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://zm.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://jr.huanxung.cn

TS:   class Admin extends User {}
来源：http://mi.chemitech.net.cn

Java: class Admin extends User {}
来源：http://vd.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yt.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://cq.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://ae.colortex.cn

[G06] 重写方法
来源：http://xa.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://ov.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kp.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://ms.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://qi.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://tz.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://of.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://cl.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ca.panjiajie.cn

[G07] 调用父类方法
来源：http://fr.wgjwhj.cn

Py:   super().greet()
来源：http://sg.bookmarksfly.cn

PHP:  parent::greet();
来源：http://nx.hnjuh.cn

JS:   super.greet();
来源：http://pq.bookmarksfly.cn

TS:   super.greet();
来源：http://ef.asd995.cn

Java: super.greet();
来源：http://se.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://co.shxzukj.cn

Ruby: super
来源：http://mu.gzmigu.cn

C#:   base.Greet();
来源：http://ah.muxihuayi.cn

[G08] 静态方法与属性
来源：http://zk.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vd.nicolike.cn

PHP:  public static function f() {}
来源：http://kw.hahajie.cn

JS:   static f() {}
来源：http://na.shtwfgs.cn

TS:   static f(): void {}
来源：http://zt.yuexingan06.cn

Java: static void f() {}
来源：http://km.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xq.hnjuh.cn

Ruby: def self.f; end
来源：http://ug.colortex.cn

C#:   public static void F() {}
来源：http://le.asd995.cn

[G09] 接口 / 抽象类
来源：http://et.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://dj.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sc.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jk.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://zo.asd995.cn

Java: interface Shape { double area(); }
来源：http://qi.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://rj.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wh.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://tl.szxytkj.cn

[G10] 访问控制
来源：http://wd.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://zm.hnjuh.cn

PHP:  public / protected / private
来源：http://uo.hahajie.cn

JS:   #private 字段；其余公开
来源：http://wb.jctech888.com.cn

TS:   public / protected / private
来源：http://bv.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://dk.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ck.asd995.cn

Ruby: public / protected / private
来源：http://vk.shxzskj.cn

C#:   public / protected / private / internal
来源：http://fq.yuntaijiaju.cn

[G11] getter / setter
来源：http://bp.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://cw.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ja.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://oo.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://jp.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://as.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dj.hnjuh.cn

Ruby: attr_accessor :name
来源：http://lh.huanxung.cn

C#:   public string Name { get; set; }
来源：http://hc.nszjky.cn

[G12] 对象转字符串
来源：http://ps.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://yx.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ze.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://ax.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://xh.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://qi.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gd.newstarts.cn

Ruby: def to_s; @name; end
来源：http://fp.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://oq.jctech888.com.cn

[G13] 判断对象类型
来源：http://rf.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://yc.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://im.jctech888.com.cn

JS:   u instanceof User
来源：http://ge.jctech888.com.cn

TS:   u instanceof User
来源：http://wc.hahajie.cn

Java: u instanceof User
来源：http://vc.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ub.nicolike.cn

Ruby: u.is_a?(User)
来源：http://po.521024.cn

C#:   u is User
来源：http://hb.huanxung.cn

[G14] 数据类 / record
来源：http://hx.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://za.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://bi.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pc.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://sh.nszjky.cn

Java: record User(String name, int age) {}
来源：http://ph.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://hl.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ih.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://jb.jctech888.com.cn

[G15] 枚举
来源：http://ny.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sj.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ir.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ys.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iy.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://un.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vh.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://qn.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hu.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://fx.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yy.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://rk.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://ub.newstarts.cn

TS:   Object.entries(obj)
来源：http://yo.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qb.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vl.newstarts.cn

Ruby: obj.instance_variables
来源：http://dz.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://vz.szxytkj.cn

================================================================================
来源：http://kz.huixiangedu.cn

H. 异常与错误处理
来源：http://go.9csxet.cn

================================================================================
来源：http://sj.gzmigu.cn

[H01] try / catch 基础
来源：http://pp.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mr.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vh.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ig.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gw.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vj.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gv.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zb.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vg.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://tx.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pr.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kh.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://or.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ql.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fv.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bj.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bm.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vk.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://aj.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://cj.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qt.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://ub.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://dh.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wq.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://et.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ky.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://os.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://xv.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://wq.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sx.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://am.nicolike.cn

TS:   class MyError extends Error {}
来源：http://pd.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://te.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lr.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://ft.szsharing.cn

C#:   class MyException : Exception {}
来源：http://vw.huixiangedu.cn

[H05] 捕获特定类型
来源：http://ac.haigaiapp.cn

Py:   except ValueError as e:
来源：http://iq.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dl.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://yg.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://ui.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://oa.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gw.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://yf.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ah.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://sx.9csxet.cn

Py:   value = d.get("k") or default
来源：http://qv.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nc.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ut.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oa.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jn.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vx.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://jz.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://mn.nszjky.cn

[H07] 断言
来源：http://gk.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://jy.nszjky.cn

PHP:  assert($x > 0);
来源：http://ux.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://ww.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://ep.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://wl.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oa.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://en.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://cl.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://ff.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://eu.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://na.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://am.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mv.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://my.521024.cn

Go:   err.Error()
来源：http://rj.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://dd.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://ss.521024.cn

[H09] 带错误码的异常
来源：http://ce.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pm.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qr.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kg.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rc.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lu.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xs.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://va.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ar.haigaiapp.cn

[H10] 资源自动释放
来源：http://wz.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vd.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zr.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qm.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dl.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jz.newstarts.cn

Go:   defer f.Close()
来源：http://ga.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://on.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://py.muxihuayi.cn

================================================================================
来源：http://ul.jctech888.com.cn

I. 正则表达式
来源：http://dm.wgjwhj.cn

================================================================================
来源：http://wt.muxihuayi.cn

[I01] 判断是否匹配
来源：http://kq.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kx.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wl.521024.cn

JS:   /\d+/.test(s)
来源：http://fn.szsharing.cn

TS:   /\d+/.test(s)
来源：http://mn.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ki.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dc.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://ye.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://it.huanxung.cn

[I02] 提取所有匹配
来源：http://bb.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://nb.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jg.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gz.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://wx.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://je.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ra.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://va.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jg.huanxung.cn

[I03] 提取捕获分组
来源：http://mb.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wd.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qc.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ri.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vk.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ms.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rm.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uf.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zn.yuntaijiaju.cn

[I04] 正则替换
来源：http://rj.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gn.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rk.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yf.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zo.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jz.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zg.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nu.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fg.panjiajie.cn

[I05] 按正则拆分
来源：http://ti.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ad.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jn.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://jr.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://zl.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://mw.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://te.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zc.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://le.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ol.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tm.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pz.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ir.panjiajie.cn


<!-- 参考信息 -->