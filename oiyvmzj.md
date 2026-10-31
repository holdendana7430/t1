代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://on.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://no.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eh.hnjuh.cn

[F12] CSV 读写
来源：http://ww.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pa.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ju.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rs.chemitech.net.cn

TS:   // 同上
来源：http://yd.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hg.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://je.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ry.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ip.yuexingan06.cn

================================================================================
来源：http://am.yuexingan06.cn

G. 面向对象
来源：http://ru.nicolike.cn

================================================================================
来源：http://fo.521024.cn

[G01] 定义类
来源：http://zu.muxihuayi.cn

Py:   class User: pass
来源：http://hm.nszjky.cn

PHP:  class User {}
来源：http://mk.yuntaijiaju.cn

JS:   class User {}
来源：http://bj.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://jf.muxihuayi.cn

Java: class User {}
来源：http://be.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://oc.haigaiapp.cn

Ruby: class User; end
来源：http://xa.wgjwhj.cn

C#:   class User {}
来源：http://ka.chemitech.net.cn

[G02] 构造函数
来源：http://xy.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://uq.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://aw.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://yc.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://kk.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://je.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://za.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://tt.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://od.colortex.cn

[G03] 实例属性
来源：http://uq.yuexingan06.cn

Py:   self.name = "x"
来源：http://er.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://kr.yuexingan06.cn

JS:   this.name = "x";
来源：http://ax.wgjwhj.cn

TS:   name: string = "x";
来源：http://oi.szxytkj.cn

Java: private String name;
来源：http://cf.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cv.521024.cn

Ruby: @name = "x"
来源：http://ii.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://bn.jianghongdianzi.cn

[G04] 定义方法
来源：http://ov.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://ch.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://av.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://pu.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://pr.lnxyls.cn

Java: String greet() { return name; }
来源：http://qq.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://md.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://ou.521024.cn

C#:   public string Greet() => Name;
来源：http://jx.huixiangedu.cn

[G05] 继承
来源：http://dm.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://jq.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://gp.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://dt.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://wg.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://dq.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yy.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://fk.521024.cn

C#:   class Admin : User {}
来源：http://zy.bookmarksfly.cn

[G06] 重写方法
来源：http://gh.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://yr.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hu.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://yv.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://xi.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://qm.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rj.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://og.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://pz.yuexingan06.cn

[G07] 调用父类方法
来源：http://ki.asd995.cn

Py:   super().greet()
来源：http://md.shxzukj.cn

PHP:  parent::greet();
来源：http://eu.shxzukj.cn

JS:   super.greet();
来源：http://id.haigaiapp.cn

TS:   super.greet();
来源：http://nr.jctech888.com.cn

Java: super.greet();
来源：http://uo.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oq.bjjhwx.cn

Ruby: super
来源：http://zk.nszjky.cn

C#:   base.Greet();
来源：http://ih.9csxet.cn

[G08] 静态方法与属性
来源：http://mz.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jb.9csxet.cn

PHP:  public static function f() {}
来源：http://bm.yuexingan06.cn

JS:   static f() {}
来源：http://kq.bjjhwx.cn

TS:   static f(): void {}
来源：http://rn.szsharing.cn

Java: static void f() {}
来源：http://cz.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hr.hahajie.cn

Ruby: def self.f; end
来源：http://ho.bjjhwx.cn

C#:   public static void F() {}
来源：http://wo.nszjky.cn

[G09] 接口 / 抽象类
来源：http://jb.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://lf.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fb.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pj.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://yu.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://ma.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://ze.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cm.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://qm.asd995.cn

[G10] 访问控制
来源：http://xs.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://dp.huixiangedu.cn

PHP:  public / protected / private
来源：http://iz.hahajie.cn

JS:   #private 字段；其余公开
来源：http://bc.asd995.cn

TS:   public / protected / private
来源：http://uu.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://xf.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tn.shxzskj.cn

Ruby: public / protected / private
来源：http://fj.szsharing.cn

C#:   public / protected / private / internal
来源：http://nh.wgjwhj.cn

[G11] getter / setter
来源：http://zl.newstarts.cn

Py:   @property 与 @x.setter
来源：http://sk.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sp.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://sn.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://bt.nszjky.cn

Java: public String getName() { return name; }
来源：http://dp.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yt.newstarts.cn

Ruby: attr_accessor :name
来源：http://rd.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://zr.huanxung.cn

[G12] 对象转字符串
来源：http://bq.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://zi.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xr.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://up.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://fc.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://yq.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lq.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://zd.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://jy.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://wp.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://mo.jctech888.com.cn

PHP:  $u instanceof User
来源：http://zh.yuexingan06.cn

JS:   u instanceof User
来源：http://wq.jianghongdianzi.cn

TS:   u instanceof User
来源：http://dh.muxihuayi.cn

Java: u instanceof User
来源：http://ke.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oh.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://sj.nicolike.cn

C#:   u is User
来源：http://xa.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://aa.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wx.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://rn.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://em.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://sh.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://vh.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://zl.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bh.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://lp.huixinmuqiang.cn

[G15] 枚举
来源：http://oo.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nk.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sm.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qd.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zi.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://cu.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tw.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://ch.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://he.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://ss.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vo.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://lj.shxzukj.cn

JS:   Object.entries(obj)
来源：http://ko.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://xm.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qu.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kf.szsharing.cn

Ruby: obj.instance_variables
来源：http://jn.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://ij.huixiangedu.cn

================================================================================
来源：http://uq.bookmarksfly.cn

H. 异常与错误处理
来源：http://xi.huixinmuqiang.cn

================================================================================
来源：http://rr.muxihuayi.cn

[H01] try / catch 基础
来源：http://gj.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xz.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eg.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wh.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xs.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fq.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ol.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lf.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dk.szsharing.cn

[H02] finally / ensure 收尾
来源：http://ot.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mf.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mc.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ec.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lv.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zd.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kk.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jh.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://az.wgjwhj.cn

[H03] 主动抛出异常
来源：http://ll.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://il.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ec.521024.cn

JS:   throw new Error("错误信息");
来源：http://vl.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://hr.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lv.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lz.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xg.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wc.colortex.cn

[H04] 自定义异常类型
来源：http://dy.521024.cn

Py:   class MyError(Exception): pass
来源：http://jd.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ye.szsharing.cn

JS:   class MyError extends Error {}
来源：http://nb.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://af.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://mh.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kx.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://fy.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://sv.nszjky.cn

[H05] 捕获特定类型
来源：http://mp.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://de.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://br.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://zm.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ac.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://xt.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tn.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://nz.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fx.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://lt.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://gr.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cx.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mk.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yb.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pl.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eq.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://qe.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://gw.gzmigu.cn

[H07] 断言
来源：http://yz.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://wj.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://lq.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://js.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://oa.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://rj.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zf.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://po.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://ul.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://fe.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ae.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lz.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ow.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kd.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pn.newstarts.cn

Go:   err.Error()
来源：http://sf.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://zo.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://zn.9csxet.cn

[H09] 带错误码的异常
来源：http://hr.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rj.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fr.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yw.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://np.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dc.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yv.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ci.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jz.gzmigu.cn

[H10] 资源自动释放
来源：http://en.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qj.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://va.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eo.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ka.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nh.yuexingan06.cn

Go:   defer f.Close()
来源：http://rn.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pu.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cr.nszjky.cn

================================================================================
来源：http://hv.panjiajie.cn

I. 正则表达式
来源：http://hx.chemitech.net.cn

================================================================================
来源：http://vv.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://tr.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hi.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ly.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://yb.colortex.cn

TS:   /\d+/.test(s)
来源：http://nx.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cw.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tv.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://pf.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kr.nicolike.cn

[I02] 提取所有匹配
来源：http://gk.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://rp.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yt.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ym.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://vw.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ob.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jk.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://dy.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wt.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://vm.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ks.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jt.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bh.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oc.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tv.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uu.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://co.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xt.hnjuh.cn

[I04] 正则替换
来源：http://kp.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tm.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zt.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ek.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bv.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ti.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lb.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mr.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cr.lnxyls.cn

[I05] 按正则拆分
来源：http://ee.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bi.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://le.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://qt.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ae.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://sr.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cq.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lw.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jl.bookmarksfly.cn


<!-- 参考信息 -->