代发 wailian999

Java: class User {}
来源：http://rn.huanxung.cn

Go:   type User struct { Name string }
来源：http://ag.hahajie.cn

Ruby: class User; end
来源：http://ws.shxzukj.cn

C#:   class User {}
来源：http://px.jctech888.com.cn

[G02] 构造函数
来源：http://ce.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://so.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://as.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://vy.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://in.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://qu.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://au.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://hk.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://ee.wgjwhj.cn

[G03] 实例属性
来源：http://ta.521024.cn

Py:   self.name = "x"
来源：http://kt.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://zp.asd995.cn

JS:   this.name = "x";
来源：http://zf.colortex.cn

TS:   name: string = "x";
来源：http://oi.huanxung.cn

Java: private String name;
来源：http://by.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gb.colortex.cn

Ruby: @name = "x"
来源：http://tf.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://dq.nicolike.cn

[G04] 定义方法
来源：http://cm.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://nc.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fu.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://vi.521024.cn

TS:   greet(): string { return this.name; }
来源：http://il.hahajie.cn

Java: String greet() { return name; }
来源：http://ed.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://og.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://rs.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://vf.shtwfgs.cn

[G05] 继承
来源：http://ln.hnjuh.cn

Py:   class Admin(User): pass
来源：http://iy.521024.cn

PHP:  class Admin extends User {}
来源：http://tl.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://zn.gzmigu.cn

TS:   class Admin extends User {}
来源：http://eb.yuexingan06.cn

Java: class Admin extends User {}
来源：http://oi.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ik.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://je.szsharing.cn

C#:   class Admin : User {}
来源：http://fo.hnjuh.cn

[G06] 重写方法
来源：http://sp.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://et.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oy.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://sd.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://fg.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://rt.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qk.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://ji.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://fv.shtwfgs.cn

[G07] 调用父类方法
来源：http://ze.szxytkj.cn

Py:   super().greet()
来源：http://fn.panjiajie.cn

PHP:  parent::greet();
来源：http://rt.chemitech.net.cn

JS:   super.greet();
来源：http://xr.shxzskj.cn

TS:   super.greet();
来源：http://dv.panjiajie.cn

Java: super.greet();
来源：http://fr.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yx.shxzukj.cn

Ruby: super
来源：http://aa.shtwfgs.cn

C#:   base.Greet();
来源：http://is.chemitech.net.cn

[G08] 静态方法与属性
来源：http://rq.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fd.nicolike.cn

PHP:  public static function f() {}
来源：http://si.chemitech.net.cn

JS:   static f() {}
来源：http://wb.gzmigu.cn

TS:   static f(): void {}
来源：http://ih.chemitech.net.cn

Java: static void f() {}
来源：http://fu.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cg.muxihuayi.cn

Ruby: def self.f; end
来源：http://js.huanxung.cn

C#:   public static void F() {}
来源：http://ag.asd995.cn

[G09] 接口 / 抽象类
来源：http://yw.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://tc.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vr.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mn.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://sn.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://pu.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://rk.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://am.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://zv.bookmarksfly.cn

[G10] 访问控制
来源：http://or.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://yv.hnjuh.cn

PHP:  public / protected / private
来源：http://bk.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://pi.newstarts.cn

TS:   public / protected / private
来源：http://uh.asd995.cn

Java: public / protected / private / 默认包级
来源：http://yh.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bx.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://bo.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://yc.lnxyls.cn

[G11] getter / setter
来源：http://yb.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://qc.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nd.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://nt.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://xw.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://jn.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pg.szxytkj.cn

Ruby: attr_accessor :name
来源：http://fp.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://iy.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://gx.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://rg.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://is.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://nd.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://hh.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://fd.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fc.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://dm.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://za.9csxet.cn

[G13] 判断对象类型
来源：http://ao.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://pf.newstarts.cn

PHP:  $u instanceof User
来源：http://ib.nicolike.cn

JS:   u instanceof User
来源：http://du.yuntaijiaju.cn

TS:   u instanceof User
来源：http://tb.asd995.cn

Java: u instanceof User
来源：http://kp.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ps.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://el.shtwfgs.cn

C#:   u is User
来源：http://bb.shtwfgs.cn

[G14] 数据类 / record
来源：http://lh.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hj.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://px.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xu.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://ng.newstarts.cn

Java: record User(String name, int age) {}
来源：http://nd.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://wd.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://py.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://hv.nicolike.cn

[G15] 枚举
来源：http://da.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qd.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://an.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ln.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nc.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://sb.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pj.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://iz.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ud.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://dg.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fp.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://zi.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://wl.521024.cn

TS:   Object.entries(obj)
来源：http://oa.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vy.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mn.gzmigu.cn

Ruby: obj.instance_variables
来源：http://yl.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://es.colortex.cn

================================================================================
来源：http://ri.lnxyls.cn

H. 异常与错误处理
来源：http://du.yuexingan06.cn

================================================================================
来源：http://ur.bjjhwx.cn

[H01] try / catch 基础
来源：http://wk.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ac.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ca.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jb.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iz.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ul.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lt.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://by.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bz.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://hy.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yh.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ls.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rf.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qz.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eh.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xa.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hx.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ep.nszjky.cn

[H03] 主动抛出异常
来源：http://tv.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://cz.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tb.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://lp.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://kl.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jc.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xc.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nl.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cy.colortex.cn

[H04] 自定义异常类型
来源：http://ha.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://br.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dl.colortex.cn

JS:   class MyError extends Error {}
来源：http://sz.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://hh.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://vj.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ia.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://xc.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://iz.chemitech.net.cn

[H05] 捕获特定类型
来源：http://sj.asd995.cn

Py:   except ValueError as e:
来源：http://sc.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cl.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://kt.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://gk.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://kf.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sz.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://my.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lg.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://dr.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://cz.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qn.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dv.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gu.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nu.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://of.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://qd.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://om.nicolike.cn

[H07] 断言
来源：http://fn.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://tw.newstarts.cn

PHP:  assert($x > 0);
来源：http://qv.newstarts.cn

JS:   console.assert(x > 0);
来源：http://vk.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://vc.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://dy.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ob.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://az.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://ec.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://kr.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://um.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://in.newstarts.cn

JS:   e.message;  e.stack
来源：http://eo.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fq.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wd.yuexingan06.cn

Go:   err.Error()
来源：http://vq.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://xg.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://ur.shtwfgs.cn

[H09] 带错误码的异常
来源：http://co.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uq.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kx.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aq.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pr.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tx.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bq.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hp.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kv.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://wu.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://le.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://li.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sr.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pl.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kw.shtwfgs.cn

Go:   defer f.Close()
来源：http://qd.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ek.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ah.haigaiapp.cn

================================================================================
来源：http://lu.huixiangedu.cn

I. 正则表达式
来源：http://fn.szxytkj.cn

================================================================================
来源：http://ot.bjjhwx.cn

[I01] 判断是否匹配
来源：http://vd.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ce.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://bj.newstarts.cn

TS:   /\d+/.test(s)
来源：http://el.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aj.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yx.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://pc.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ze.asd995.cn

[I02] 提取所有匹配
来源：http://jz.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://cb.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ud.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bo.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://fx.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://di.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qw.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://og.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://et.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://pq.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iw.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vw.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zj.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xu.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hl.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ze.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tn.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://il.huanxung.cn

[I04] 正则替换
来源：http://pg.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vc.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zw.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kn.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gd.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://el.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ur.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yu.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xs.haigaiapp.cn

[I05] 按正则拆分
来源：http://qc.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hs.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qn.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://pq.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://ff.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://he.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jy.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pu.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cc.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://km.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xs.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gu.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ca.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ue.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://io.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zy.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sv.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://as.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://gw.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ef.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ak.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sc.newstarts.cn

TS:   /error/gim
来源：http://yi.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://em.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uf.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://tl.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eu.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://lp.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bv.shxzskj.cn


<!-- 参考信息 -->