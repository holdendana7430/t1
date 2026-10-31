代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fc.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ma.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yo.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://li.yuexingan06.cn

================================================================================
来源：http://vp.nszjky.cn

G. 面向对象
来源：http://ea.asd995.cn

================================================================================
来源：http://os.yuexingan06.cn

[G01] 定义类
来源：http://yv.wgjwhj.cn

Py:   class User: pass
来源：http://gu.bookmarksfly.cn

PHP:  class User {}
来源：http://lx.9csxet.cn

JS:   class User {}
来源：http://cg.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://ad.yuexingan06.cn

Java: class User {}
来源：http://kp.szxytkj.cn

Go:   type User struct { Name string }
来源：http://fc.521024.cn

Ruby: class User; end
来源：http://mq.521024.cn

C#:   class User {}
来源：http://rt.yuntaijiaju.cn

[G02] 构造函数
来源：http://ng.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://cg.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://cs.chemitech.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://zz.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://zl.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://mm.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hl.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://mb.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://lz.yuntaijiaju.cn

[G03] 实例属性
来源：http://cd.nszjky.cn

Py:   self.name = "x"
来源：http://on.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://cd.haigaiapp.cn

JS:   this.name = "x";
来源：http://jx.gzmigu.cn

TS:   name: string = "x";
来源：http://ch.shxzukj.cn

Java: private String name;
来源：http://ux.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ne.gzmigu.cn

Ruby: @name = "x"
来源：http://hv.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://tk.shxzskj.cn

[G04] 定义方法
来源：http://mj.9csxet.cn

Py:   def greet(self): return self.name
来源：http://jt.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://az.huanxung.cn

JS:   greet() { return this.name; }
来源：http://oh.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://zn.huixiangedu.cn

Java: String greet() { return name; }
来源：http://rs.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gp.panjiajie.cn

Ruby: def greet; @name; end
来源：http://xk.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://sj.colortex.cn

[G05] 继承
来源：http://oh.panjiajie.cn

Py:   class Admin(User): pass
来源：http://ex.nicolike.cn

PHP:  class Admin extends User {}
来源：http://wq.hahajie.cn

JS:   class Admin extends User {}
来源：http://wy.hahajie.cn

TS:   class Admin extends User {}
来源：http://un.shxzukj.cn

Java: class Admin extends User {}
来源：http://bm.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hu.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://hy.hahajie.cn

C#:   class Admin : User {}
来源：http://tv.jianghongdianzi.cn

[G06] 重写方法
来源：http://ae.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://js.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yd.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://pp.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://hj.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://ka.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://in.colortex.cn

Ruby: def greet; "admin"; end
来源：http://ue.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://hx.521024.cn

[G07] 调用父类方法
来源：http://cv.muxihuayi.cn

Py:   super().greet()
来源：http://mm.hnjuh.cn

PHP:  parent::greet();
来源：http://do.nszjky.cn

JS:   super.greet();
来源：http://fv.yuntaijiaju.cn

TS:   super.greet();
来源：http://gb.shtwfgs.cn

Java: super.greet();
来源：http://az.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kp.hnjuh.cn

Ruby: super
来源：http://gl.muxihuayi.cn

C#:   base.Greet();
来源：http://jk.jctech888.com.cn

[G08] 静态方法与属性
来源：http://zu.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gn.9csxet.cn

PHP:  public static function f() {}
来源：http://af.hahajie.cn

JS:   static f() {}
来源：http://mx.521024.cn

TS:   static f(): void {}
来源：http://pq.wgjwhj.cn

Java: static void f() {}
来源：http://wf.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vv.gzmigu.cn

Ruby: def self.f; end
来源：http://xh.muxihuayi.cn

C#:   public static void F() {}
来源：http://id.nicolike.cn

[G09] 接口 / 抽象类
来源：http://pt.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://tx.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ch.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wh.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://tr.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://pl.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://vu.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yg.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://ws.shxzukj.cn

[G10] 访问控制
来源：http://ck.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ej.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://ju.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://rx.huixinmuqiang.cn

TS:   public / protected / private
来源：http://jh.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://ir.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://od.nicolike.cn

Ruby: public / protected / private
来源：http://tm.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://tf.asd995.cn

[G11] getter / setter
来源：http://gw.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://kz.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://it.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://sr.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://xd.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://rq.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ii.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://ws.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://xs.shxzskj.cn

[G12] 对象转字符串
来源：http://yx.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://zc.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ch.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://mq.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://bk.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://np.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gu.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://hi.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://sh.jctech888.com.cn

[G13] 判断对象类型
来源：http://jz.gzmigu.cn

Py:   isinstance(u, User)
来源：http://jn.nicolike.cn

PHP:  $u instanceof User
来源：http://py.9csxet.cn

JS:   u instanceof User
来源：http://fd.521024.cn

TS:   u instanceof User
来源：http://zm.haigaiapp.cn

Java: u instanceof User
来源：http://in.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cf.hahajie.cn

Ruby: u.is_a?(User)
来源：http://am.gzmigu.cn

C#:   u is User
来源：http://em.nszjky.cn

[G14] 数据类 / record
来源：http://ff.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zg.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://qh.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pt.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://yn.hahajie.cn

Java: record User(String name, int age) {}
来源：http://ji.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://km.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ob.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://kj.haigaiapp.cn

[G15] 枚举
来源：http://xj.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gk.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tw.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kg.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://df.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://oo.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dz.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://gn.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fp.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://ir.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://my.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://fe.nszjky.cn

JS:   Object.entries(obj)
来源：http://vf.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://rm.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wq.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://en.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://qi.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://bo.wgjwhj.cn

================================================================================
来源：http://dp.muxihuayi.cn

H. 异常与错误处理
来源：http://pz.huixinmuqiang.cn

================================================================================
来源：http://lw.gzmigu.cn

[H01] try / catch 基础
来源：http://me.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dk.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wl.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hf.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zx.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tv.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gv.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pb.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://os.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://fy.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nh.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mn.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ct.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hi.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zf.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://de.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bk.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hs.nicolike.cn

[H03] 主动抛出异常
来源：http://hb.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://hz.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uq.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://dk.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://iz.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xe.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mv.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xo.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kg.hahajie.cn

[H04] 自定义异常类型
来源：http://vt.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://td.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gn.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://uc.huanxung.cn

TS:   class MyError extends Error {}
来源：http://xh.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://hh.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ph.521024.cn

Ruby: class MyError < StandardError; end
来源：http://gg.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://rc.szxytkj.cn

[H05] 捕获特定类型
来源：http://ba.muxihuayi.cn

Py:   except ValueError as e:
来源：http://kx.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ff.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://dz.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://hy.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://yv.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ww.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://ob.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ug.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://nf.colortex.cn

Py:   value = d.get("k") or default
来源：http://gr.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oz.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rt.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mf.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sm.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://by.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://wm.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://vo.shxzukj.cn

[H07] 断言
来源：http://ps.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://rp.shxzskj.cn

PHP:  assert($x > 0);
来源：http://gb.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://ti.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://ml.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://of.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mw.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://it.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://nc.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://fr.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://qz.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ha.nicolike.cn

JS:   e.message;  e.stack
来源：http://qs.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zy.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hk.szxytkj.cn

Go:   err.Error()
来源：http://tq.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://oc.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://mp.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://rl.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cc.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qv.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gv.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ti.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fu.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://io.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://at.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pd.521024.cn

[H10] 资源自动释放
来源：http://zq.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xp.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xb.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bi.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bh.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://am.panjiajie.cn

Go:   defer f.Close()
来源：http://si.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ti.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yh.lnxyls.cn

================================================================================
来源：http://oy.gzmigu.cn

I. 正则表达式
来源：http://fo.bookmarksfly.cn

================================================================================
来源：http://zy.bjjhwx.cn

[I01] 判断是否匹配
来源：http://db.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ge.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ku.szsharing.cn

JS:   /\d+/.test(s)
来源：http://wz.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://mg.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gp.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ip.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://gd.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://na.shxzukj.cn

[I02] 提取所有匹配
来源：http://ge.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://es.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jd.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vi.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://sp.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://te.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oy.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://yd.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oh.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://lv.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ql.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://or.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sb.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uw.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yr.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uv.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tb.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lq.hnjuh.cn

[I04] 正则替换
来源：http://ii.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://la.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nz.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sh.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zf.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://do.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pb.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zx.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tk.wgjwhj.cn

[I05] 按正则拆分
来源：http://gm.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yg.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ew.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://wz.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://cb.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://vu.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ym.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vq.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://if.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wr.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vk.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gp.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jz.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gj.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://px.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yu.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bq.nicolike.cn


<!-- 参考信息 -->