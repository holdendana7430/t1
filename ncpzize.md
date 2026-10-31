代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yf.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sw.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ff.lnxyls.cn

TS:   // 同上
来源：http://uc.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ow.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://in.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tk.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ik.yuntaijiaju.cn

================================================================================
来源：http://ub.jctech888.com.cn

G. 面向对象
来源：http://vp.shxzukj.cn

================================================================================
来源：http://jf.newstarts.cn

[G01] 定义类
来源：http://kq.bjjhwx.cn

Py:   class User: pass
来源：http://jn.521024.cn

PHP:  class User {}
来源：http://pq.colortex.cn

JS:   class User {}
来源：http://pn.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://nx.chemitech.net.cn

Java: class User {}
来源：http://gc.nicolike.cn

Go:   type User struct { Name string }
来源：http://xl.shxzskj.cn

Ruby: class User; end
来源：http://el.hahajie.cn

C#:   class User {}
来源：http://id.9csxet.cn

[G02] 构造函数
来源：http://bf.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://lq.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://xn.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://sn.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://fs.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://ab.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jj.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ea.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://nv.chemitech.net.cn

[G03] 实例属性
来源：http://on.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://la.asd995.cn

PHP:  public string $name = "x";
来源：http://gr.yuexingan06.cn

JS:   this.name = "x";
来源：http://oe.jctech888.com.cn

TS:   name: string = "x";
来源：http://dh.haigaiapp.cn

Java: private String name;
来源：http://mc.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://la.9csxet.cn

Ruby: @name = "x"
来源：http://fv.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://mo.chemitech.net.cn

[G04] 定义方法
来源：http://am.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://vi.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mj.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://tf.521024.cn

TS:   greet(): string { return this.name; }
来源：http://rz.9csxet.cn

Java: String greet() { return name; }
来源：http://tm.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yx.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://ub.huanxung.cn

C#:   public string Greet() => Name;
来源：http://hv.szxytkj.cn

[G05] 继承
来源：http://kd.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://lc.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://on.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://nl.521024.cn

TS:   class Admin extends User {}
来源：http://ws.shxzskj.cn

Java: class Admin extends User {}
来源：http://hc.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qz.szsharing.cn

Ruby: class Admin < User; end
来源：http://zy.asd995.cn

C#:   class Admin : User {}
来源：http://ww.haigaiapp.cn

[G06] 重写方法
来源：http://pn.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://fn.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ne.colortex.cn

JS:   greet() { return "admin"; }
来源：http://mh.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://fi.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://os.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xt.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://dt.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://sx.shtwfgs.cn

[G07] 调用父类方法
来源：http://fx.lnxyls.cn

Py:   super().greet()
来源：http://wk.yuexingan06.cn

PHP:  parent::greet();
来源：http://jk.nszjky.cn

JS:   super.greet();
来源：http://gu.asd995.cn

TS:   super.greet();
来源：http://le.jctech888.com.cn

Java: super.greet();
来源：http://op.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iv.panjiajie.cn

Ruby: super
来源：http://fp.shxzukj.cn

C#:   base.Greet();
来源：http://ja.szsharing.cn

[G08] 静态方法与属性
来源：http://lq.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cz.huixiangedu.cn

PHP:  public static function f() {}
来源：http://og.521024.cn

JS:   static f() {}
来源：http://cf.huixiangedu.cn

TS:   static f(): void {}
来源：http://fi.hnjuh.cn

Java: static void f() {}
来源：http://ib.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://df.colortex.cn

Ruby: def self.f; end
来源：http://vl.bookmarksfly.cn

C#:   public static void F() {}
来源：http://dy.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://lc.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://ey.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://el.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ki.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://og.9csxet.cn

Java: interface Shape { double area(); }
来源：http://os.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://bd.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ca.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://oa.szxytkj.cn

[G10] 访问控制
来源：http://va.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://xi.newstarts.cn

PHP:  public / protected / private
来源：http://wo.colortex.cn

JS:   #private 字段；其余公开
来源：http://zc.bjjhwx.cn

TS:   public / protected / private
来源：http://lw.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://dt.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mi.colortex.cn

Ruby: public / protected / private
来源：http://or.lnxyls.cn

C#:   public / protected / private / internal
来源：http://uf.szsharing.cn

[G11] getter / setter
来源：http://hr.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://cx.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xq.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://vf.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://ah.shxzukj.cn

Java: public String getName() { return name; }
来源：http://yn.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yy.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://ks.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://ha.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://xv.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://sm.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tb.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://zk.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://on.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://ns.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oo.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://fj.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://uy.chemitech.net.cn

[G13] 判断对象类型
来源：http://fm.nicolike.cn

Py:   isinstance(u, User)
来源：http://qv.521024.cn

PHP:  $u instanceof User
来源：http://qg.hahajie.cn

JS:   u instanceof User
来源：http://py.panjiajie.cn

TS:   u instanceof User
来源：http://yn.panjiajie.cn

Java: u instanceof User
来源：http://ps.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zp.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://nr.shxzskj.cn

C#:   u is User
来源：http://jg.lnxyls.cn

[G14] 数据类 / record
来源：http://gz.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://li.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://or.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gd.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://up.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://py.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://zc.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tm.asd995.cn

C#:   record User(string Name, int Age);
来源：http://ig.newstarts.cn

[G15] 枚举
来源：http://xa.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ii.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://au.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zu.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dt.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://va.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pp.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://df.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ai.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://uf.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ve.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://wb.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://ue.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ps.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ax.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dp.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://tv.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://zp.panjiajie.cn

================================================================================
来源：http://ns.nicolike.cn

H. 异常与错误处理
来源：http://xy.newstarts.cn

================================================================================
来源：http://cg.bjjhwx.cn

[H01] try / catch 基础
来源：http://vb.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://un.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tw.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pc.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oc.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kt.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yn.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ld.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pq.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://ey.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eb.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://li.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uy.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ho.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jp.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oc.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gs.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ka.szxytkj.cn

[H03] 主动抛出异常
来源：http://tx.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://hp.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tn.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://sm.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://hh.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yl.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://da.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cv.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://le.9csxet.cn

[H04] 自定义异常类型
来源：http://qp.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://zm.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dx.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://az.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://jv.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://qd.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://go.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://tr.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://jj.huixiangedu.cn

[H05] 捕获特定类型
来源：http://yq.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://nt.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://br.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://lh.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://rr.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://ek.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pn.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://nk.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://os.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://hm.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://ti.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://en.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vo.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rf.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bt.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oh.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://fe.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://wz.huixiangedu.cn

[H07] 断言
来源：http://jl.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://hn.hahajie.cn

PHP:  assert($x > 0);
来源：http://ih.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://wd.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://gd.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://or.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bb.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bd.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://wh.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://kv.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://bs.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ze.gzmigu.cn

JS:   e.message;  e.stack
来源：http://df.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yb.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pe.nicolike.cn

Go:   err.Error()
来源：http://ob.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://wy.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://dl.szxytkj.cn

[H09] 带错误码的异常
来源：http://oe.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wp.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yc.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cw.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wh.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oy.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cz.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mh.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://or.bookmarksfly.cn

[H10] 资源自动释放
来源：http://ld.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hs.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xk.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rg.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dy.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.szxytkj.cn

Go:   defer f.Close()
来源：http://bj.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dz.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pb.haigaiapp.cn

================================================================================
来源：http://cg.jianghongdianzi.cn

I. 正则表达式
来源：http://mv.hnjuh.cn

================================================================================
来源：http://op.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://sg.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ls.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cg.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://sj.szsharing.cn

TS:   /\d+/.test(s)
来源：http://ux.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cf.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://do.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://wf.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yp.muxihuayi.cn

[I02] 提取所有匹配
来源：http://jk.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://hc.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wj.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bk.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://az.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qb.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vc.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://ut.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fi.szsharing.cn

[I03] 提取捕获分组
来源：http://zm.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xe.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zb.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nd.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hc.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lm.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://un.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://at.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iy.szsharing.cn

[I04] 正则替换
来源：http://jm.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zm.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rk.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bc.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mp.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tv.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zg.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wq.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ej.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://kj.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ux.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kn.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://vb.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://mx.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://ou.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xw.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://va.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mm.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rq.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qr.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xi.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://el.shtwfgs.cn


<!-- 参考信息 -->