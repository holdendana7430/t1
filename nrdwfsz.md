代发 wailian999

[G02] 构造函数
来源：http://ju.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://mq.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://rg.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://hy.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://ds.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://uc.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tm.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://rq.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://hf.9csxet.cn

[G03] 实例属性
来源：http://ut.521024.cn

Py:   self.name = "x"
来源：http://oc.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://us.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ej.panjiajie.cn

TS:   name: string = "x";
来源：http://mh.shxzskj.cn

Java: private String name;
来源：http://zt.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://js.bjjhwx.cn

Ruby: @name = "x"
来源：http://oy.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://pz.newstarts.cn

[G04] 定义方法
来源：http://sj.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://ff.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rk.colortex.cn

JS:   greet() { return this.name; }
来源：http://yc.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://bs.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://iq.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://on.hnjuh.cn

Ruby: def greet; @name; end
来源：http://jv.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://tb.newstarts.cn

[G05] 继承
来源：http://ar.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://py.asd995.cn

PHP:  class Admin extends User {}
来源：http://vf.huanxung.cn

JS:   class Admin extends User {}
来源：http://xd.gzmigu.cn

TS:   class Admin extends User {}
来源：http://qk.asd995.cn

Java: class Admin extends User {}
来源：http://ro.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eu.shxzukj.cn

Ruby: class Admin < User; end
来源：http://go.panjiajie.cn

C#:   class Admin : User {}
来源：http://se.shtwfgs.cn

[G06] 重写方法
来源：http://ki.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://qy.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ka.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://yx.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://fw.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://wm.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wg.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://yr.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://xl.shxzukj.cn

[G07] 调用父类方法
来源：http://fa.chemitech.net.cn

Py:   super().greet()
来源：http://ad.huixiangedu.cn

PHP:  parent::greet();
来源：http://to.521024.cn

JS:   super.greet();
来源：http://kq.newstarts.cn

TS:   super.greet();
来源：http://dd.panjiajie.cn

Java: super.greet();
来源：http://ve.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lh.hnjuh.cn

Ruby: super
来源：http://zn.newstarts.cn

C#:   base.Greet();
来源：http://au.asd995.cn

[G08] 静态方法与属性
来源：http://rc.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://id.haigaiapp.cn

PHP:  public static function f() {}
来源：http://pk.asd995.cn

JS:   static f() {}
来源：http://re.panjiajie.cn

TS:   static f(): void {}
来源：http://up.hnjuh.cn

Java: static void f() {}
来源：http://aw.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sb.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://of.szsharing.cn

C#:   public static void F() {}
来源：http://qi.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://dt.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://is.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eq.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zj.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://zd.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://em.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://wu.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lp.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://ui.szxytkj.cn

[G10] 访问控制
来源：http://ml.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://as.wgjwhj.cn

PHP:  public / protected / private
来源：http://ve.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://gh.9csxet.cn

TS:   public / protected / private
来源：http://my.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://hi.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rr.lnxyls.cn

Ruby: public / protected / private
来源：http://fj.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://lj.szsharing.cn

[G11] getter / setter
来源：http://rg.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://uo.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gw.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://so.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://ih.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://ll.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nc.huanxung.cn

Ruby: attr_accessor :name
来源：http://vl.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://rg.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://tu.colortex.cn

Py:   def __str__(self): return self.name
来源：http://sk.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ff.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://qc.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://in.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://gy.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dq.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://zz.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://bt.9csxet.cn

[G13] 判断对象类型
来源：http://jr.hahajie.cn

Py:   isinstance(u, User)
来源：http://qa.chemitech.net.cn

PHP:  $u instanceof User
来源：http://ox.newstarts.cn

JS:   u instanceof User
来源：http://ux.shtwfgs.cn

TS:   u instanceof User
来源：http://dp.huixiangedu.cn

Java: u instanceof User
来源：http://hp.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ud.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://fz.szsharing.cn

C#:   u is User
来源：http://kh.bjjhwx.cn

[G14] 数据类 / record
来源：http://dq.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bs.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ih.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mr.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://vo.nicolike.cn

Java: record User(String name, int age) {}
来源：http://rp.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://su.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xy.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://oz.huixiangedu.cn

[G15] 枚举
来源：http://th.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ks.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wj.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wl.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kv.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://ef.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wu.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://kw.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jv.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://pf.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yn.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://ym.newstarts.cn

JS:   Object.entries(obj)
来源：http://lc.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://dv.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yp.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gb.nszjky.cn

Ruby: obj.instance_variables
来源：http://hu.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://ct.hahajie.cn

================================================================================
来源：http://qn.yuntaijiaju.cn

H. 异常与错误处理
来源：http://gy.szsharing.cn

================================================================================
来源：http://aj.hahajie.cn

[H01] try / catch 基础
来源：http://uk.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gh.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pb.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qs.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sw.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uf.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ss.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wz.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hr.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://bh.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qj.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vu.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rd.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vr.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fg.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gl.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://be.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iw.colortex.cn

[H03] 主动抛出异常
来源：http://im.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://ig.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fm.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://an.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://ay.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mh.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://km.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ql.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fd.nicolike.cn

[H04] 自定义异常类型
来源：http://pm.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://zr.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yz.nicolike.cn

JS:   class MyError extends Error {}
来源：http://uu.9csxet.cn

TS:   class MyError extends Error {}
来源：http://xj.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://gr.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vc.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://td.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://au.haigaiapp.cn

[H05] 捕获特定类型
来源：http://cf.szxytkj.cn

Py:   except ValueError as e:
来源：http://mq.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vr.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://sf.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://jb.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://hj.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://db.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://dj.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yf.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://gq.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://al.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mt.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://km.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ko.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jk.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hd.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://zs.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://cb.jctech888.com.cn

[H07] 断言
来源：http://ka.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://vr.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://yg.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://mj.521024.cn

TS:   console.assert(x > 0);
来源：http://ss.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://mi.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cl.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://or.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://vi.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://nu.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://cx.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gd.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://vn.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ay.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kg.bookmarksfly.cn

Go:   err.Error()
来源：http://js.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://sm.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://vr.jctech888.com.cn

[H09] 带错误码的异常
来源：http://sn.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bm.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gi.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kt.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mm.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fw.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ki.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ix.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cb.bjjhwx.cn

[H10] 资源自动释放
来源：http://wu.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nf.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ic.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zg.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cs.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://th.huanxung.cn

Go:   defer f.Close()
来源：http://uj.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vj.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dj.szxytkj.cn

================================================================================
来源：http://ku.colortex.cn

I. 正则表达式
来源：http://lm.shxzukj.cn

================================================================================
来源：http://ho.bjjhwx.cn

[I01] 判断是否匹配
来源：http://wo.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aw.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fc.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://do.nicolike.cn

TS:   /\d+/.test(s)
来源：http://uu.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nh.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vc.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://cq.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zz.521024.cn

[I02] 提取所有匹配
来源：http://gk.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://pz.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bm.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gs.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://xb.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zh.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yc.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://tp.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wg.hnjuh.cn

[I03] 提取捕获分组
来源：http://ob.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cx.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bc.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://po.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zx.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fg.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://et.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rq.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ky.huixiangedu.cn

[I04] 正则替换
来源：http://qw.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://be.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vd.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cj.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nt.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://he.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ey.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dw.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zs.yuexingan06.cn

[I05] 按正则拆分
来源：http://hk.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ub.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ss.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://jo.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://pb.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://ij.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pq.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rr.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qd.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ia.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ax.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://en.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tq.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mz.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wx.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://el.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ba.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://gl.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vs.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zv.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xa.muxihuayi.cn

TS:   /error/gim
来源：http://jq.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mx.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gi.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://sy.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lc.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://vg.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://he.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ij.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://od.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kr.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uv.huixiangedu.cn


<!-- 参考信息 -->