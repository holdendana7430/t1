代发 wailian999

TS:   constructor(public name: string) {}
来源：http://rk.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://je.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rj.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://sv.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://iz.9csxet.cn

[G03] 实例属性
来源：http://xs.shtwfgs.cn

Py:   self.name = "x"
来源：http://ri.panjiajie.cn

PHP:  public string $name = "x";
来源：http://wp.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://yj.huixiangedu.cn

TS:   name: string = "x";
来源：http://jg.9csxet.cn

Java: private String name;
来源：http://bl.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uv.bjjhwx.cn

Ruby: @name = "x"
来源：http://zw.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://mw.panjiajie.cn

[G04] 定义方法
来源：http://iq.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://eu.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://df.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://ox.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://tr.huanxung.cn

Java: String greet() { return name; }
来源：http://qm.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://id.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://bo.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://vq.521024.cn

[G05] 继承
来源：http://ph.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ot.nicolike.cn

PHP:  class Admin extends User {}
来源：http://zy.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://tm.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://za.huixiangedu.cn

Java: class Admin extends User {}
来源：http://lb.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kc.shxzskj.cn

Ruby: class Admin < User; end
来源：http://yz.huixiangedu.cn

C#:   class Admin : User {}
来源：http://lv.huanxung.cn

[G06] 重写方法
来源：http://bs.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://bw.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tu.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://up.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ni.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://br.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mp.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://yc.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://ir.jctech888.com.cn

[G07] 调用父类方法
来源：http://ay.shxzskj.cn

Py:   super().greet()
来源：http://zc.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://vv.szxytkj.cn

JS:   super.greet();
来源：http://tx.jctech888.com.cn

TS:   super.greet();
来源：http://ct.9csxet.cn

Java: super.greet();
来源：http://tz.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vq.bookmarksfly.cn

Ruby: super
来源：http://uv.szxytkj.cn

C#:   base.Greet();
来源：http://ed.szxytkj.cn

[G08] 静态方法与属性
来源：http://ue.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tt.nicolike.cn

PHP:  public static function f() {}
来源：http://vz.newstarts.cn

JS:   static f() {}
来源：http://ba.lnxyls.cn

TS:   static f(): void {}
来源：http://lf.yuntaijiaju.cn

Java: static void f() {}
来源：http://va.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ot.gzmigu.cn

Ruby: def self.f; end
来源：http://vk.hnjuh.cn

C#:   public static void F() {}
来源：http://am.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://bg.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://je.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ix.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cr.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://bf.9csxet.cn

Java: interface Shape { double area(); }
来源：http://ub.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://tb.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fj.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://jr.bjjhwx.cn

[G10] 访问控制
来源：http://xt.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://mv.hahajie.cn

PHP:  public / protected / private
来源：http://an.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://dj.jianghongdianzi.cn

TS:   public / protected / private
来源：http://ig.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://ig.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gy.asd995.cn

Ruby: public / protected / private
来源：http://zs.panjiajie.cn

C#:   public / protected / private / internal
来源：http://fl.nszjky.cn

[G11] getter / setter
来源：http://og.huanxung.cn

Py:   @property 与 @x.setter
来源：http://ty.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://an.newstarts.cn

JS:   get name() { return this._name; }
来源：http://fr.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://va.newstarts.cn

Java: public String getName() { return name; }
来源：http://xi.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://um.szsharing.cn

Ruby: attr_accessor :name
来源：http://ql.huanxung.cn

C#:   public string Name { get; set; }
来源：http://ld.nszjky.cn

[G12] 对象转字符串
来源：http://ou.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://ak.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jx.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://kb.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://et.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://fr.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oj.nszjky.cn

Ruby: def to_s; @name; end
来源：http://ol.521024.cn

C#:   public override string ToString() => Name;
来源：http://kz.bookmarksfly.cn

[G13] 判断对象类型
来源：http://qe.hahajie.cn

Py:   isinstance(u, User)
来源：http://ed.shtwfgs.cn

PHP:  $u instanceof User
来源：http://mv.haigaiapp.cn

JS:   u instanceof User
来源：http://ji.9csxet.cn

TS:   u instanceof User
来源：http://kw.szsharing.cn

Java: u instanceof User
来源：http://zg.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://di.nszjky.cn

Ruby: u.is_a?(User)
来源：http://ex.szsharing.cn

C#:   u is User
来源：http://dj.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://yn.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wr.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://tu.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://he.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://pn.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://hb.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://aq.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ov.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://bd.muxihuayi.cn

[G15] 枚举
来源：http://aq.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kx.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kl.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mf.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fo.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://hi.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://md.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://kw.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wq.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://js.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hr.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://yg.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://xd.nicolike.cn

TS:   Object.entries(obj)
来源：http://dj.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gg.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://od.nicolike.cn

Ruby: obj.instance_variables
来源：http://sy.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://rs.colortex.cn

================================================================================
来源：http://nh.colortex.cn

H. 异常与错误处理
来源：http://tz.shxzukj.cn

================================================================================
来源：http://kn.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://gj.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zy.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ci.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fh.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xy.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ha.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ou.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ip.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ks.nszjky.cn

[H02] finally / ensure 收尾
来源：http://xs.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ca.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gm.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ow.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dz.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xz.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lu.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dh.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eo.huanxung.cn

[H03] 主动抛出异常
来源：http://yl.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://ju.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ge.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://ga.521024.cn

TS:   throw new Error("错误信息");
来源：http://gi.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xb.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sh.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nx.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ve.hnjuh.cn

[H04] 自定义异常类型
来源：http://rb.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://go.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tg.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://mj.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://eb.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://ni.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wr.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://zy.huanxung.cn

C#:   class MyException : Exception {}
来源：http://zn.nszjky.cn

[H05] 捕获特定类型
来源：http://xs.chemitech.net.cn

Py:   except ValueError as e:
来源：http://vk.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cz.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://mg.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://qh.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://wo.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ir.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://rm.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iv.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://mi.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://wo.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gm.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xu.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fc.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fb.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://af.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://ci.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://re.wgjwhj.cn

[H07] 断言
来源：http://wp.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://fa.colortex.cn

PHP:  assert($x > 0);
来源：http://qf.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://da.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://jt.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://nf.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nw.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zm.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://qw.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://my.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://av.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xg.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://rm.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hg.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fz.shxzskj.cn

Go:   err.Error()
来源：http://xd.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://hu.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://ng.bjjhwx.cn

[H09] 带错误码的异常
来源：http://mb.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zt.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wc.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ry.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uw.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zq.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oz.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pw.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vu.wgjwhj.cn

[H10] 资源自动释放
来源：http://hc.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fc.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://la.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://af.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cc.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ly.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://nu.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qr.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ut.huixiangedu.cn

================================================================================
来源：http://fh.haigaiapp.cn

I. 正则表达式
来源：http://mc.nszjky.cn

================================================================================
来源：http://xf.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://sx.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ey.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wn.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://hs.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://wz.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xc.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://es.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://jm.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pq.wgjwhj.cn

[I02] 提取所有匹配
来源：http://kp.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://sj.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tm.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cm.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://kf.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hq.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ks.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://if.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ab.asd995.cn

[I03] 提取捕获分组
来源：http://fa.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://he.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cq.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ta.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://br.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qm.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://we.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jv.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://na.wgjwhj.cn

[I04] 正则替换
来源：http://or.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ya.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bu.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mk.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nk.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cj.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bg.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tb.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qh.newstarts.cn

[I05] 按正则拆分
来源：http://nk.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bt.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rb.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://lz.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://zl.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://wc.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ph.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://at.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ft.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dr.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uv.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yd.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uj.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qh.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jx.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://je.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xc.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kx.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ct.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oc.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gv.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kt.panjiajie.cn

TS:   /error/gim
来源：http://an.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ss.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zg.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ay.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sh.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://tj.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xp.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lh.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gv.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sy.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://us.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wb.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zo.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iw.jctech888.com.cn

================================================================================
来源：http://qr.colortex.cn


<!-- 参考信息 -->