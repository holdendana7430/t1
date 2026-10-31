代发 wailian999

[G02] 构造函数
来源：http://xr.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://qr.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://js.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://pj.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://kv.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://xl.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rz.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://pq.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://aa.9csxet.cn

[G03] 实例属性
来源：http://eo.jctech888.com.cn

Py:   self.name = "x"
来源：http://xr.szxytkj.cn

PHP:  public string $name = "x";
来源：http://ph.lnxyls.cn

JS:   this.name = "x";
来源：http://hr.shxzukj.cn

TS:   name: string = "x";
来源：http://lz.haigaiapp.cn

Java: private String name;
来源：http://lu.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xy.shxzukj.cn

Ruby: @name = "x"
来源：http://af.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://zy.lnxyls.cn

[G04] 定义方法
来源：http://jd.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://wf.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ak.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://yh.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://ua.asd995.cn

Java: String greet() { return name; }
来源：http://lf.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bt.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://yg.asd995.cn

C#:   public string Greet() => Name;
来源：http://nn.shxzukj.cn

[G05] 继承
来源：http://qd.huanxung.cn

Py:   class Admin(User): pass
来源：http://yk.huanxung.cn

PHP:  class Admin extends User {}
来源：http://hg.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://wq.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://gu.hnjuh.cn

Java: class Admin extends User {}
来源：http://oe.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ab.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://hw.panjiajie.cn

C#:   class Admin : User {}
来源：http://rw.nicolike.cn

[G06] 重写方法
来源：http://is.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://ws.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rc.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://lq.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://bb.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://qz.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ki.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://xw.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://et.lnxyls.cn

[G07] 调用父类方法
来源：http://cp.huixinmuqiang.cn

Py:   super().greet()
来源：http://zg.bookmarksfly.cn

PHP:  parent::greet();
来源：http://yy.521024.cn

JS:   super.greet();
来源：http://dx.yuntaijiaju.cn

TS:   super.greet();
来源：http://as.nicolike.cn

Java: super.greet();
来源：http://du.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sn.asd995.cn

Ruby: super
来源：http://yz.muxihuayi.cn

C#:   base.Greet();
来源：http://za.gzmigu.cn

[G08] 静态方法与属性
来源：http://et.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://de.jctech888.com.cn

PHP:  public static function f() {}
来源：http://oj.huanxung.cn

JS:   static f() {}
来源：http://ut.bookmarksfly.cn

TS:   static f(): void {}
来源：http://xz.521024.cn

Java: static void f() {}
来源：http://xh.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gs.haigaiapp.cn

Ruby: def self.f; end
来源：http://wz.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://by.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ti.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ua.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uc.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://si.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://dk.huanxung.cn

Java: interface Shape { double area(); }
来源：http://vl.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ab.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ad.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://vy.9csxet.cn

[G10] 访问控制
来源：http://hj.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ni.newstarts.cn

PHP:  public / protected / private
来源：http://sb.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://vk.9csxet.cn

TS:   public / protected / private
来源：http://am.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://zw.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jr.9csxet.cn

Ruby: public / protected / private
来源：http://yt.nszjky.cn

C#:   public / protected / private / internal
来源：http://wi.huixinmuqiang.cn

[G11] getter / setter
来源：http://fy.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://tw.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hd.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://ib.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://hx.asd995.cn

Java: public String getName() { return name; }
来源：http://ud.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wz.lnxyls.cn

Ruby: attr_accessor :name
来源：http://zz.521024.cn

C#:   public string Name { get; set; }
来源：http://jv.colortex.cn

[G12] 对象转字符串
来源：http://zh.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://pu.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jc.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://lk.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://ih.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://ya.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ka.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://zb.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://iu.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://og.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://la.lnxyls.cn

PHP:  $u instanceof User
来源：http://cu.szxytkj.cn

JS:   u instanceof User
来源：http://lb.nicolike.cn

TS:   u instanceof User
来源：http://zz.jctech888.com.cn

Java: u instanceof User
来源：http://mm.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cx.szsharing.cn

Ruby: u.is_a?(User)
来源：http://ze.shxzskj.cn

C#:   u is User
来源：http://dj.lnxyls.cn

[G14] 数据类 / record
来源：http://ln.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://af.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://rd.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ec.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://ed.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://cl.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://cq.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sv.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://hh.huixinmuqiang.cn

[G15] 枚举
来源：http://gd.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ra.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bw.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rq.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tu.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://ly.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fh.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://ap.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yh.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://hq.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fq.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://ht.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://cd.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://ig.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qk.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ql.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://jv.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://pf.shxzskj.cn

================================================================================
来源：http://xl.bjjhwx.cn

H. 异常与错误处理
来源：http://gb.shtwfgs.cn

================================================================================
来源：http://lg.shtwfgs.cn

[H01] try / catch 基础
来源：http://ld.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kw.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xp.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://if.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mj.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jr.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://du.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ac.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gt.huanxung.cn

[H02] finally / ensure 收尾
来源：http://gf.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ub.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ki.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mz.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://st.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zi.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fs.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://az.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://la.asd995.cn

[H03] 主动抛出异常
来源：http://wo.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://hd.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ss.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://cn.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://mx.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vq.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ve.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rv.huanxung.cn

[H04] 自定义异常类型
来源：http://hb.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://ys.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ln.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://cc.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://gn.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://vj.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cd.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://iw.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://jd.huixiangedu.cn

[H05] 捕获特定类型
来源：http://vv.bjjhwx.cn

Py:   except ValueError as e:
来源：http://wv.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://en.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://xh.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://pm.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://bt.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nh.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://oj.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gu.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://jl.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://gc.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ik.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vq.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://um.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gc.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lp.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://ft.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://dk.huixinmuqiang.cn

[H07] 断言
来源：http://zx.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://ti.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://ca.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://kv.hahajie.cn

TS:   console.assert(x > 0);
来源：http://sv.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://bb.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zn.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fd.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://on.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://lz.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://gg.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bz.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://xz.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jv.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://af.bookmarksfly.cn

Go:   err.Error()
来源：http://iz.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://vx.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ul.shxzukj.cn

[H09] 带错误码的异常
来源：http://vu.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ye.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xs.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gx.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cq.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mi.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rm.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ou.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sg.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://yr.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hy.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gc.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aq.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zm.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dx.huixiangedu.cn

Go:   defer f.Close()
来源：http://ih.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ha.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yb.colortex.cn

================================================================================
来源：http://pf.yuexingan06.cn

I. 正则表达式
来源：http://ra.shxzukj.cn

================================================================================
来源：http://ak.lnxyls.cn

[I01] 判断是否匹配
来源：http://hu.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lo.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pc.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://yc.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://aw.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sb.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zr.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://ps.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bq.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://rb.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://la.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://im.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cg.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://pu.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ez.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ra.521024.cn

Ruby: s.scan(/\d+/)
来源：http://mm.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ol.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://xx.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ks.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oo.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://it.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vh.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eh.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ga.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://we.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://og.asd995.cn

[I04] 正则替换
来源：http://ga.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yo.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oc.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tf.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nr.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jr.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nw.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eb.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wo.muxihuayi.cn

[I05] 按正则拆分
来源：http://tu.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ka.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://up.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://sy.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://nk.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://kt.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://od.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lr.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ce.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gs.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tb.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jb.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hw.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ma.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mr.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fg.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hb.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lv.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://qv.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lz.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eh.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yj.jctech888.com.cn

TS:   /error/gim
来源：http://fu.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kr.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jw.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://jt.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xv.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://xe.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://od.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zc.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yd.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yz.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gk.panjiajie.cn


<!-- 参考信息 -->