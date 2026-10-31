代发 wailian999

TS:   constructor(public name: string) {}
来源：http://po.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://bi.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://km.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://nh.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://lm.huixiangedu.cn

[G03] 实例属性
来源：http://mo.shxzskj.cn

Py:   self.name = "x"
来源：http://rg.521024.cn

PHP:  public string $name = "x";
来源：http://rf.huanxung.cn

JS:   this.name = "x";
来源：http://aa.shxzukj.cn

TS:   name: string = "x";
来源：http://dh.jctech888.com.cn

Java: private String name;
来源：http://gi.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dj.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://jy.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://pd.wgjwhj.cn

[G04] 定义方法
来源：http://dl.hahajie.cn

Py:   def greet(self): return self.name
来源：http://xq.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vz.nszjky.cn

JS:   greet() { return this.name; }
来源：http://jk.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://ig.colortex.cn

Java: String greet() { return name; }
来源：http://ss.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dk.szxytkj.cn

Ruby: def greet; @name; end
来源：http://oo.521024.cn

C#:   public string Greet() => Name;
来源：http://ne.yuntaijiaju.cn

[G05] 继承
来源：http://io.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://qy.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://mj.nszjky.cn

JS:   class Admin extends User {}
来源：http://cu.521024.cn

TS:   class Admin extends User {}
来源：http://ve.shxzukj.cn

Java: class Admin extends User {}
来源：http://gh.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uo.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://pg.jctech888.com.cn

C#:   class Admin : User {}
来源：http://pv.shtwfgs.cn

[G06] 重写方法
来源：http://st.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://vl.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sy.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://gu.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ty.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://pg.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sl.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://gx.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://av.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://qr.shxzskj.cn

Py:   super().greet()
来源：http://lu.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://ga.521024.cn

JS:   super.greet();
来源：http://dx.bookmarksfly.cn

TS:   super.greet();
来源：http://co.colortex.cn

Java: super.greet();
来源：http://nk.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ya.gzmigu.cn

Ruby: super
来源：http://uk.jianghongdianzi.cn

C#:   base.Greet();
来源：http://ot.huixiangedu.cn

[G08] 静态方法与属性
来源：http://yv.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vj.muxihuayi.cn

PHP:  public static function f() {}
来源：http://ri.jctech888.com.cn

JS:   static f() {}
来源：http://fm.colortex.cn

TS:   static f(): void {}
来源：http://vn.chemitech.net.cn

Java: static void f() {}
来源：http://th.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oy.shxzukj.cn

Ruby: def self.f; end
来源：http://fo.panjiajie.cn

C#:   public static void F() {}
来源：http://kg.hahajie.cn

[G09] 接口 / 抽象类
来源：http://uk.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://dr.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qs.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://en.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://dh.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://gv.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ot.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mg.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://rj.wgjwhj.cn

[G10] 访问控制
来源：http://cq.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://of.szsharing.cn

PHP:  public / protected / private
来源：http://sb.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://bf.shtwfgs.cn

TS:   public / protected / private
来源：http://ce.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://zc.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qk.shxzukj.cn

Ruby: public / protected / private
来源：http://ih.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://qu.nszjky.cn

[G11] getter / setter
来源：http://jf.hahajie.cn

Py:   @property 与 @x.setter
来源：http://zp.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gz.521024.cn

JS:   get name() { return this._name; }
来源：http://sb.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://ao.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://zl.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yp.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://sw.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://by.gzmigu.cn

[G12] 对象转字符串
来源：http://rt.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://hy.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oy.colortex.cn

JS:   toString() { return this.name; }
来源：http://gg.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://tf.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://ol.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zm.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://ub.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://bo.shxzskj.cn

[G13] 判断对象类型
来源：http://xd.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://wa.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://tp.asd995.cn

JS:   u instanceof User
来源：http://de.nicolike.cn

TS:   u instanceof User
来源：http://qn.gzmigu.cn

Java: u instanceof User
来源：http://eh.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jr.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://tf.jianghongdianzi.cn

C#:   u is User
来源：http://rw.nicolike.cn

[G14] 数据类 / record
来源：http://fv.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lo.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://fe.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kn.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://rs.nicolike.cn

Java: record User(String name, int age) {}
来源：http://pm.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://xs.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pe.asd995.cn

C#:   record User(string Name, int Age);
来源：http://kq.jianghongdianzi.cn

[G15] 枚举
来源：http://or.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xt.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ee.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lr.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uc.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://mv.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fk.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://vk.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://no.521024.cn

[G16] 对象转数组 / 字典
来源：http://ii.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xe.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://ky.szxytkj.cn

JS:   Object.entries(obj)
来源：http://yl.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://pz.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ul.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cc.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://qh.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://bi.hnjuh.cn

================================================================================
来源：http://li.panjiajie.cn

H. 异常与错误处理
来源：http://ub.bjjhwx.cn

================================================================================
来源：http://py.muxihuayi.cn

[H01] try / catch 基础
来源：http://da.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ra.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ef.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fe.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fg.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uc.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vu.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pj.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ys.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://wq.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lx.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fx.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://se.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dt.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zh.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qz.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xe.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vv.yuexingan06.cn

[H03] 主动抛出异常
来源：http://sw.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ls.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bs.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://vj.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://ux.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pc.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tl.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ev.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xb.panjiajie.cn

[H04] 自定义异常类型
来源：http://ox.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://gd.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qm.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://ic.nszjky.cn

TS:   class MyError extends Error {}
来源：http://ak.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://ar.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fv.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://cd.521024.cn

C#:   class MyException : Exception {}
来源：http://oi.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://rt.nszjky.cn

Py:   except ValueError as e:
来源：http://nn.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mi.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://rf.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://ka.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://fz.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bs.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://mm.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zz.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://xv.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://wm.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://in.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pm.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vr.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jz.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oq.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://fh.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://ga.jctech888.com.cn

[H07] 断言
来源：http://ki.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://si.nszjky.cn

PHP:  assert($x > 0);
来源：http://gk.newstarts.cn

JS:   console.assert(x > 0);
来源：http://rv.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://vb.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://wc.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ya.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ia.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://hm.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://hy.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://se.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nx.521024.cn

JS:   e.message;  e.stack
来源：http://ib.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xx.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xt.colortex.cn

Go:   err.Error()
来源：http://mf.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://dp.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://tt.nszjky.cn

[H09] 带错误码的异常
来源：http://hk.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gm.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kc.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://et.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wv.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hq.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lk.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ho.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vd.gzmigu.cn

[H10] 资源自动释放
来源：http://gt.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://so.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xu.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cg.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qa.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pz.9csxet.cn

Go:   defer f.Close()
来源：http://tr.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mg.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xi.lnxyls.cn

================================================================================
来源：http://ac.bjjhwx.cn

I. 正则表达式
来源：http://hv.colortex.cn

================================================================================
来源：http://il.jctech888.com.cn

[I01] 判断是否匹配
来源：http://ym.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jj.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dy.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://ve.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://xq.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ne.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wd.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://gq.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fg.yuexingan06.cn

[I02] 提取所有匹配
来源：http://af.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ff.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ep.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rl.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://bi.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rq.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lr.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://nh.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fv.nicolike.cn

[I03] 提取捕获分组
来源：http://ui.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ju.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dl.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xh.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cr.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fd.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ci.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tb.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xh.bjjhwx.cn

[I04] 正则替换
来源：http://wf.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ep.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sz.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hw.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gq.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dw.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pi.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xq.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wv.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://ij.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nk.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yj.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://yl.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://wy.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://jd.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zg.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ln.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vz.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://no.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fo.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://av.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hl.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nj.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cp.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://br.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ri.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rd.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://nz.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yf.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dd.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hk.huanxung.cn

TS:   /error/gim
来源：http://mz.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://he.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mh.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://xd.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nd.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://fl.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ta.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oa.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jg.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xq.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://es.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uf.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gj.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zv.huanxung.cn

================================================================================
来源：http://ei.jctech888.com.cn


<!-- 参考信息 -->