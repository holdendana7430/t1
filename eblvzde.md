代发 wailian999

Py:   class User: pass
来源：http://qy.huixinmuqiang.cn

PHP:  class User {}
来源：http://do.nszjky.cn

JS:   class User {}
来源：http://sh.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://uw.chemitech.net.cn

Java: class User {}
来源：http://dl.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://rb.yuexingan06.cn

Ruby: class User; end
来源：http://tz.521024.cn

C#:   class User {}
来源：http://tr.chemitech.net.cn

[G02] 构造函数
来源：http://zx.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://hc.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://vf.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://wg.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://ua.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://ch.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sk.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://wh.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://ja.shxzskj.cn

[G03] 实例属性
来源：http://lh.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://qh.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://jj.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://au.hnjuh.cn

TS:   name: string = "x";
来源：http://mq.lnxyls.cn

Java: private String name;
来源：http://hu.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kk.9csxet.cn

Ruby: @name = "x"
来源：http://bk.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ka.huanxung.cn

[G04] 定义方法
来源：http://xt.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://he.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ud.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://kz.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://bo.huanxung.cn

Java: String greet() { return name; }
来源：http://gd.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nc.panjiajie.cn

Ruby: def greet; @name; end
来源：http://wp.asd995.cn

C#:   public string Greet() => Name;
来源：http://bg.wgjwhj.cn

[G05] 继承
来源：http://in.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://nw.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://zd.panjiajie.cn

JS:   class Admin extends User {}
来源：http://gi.gzmigu.cn

TS:   class Admin extends User {}
来源：http://hr.9csxet.cn

Java: class Admin extends User {}
来源：http://sf.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ux.nszjky.cn

Ruby: class Admin < User; end
来源：http://dl.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://io.haigaiapp.cn

[G06] 重写方法
来源：http://ch.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://gp.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bo.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://wc.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://ps.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://as.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bd.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://rh.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://ok.newstarts.cn

[G07] 调用父类方法
来源：http://il.bjjhwx.cn

Py:   super().greet()
来源：http://ap.szxytkj.cn

PHP:  parent::greet();
来源：http://bs.huixiangedu.cn

JS:   super.greet();
来源：http://wj.shtwfgs.cn

TS:   super.greet();
来源：http://xx.panjiajie.cn

Java: super.greet();
来源：http://yl.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cj.colortex.cn

Ruby: super
来源：http://se.521024.cn

C#:   base.Greet();
来源：http://kj.jctech888.com.cn

[G08] 静态方法与属性
来源：http://eu.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ci.shtwfgs.cn

PHP:  public static function f() {}
来源：http://sy.huanxung.cn

JS:   static f() {}
来源：http://tk.yuexingan06.cn

TS:   static f(): void {}
来源：http://vn.huanxung.cn

Java: static void f() {}
来源：http://hf.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yf.huixiangedu.cn

Ruby: def self.f; end
来源：http://lm.lnxyls.cn

C#:   public static void F() {}
来源：http://tx.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://nf.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ux.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wn.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wg.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://dh.huanxung.cn

Java: interface Shape { double area(); }
来源：http://ex.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://ch.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://en.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://rc.wgjwhj.cn

[G10] 访问控制
来源：http://ks.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://uz.asd995.cn

PHP:  public / protected / private
来源：http://ht.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://bq.szsharing.cn

TS:   public / protected / private
来源：http://of.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://fe.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cm.szxytkj.cn

Ruby: public / protected / private
来源：http://ov.panjiajie.cn

C#:   public / protected / private / internal
来源：http://me.chemitech.net.cn

[G11] getter / setter
来源：http://tu.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://hg.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xx.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://bo.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://vz.huanxung.cn

Java: public String getName() { return name; }
来源：http://we.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://og.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://wx.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://us.colortex.cn

[G12] 对象转字符串
来源：http://ei.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://sf.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jy.9csxet.cn

JS:   toString() { return this.name; }
来源：http://vq.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://wc.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://ty.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ju.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://ks.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://yc.haigaiapp.cn

[G13] 判断对象类型
来源：http://xm.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://me.panjiajie.cn

PHP:  $u instanceof User
来源：http://ow.shxzskj.cn

JS:   u instanceof User
来源：http://xl.colortex.cn

TS:   u instanceof User
来源：http://ey.huixiangedu.cn

Java: u instanceof User
来源：http://et.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nz.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://xh.shtwfgs.cn

C#:   u is User
来源：http://nc.shtwfgs.cn

[G14] 数据类 / record
来源：http://tf.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://po.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://eu.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bz.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://wp.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://ht.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://za.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hk.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://ej.jianghongdianzi.cn

[G15] 枚举
来源：http://ev.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pv.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vq.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nv.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yk.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://ug.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://br.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://to.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ux.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://oq.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rb.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://rd.9csxet.cn

JS:   Object.entries(obj)
来源：http://nb.asd995.cn

TS:   Object.entries(obj)
来源：http://ed.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kl.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zr.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://hy.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://fv.nicolike.cn

================================================================================
来源：http://eb.asd995.cn

H. 异常与错误处理
来源：http://jy.szsharing.cn

================================================================================
来源：http://qh.9csxet.cn

[H01] try / catch 基础
来源：http://my.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ky.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iw.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cx.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://af.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uq.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://di.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uh.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gm.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://xr.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lz.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rn.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ed.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pb.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kk.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sz.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nh.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tv.szsharing.cn

[H03] 主动抛出异常
来源：http://zs.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://wt.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jh.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://ug.521024.cn

TS:   throw new Error("错误信息");
来源：http://ii.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jx.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aq.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://no.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ut.wgjwhj.cn

[H04] 自定义异常类型
来源：http://ju.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://hq.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vr.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://au.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://ue.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://cu.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cg.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://eh.nszjky.cn

C#:   class MyException : Exception {}
来源：http://kq.huanxung.cn

[H05] 捕获特定类型
来源：http://wq.shtwfgs.cn

Py:   except ValueError as e:
来源：http://xg.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wu.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://pc.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://td.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://di.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pm.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://wv.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xm.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://cn.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://vy.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://om.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://it.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://it.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aj.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cm.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://fn.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://id.huixiangedu.cn

[H07] 断言
来源：http://yl.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://yl.hnjuh.cn

PHP:  assert($x > 0);
来源：http://fl.hahajie.cn

JS:   console.assert(x > 0);
来源：http://cz.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://pp.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://kd.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://db.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oq.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://rj.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://no.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://mc.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yr.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://oo.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ny.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qb.yuntaijiaju.cn

Go:   err.Error()
来源：http://gk.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://fk.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://rc.hnjuh.cn

[H09] 带错误码的异常
来源：http://xf.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vz.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pj.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zc.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xj.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://js.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mk.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ay.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lc.jctech888.com.cn

[H10] 资源自动释放
来源：http://ni.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jn.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ge.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bl.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pk.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://te.shxzukj.cn

Go:   defer f.Close()
来源：http://zs.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uw.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jx.huanxung.cn

================================================================================
来源：http://zf.asd995.cn

I. 正则表达式
来源：http://ob.muxihuayi.cn

================================================================================
来源：http://ic.nicolike.cn

[I01] 判断是否匹配
来源：http://xv.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://co.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qn.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://pp.521024.cn

TS:   /\d+/.test(s)
来源：http://ab.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hp.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yg.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://vc.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mk.jctech888.com.cn

[I02] 提取所有匹配
来源：http://uu.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://se.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ip.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jn.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://as.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tw.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qa.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://qh.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cm.huanxung.cn

[I03] 提取捕获分组
来源：http://wa.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ue.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sp.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uh.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dn.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ub.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://al.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bo.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gk.muxihuayi.cn

[I04] 正则替换
来源：http://gh.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cz.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ro.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eq.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fi.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lt.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cx.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mh.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ka.muxihuayi.cn

[I05] 按正则拆分
来源：http://nl.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nm.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nf.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://fx.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://fn.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://ln.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qe.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://om.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yd.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gf.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dr.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xh.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fp.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://co.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eo.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fz.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ot.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qp.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://vh.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qq.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zz.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iw.9csxet.cn

TS:   /error/gim
来源：http://ls.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vi.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ds.muxihuayi.cn


<!-- 参考信息 -->