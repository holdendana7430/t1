代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://og.9csxet.cn

[G03] 实例属性
来源：http://js.hnjuh.cn

Py:   self.name = "x"
来源：http://qj.521024.cn

PHP:  public string $name = "x";
来源：http://bw.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://hd.szxytkj.cn

TS:   name: string = "x";
来源：http://kb.chemitech.net.cn

Java: private String name;
来源：http://ho.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vb.huanxung.cn

Ruby: @name = "x"
来源：http://ku.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://oz.yuexingan06.cn

[G04] 定义方法
来源：http://kj.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://kp.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fa.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://tq.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://ir.huanxung.cn

Java: String greet() { return name; }
来源：http://lo.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iq.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://dr.521024.cn

C#:   public string Greet() => Name;
来源：http://qz.hahajie.cn

[G05] 继承
来源：http://vt.asd995.cn

Py:   class Admin(User): pass
来源：http://je.521024.cn

PHP:  class Admin extends User {}
来源：http://ly.szxytkj.cn

JS:   class Admin extends User {}
来源：http://xp.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://rs.gzmigu.cn

Java: class Admin extends User {}
来源：http://oy.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ak.hnjuh.cn

Ruby: class Admin < User; end
来源：http://qn.hahajie.cn

C#:   class Admin : User {}
来源：http://gz.szsharing.cn

[G06] 重写方法
来源：http://jz.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://xg.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uv.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://ly.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://kv.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://el.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hd.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://ly.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://wr.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://pj.huanxung.cn

Py:   super().greet()
来源：http://qn.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://qs.szxytkj.cn

JS:   super.greet();
来源：http://ts.nszjky.cn

TS:   super.greet();
来源：http://at.colortex.cn

Java: super.greet();
来源：http://mp.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kx.lnxyls.cn

Ruby: super
来源：http://wy.hnjuh.cn

C#:   base.Greet();
来源：http://mv.shxzskj.cn

[G08] 静态方法与属性
来源：http://iu.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ob.asd995.cn

PHP:  public static function f() {}
来源：http://zt.muxihuayi.cn

JS:   static f() {}
来源：http://uc.szxytkj.cn

TS:   static f(): void {}
来源：http://fg.shxzskj.cn

Java: static void f() {}
来源：http://kt.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ah.shxzskj.cn

Ruby: def self.f; end
来源：http://vr.yuexingan06.cn

C#:   public static void F() {}
来源：http://ex.nszjky.cn

[G09] 接口 / 抽象类
来源：http://gi.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://zy.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xm.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ll.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://cd.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://ob.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://fc.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vk.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://sz.yuntaijiaju.cn

[G10] 访问控制
来源：http://cl.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://pi.huanxung.cn

PHP:  public / protected / private
来源：http://wx.asd995.cn

JS:   #private 字段；其余公开
来源：http://to.yuexingan06.cn

TS:   public / protected / private
来源：http://gk.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://ml.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xm.gzmigu.cn

Ruby: public / protected / private
来源：http://hq.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://pt.9csxet.cn

[G11] getter / setter
来源：http://eg.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://pi.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ot.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://ds.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://cq.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://sg.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fo.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://pk.nszjky.cn

C#:   public string Name { get; set; }
来源：http://lc.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://vu.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://ag.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ku.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://eh.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://nn.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://hb.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ic.nicolike.cn

Ruby: def to_s; @name; end
来源：http://mh.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://xm.nicolike.cn

[G13] 判断对象类型
来源：http://ag.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://ov.9csxet.cn

PHP:  $u instanceof User
来源：http://mt.521024.cn

JS:   u instanceof User
来源：http://qw.huanxung.cn

TS:   u instanceof User
来源：http://tb.bookmarksfly.cn

Java: u instanceof User
来源：http://ju.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fi.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://ee.lnxyls.cn

C#:   u is User
来源：http://ub.colortex.cn

[G14] 数据类 / record
来源：http://qr.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nc.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://fd.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hu.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://ru.nicolike.cn

Java: record User(String name, int age) {}
来源：http://sc.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://wv.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nw.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://hp.shxzskj.cn

[G15] 枚举
来源：http://dj.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sz.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kk.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lr.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bz.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://gy.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://so.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://up.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wx.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://fr.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lz.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://bh.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://hq.shxzskj.cn

TS:   Object.entries(obj)
来源：http://qe.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rt.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hu.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://zj.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://sl.huixinmuqiang.cn

================================================================================
来源：http://zj.newstarts.cn

H. 异常与错误处理
来源：http://zx.yuexingan06.cn

================================================================================
来源：http://db.huanxung.cn

[H01] try / catch 基础
来源：http://yw.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ev.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vp.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hv.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ys.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oc.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dv.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sp.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ma.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://vk.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ej.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gn.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iq.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ck.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://en.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fc.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pq.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cc.nicolike.cn

[H03] 主动抛出异常
来源：http://ay.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://qh.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fi.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://ad.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://rj.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rl.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vw.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tz.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pw.colortex.cn

[H04] 自定义异常类型
来源：http://mq.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://dg.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dn.huanxung.cn

JS:   class MyError extends Error {}
来源：http://ws.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://eq.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://as.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sh.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://cw.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://cn.haigaiapp.cn

[H05] 捕获特定类型
来源：http://yr.lnxyls.cn

Py:   except ValueError as e:
来源：http://qr.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bx.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://py.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://qf.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://uz.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ah.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://bg.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://in.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://id.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://cy.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hq.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ie.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sb.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uc.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zp.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://zm.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://ae.colortex.cn

[H07] 断言
来源：http://st.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://ck.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://rj.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://xh.521024.cn

TS:   console.assert(x > 0);
来源：http://se.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://uc.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eo.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dt.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://sl.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://at.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://fv.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oj.newstarts.cn

JS:   e.message;  e.stack
来源：http://wx.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mj.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wf.newstarts.cn

Go:   err.Error()
来源：http://lz.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://kw.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://iy.bjjhwx.cn

[H09] 带错误码的异常
来源：http://fp.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hx.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cr.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kn.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xn.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://je.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bq.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ky.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vp.chemitech.net.cn

[H10] 资源自动释放
来源：http://qe.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sq.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uv.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://if.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ne.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://he.muxihuayi.cn

Go:   defer f.Close()
来源：http://qo.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ev.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bu.shxzukj.cn

================================================================================
来源：http://ul.haigaiapp.cn

I. 正则表达式
来源：http://eq.colortex.cn

================================================================================
来源：http://nw.colortex.cn

[I01] 判断是否匹配
来源：http://nq.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bl.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pj.asd995.cn

JS:   /\d+/.test(s)
来源：http://pv.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://bl.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ha.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qg.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://fy.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cn.muxihuayi.cn

[I02] 提取所有匹配
来源：http://sk.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://ts.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ar.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mp.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://bb.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vu.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ys.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://uk.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://if.huixiangedu.cn

[I03] 提取捕获分组
来源：http://nr.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://az.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://of.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vp.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ta.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cq.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bo.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ae.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oy.jianghongdianzi.cn

[I04] 正则替换
来源：http://yp.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ov.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nt.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qo.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nh.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gj.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pb.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gd.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mp.haigaiapp.cn

[I05] 按正则拆分
来源：http://wj.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cs.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qj.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://ad.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ym.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://oh.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yk.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wg.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nc.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wv.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zc.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nt.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hk.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qq.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hx.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://js.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gx.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ef.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://bt.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lc.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kr.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ii.shxzskj.cn

TS:   /error/gim
来源：http://qf.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zg.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qb.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://hs.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zn.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://nn.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jc.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jm.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yt.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vd.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ug.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cl.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mp.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ik.gzmigu.cn

================================================================================
来源：http://wb.haigaiapp.cn

J. 日期与时间
来源：http://qp.jianghongdianzi.cn

================================================================================
来源：http://zs.bookmarksfly.cn

[J01] 获取当前时间
来源：http://ry.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sk.lnxyls.cn


<!-- 参考信息 -->