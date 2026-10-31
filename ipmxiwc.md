代发 wailian999

TS:   constructor(public name: string) {}
来源：http://tw.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://vf.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zr.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ic.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://wd.yuntaijiaju.cn

[G03] 实例属性
来源：http://ma.521024.cn

Py:   self.name = "x"
来源：http://qm.hnjuh.cn

PHP:  public string $name = "x";
来源：http://gw.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://fb.huixiangedu.cn

TS:   name: string = "x";
来源：http://hg.hnjuh.cn

Java: private String name;
来源：http://mq.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wi.shxzukj.cn

Ruby: @name = "x"
来源：http://cb.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://gj.colortex.cn

[G04] 定义方法
来源：http://lo.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://gp.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gt.nszjky.cn

JS:   greet() { return this.name; }
来源：http://no.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://ga.yuexingan06.cn

Java: String greet() { return name; }
来源：http://xh.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pb.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://vq.nszjky.cn

C#:   public string Greet() => Name;
来源：http://tf.shtwfgs.cn

[G05] 继承
来源：http://db.lnxyls.cn

Py:   class Admin(User): pass
来源：http://gl.nszjky.cn

PHP:  class Admin extends User {}
来源：http://kr.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://ml.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://xs.hahajie.cn

Java: class Admin extends User {}
来源：http://qs.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rf.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://as.panjiajie.cn

C#:   class Admin : User {}
来源：http://uh.huixiangedu.cn

[G06] 重写方法
来源：http://rn.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://wj.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://je.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://zf.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://fz.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://pz.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rm.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://ik.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://wk.haigaiapp.cn

[G07] 调用父类方法
来源：http://yo.haigaiapp.cn

Py:   super().greet()
来源：http://pw.shxzskj.cn

PHP:  parent::greet();
来源：http://pe.wgjwhj.cn

JS:   super.greet();
来源：http://fm.colortex.cn

TS:   super.greet();
来源：http://tt.shxzukj.cn

Java: super.greet();
来源：http://qq.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qx.szxytkj.cn

Ruby: super
来源：http://se.wgjwhj.cn

C#:   base.Greet();
来源：http://bt.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://fs.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kd.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://qw.yuntaijiaju.cn

JS:   static f() {}
来源：http://lw.panjiajie.cn

TS:   static f(): void {}
来源：http://rt.hahajie.cn

Java: static void f() {}
来源：http://ad.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gg.muxihuayi.cn

Ruby: def self.f; end
来源：http://ij.shtwfgs.cn

C#:   public static void F() {}
来源：http://mj.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://tj.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://hr.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zw.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wg.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://zz.521024.cn

Java: interface Shape { double area(); }
来源：http://og.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://eq.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rc.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://kk.9csxet.cn

[G10] 访问控制
来源：http://sq.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://pt.shtwfgs.cn

PHP:  public / protected / private
来源：http://ef.521024.cn

JS:   #private 字段；其余公开
来源：http://nq.hahajie.cn

TS:   public / protected / private
来源：http://wn.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://ob.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fn.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://hd.huanxung.cn

C#:   public / protected / private / internal
来源：http://nu.newstarts.cn

[G11] getter / setter
来源：http://uk.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://ma.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cv.521024.cn

JS:   get name() { return this._name; }
来源：http://at.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://ro.szxytkj.cn

Java: public String getName() { return name; }
来源：http://fe.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wi.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://ok.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://dk.newstarts.cn

[G12] 对象转字符串
来源：http://fq.colortex.cn

Py:   def __str__(self): return self.name
来源：http://qj.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qv.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://iv.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://hu.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://wz.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://go.hahajie.cn

Ruby: def to_s; @name; end
来源：http://ad.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://uc.wgjwhj.cn

[G13] 判断对象类型
来源：http://yx.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://lr.hnjuh.cn

PHP:  $u instanceof User
来源：http://ql.hnjuh.cn

JS:   u instanceof User
来源：http://dv.shxzukj.cn

TS:   u instanceof User
来源：http://pd.chemitech.net.cn

Java: u instanceof User
来源：http://yn.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://us.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://pm.huanxung.cn

C#:   u is User
来源：http://hk.bjjhwx.cn

[G14] 数据类 / record
来源：http://am.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cn.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://jq.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tm.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://uu.huanxung.cn

Java: record User(String name, int age) {}
来源：http://wv.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://fo.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ak.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://on.szsharing.cn

[G15] 枚举
来源：http://oj.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pb.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hd.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://up.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wd.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://lg.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ey.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://mf.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xi.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://vt.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ef.521024.cn

PHP:  get_object_vars($obj);
来源：http://jx.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://cu.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ch.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vd.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zu.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://db.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://xl.colortex.cn

================================================================================
来源：http://du.chemitech.net.cn

H. 异常与错误处理
来源：http://fv.9csxet.cn

================================================================================
来源：http://mb.asd995.cn

[H01] try / catch 基础
来源：http://je.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xu.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fw.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pd.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vf.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cw.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yg.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kq.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tz.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://cw.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vv.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wn.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://li.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sb.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dp.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bz.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uy.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qy.lnxyls.cn

[H03] 主动抛出异常
来源：http://ig.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://wu.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://em.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://ou.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://ry.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iq.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://za.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://go.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jt.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://hp.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://nw.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ig.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://iq.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://no.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://po.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://va.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://qj.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://dw.nszjky.cn

[H05] 捕获特定类型
来源：http://ma.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://oa.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ci.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://fy.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://rd.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://zd.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ml.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://hb.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vc.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://ag.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://kf.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kg.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nc.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dm.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ba.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ot.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://rp.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://te.hahajie.cn

[H07] 断言
来源：http://kr.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://vp.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://kq.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://dj.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://vr.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://lz.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lb.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://su.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://pj.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://vb.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://vr.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eg.panjiajie.cn

JS:   e.message;  e.stack
来源：http://lg.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bn.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mf.gzmigu.cn

Go:   err.Error()
来源：http://tt.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://po.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://vw.szxytkj.cn

[H09] 带错误码的异常
来源：http://hf.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kz.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xh.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pm.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xc.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jx.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pb.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rs.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fa.wgjwhj.cn

[H10] 资源自动释放
来源：http://jt.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nq.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ou.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://om.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eq.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.colortex.cn

Go:   defer f.Close()
来源：http://tb.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pd.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ms.huanxung.cn

================================================================================
来源：http://vb.shtwfgs.cn

I. 正则表达式
来源：http://if.shxzukj.cn

================================================================================
来源：http://wl.colortex.cn

[I01] 判断是否匹配
来源：http://rv.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jl.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sx.521024.cn

JS:   /\d+/.test(s)
来源：http://zf.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://oh.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iy.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fg.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://cd.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dj.muxihuayi.cn

[I02] 提取所有匹配
来源：http://ep.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://iz.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ad.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ck.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://mt.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ln.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jq.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://tq.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kx.hahajie.cn

[I03] 提取捕获分组
来源：http://fx.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uq.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qq.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yz.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://na.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ex.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fc.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://an.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://av.shxzskj.cn

[I04] 正则替换
来源：http://lm.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dx.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pb.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ec.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yz.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://st.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qo.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ne.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ni.lnxyls.cn

[I05] 按正则拆分
来源：http://xa.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://px.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rl.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://hp.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://ic.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://lx.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yg.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wz.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nv.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rm.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hr.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qo.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cu.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kp.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zu.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xs.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vn.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lx.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://ul.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://du.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fk.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fx.szxytkj.cn

TS:   /error/gim
来源：http://jo.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ej.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ly.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://tp.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aa.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ia.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rn.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bv.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fs.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nv.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tz.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xa.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qt.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fy.bookmarksfly.cn

================================================================================
来源：http://bk.colortex.cn


<!-- 参考信息 -->