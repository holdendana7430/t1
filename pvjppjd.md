代发 wailian999

Java: class User {}
来源：http://ql.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://px.bjjhwx.cn

Ruby: class User; end
来源：http://sn.haigaiapp.cn

C#:   class User {}
来源：http://pj.yuexingan06.cn

[G02] 构造函数
来源：http://ei.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://td.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://wb.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://jj.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://gs.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://oy.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nm.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://tw.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://wo.9csxet.cn

[G03] 实例属性
来源：http://gd.huanxung.cn

Py:   self.name = "x"
来源：http://dw.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://zl.muxihuayi.cn

JS:   this.name = "x";
来源：http://jq.newstarts.cn

TS:   name: string = "x";
来源：http://ic.panjiajie.cn

Java: private String name;
来源：http://sf.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ms.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://kk.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://eh.colortex.cn

[G04] 定义方法
来源：http://gw.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://hk.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cu.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://rh.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://jc.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://jr.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://le.szsharing.cn

Ruby: def greet; @name; end
来源：http://gb.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://vg.yuexingan06.cn

[G05] 继承
来源：http://ex.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://yt.newstarts.cn

PHP:  class Admin extends User {}
来源：http://us.hahajie.cn

JS:   class Admin extends User {}
来源：http://vw.szxytkj.cn

TS:   class Admin extends User {}
来源：http://cn.jctech888.com.cn

Java: class Admin extends User {}
来源：http://yo.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ti.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://kw.shtwfgs.cn

C#:   class Admin : User {}
来源：http://hn.jianghongdianzi.cn

[G06] 重写方法
来源：http://ek.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://rx.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wm.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://vo.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://eq.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://ly.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wy.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://ik.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://bj.shxzukj.cn

[G07] 调用父类方法
来源：http://zw.nszjky.cn

Py:   super().greet()
来源：http://ys.chemitech.net.cn

PHP:  parent::greet();
来源：http://sw.chemitech.net.cn

JS:   super.greet();
来源：http://pm.hahajie.cn

TS:   super.greet();
来源：http://ir.panjiajie.cn

Java: super.greet();
来源：http://fs.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://za.bookmarksfly.cn

Ruby: super
来源：http://xu.haigaiapp.cn

C#:   base.Greet();
来源：http://rl.shxzskj.cn

[G08] 静态方法与属性
来源：http://bs.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tv.wgjwhj.cn

PHP:  public static function f() {}
来源：http://lr.shxzskj.cn

JS:   static f() {}
来源：http://jv.shxzskj.cn

TS:   static f(): void {}
来源：http://sd.shtwfgs.cn

Java: static void f() {}
来源：http://ts.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vd.chemitech.net.cn

Ruby: def self.f; end
来源：http://iv.szsharing.cn

C#:   public static void F() {}
来源：http://xy.hahajie.cn

[G09] 接口 / 抽象类
来源：http://qp.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://gf.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bf.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ai.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://wi.asd995.cn

Java: interface Shape { double area(); }
来源：http://tx.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://cf.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ww.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://bx.huanxung.cn

[G10] 访问控制
来源：http://be.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://ff.shxzukj.cn

PHP:  public / protected / private
来源：http://mb.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://pa.yuntaijiaju.cn

TS:   public / protected / private
来源：http://rn.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://rl.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oa.szsharing.cn

Ruby: public / protected / private
来源：http://yp.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://hn.chemitech.net.cn

[G11] getter / setter
来源：http://nx.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ss.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://to.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://lm.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://am.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://dr.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cu.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://aw.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://es.lnxyls.cn

[G12] 对象转字符串
来源：http://ro.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://qr.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ww.asd995.cn

JS:   toString() { return this.name; }
来源：http://bz.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://is.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://rc.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ow.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://zp.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://uc.yuexingan06.cn

[G13] 判断对象类型
来源：http://io.szxytkj.cn

Py:   isinstance(u, User)
来源：http://vp.muxihuayi.cn

PHP:  $u instanceof User
来源：http://jm.yuexingan06.cn

JS:   u instanceof User
来源：http://cx.huanxung.cn

TS:   u instanceof User
来源：http://me.jctech888.com.cn

Java: u instanceof User
来源：http://dz.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sd.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://oi.huixinmuqiang.cn

C#:   u is User
来源：http://fd.huixiangedu.cn

[G14] 数据类 / record
来源：http://om.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ep.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://rx.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ua.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://tf.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://be.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://qw.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zh.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://mv.bookmarksfly.cn

[G15] 枚举
来源：http://kp.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qk.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sw.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tx.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eq.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://oe.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ig.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://ap.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vc.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://wj.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ja.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://ew.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://vm.nicolike.cn

TS:   Object.entries(obj)
来源：http://wo.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kq.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jn.hnjuh.cn

Ruby: obj.instance_variables
来源：http://xk.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://al.huixinmuqiang.cn

================================================================================
来源：http://on.521024.cn

H. 异常与错误处理
来源：http://bm.521024.cn

================================================================================
来源：http://zt.panjiajie.cn

[H01] try / catch 基础
来源：http://tk.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hh.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mv.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://py.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zj.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ch.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zb.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kj.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yk.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://yl.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vz.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://en.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vq.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jf.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dv.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dp.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dd.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oo.hnjuh.cn

[H03] 主动抛出异常
来源：http://yl.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://fk.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pv.521024.cn

JS:   throw new Error("错误信息");
来源：http://or.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://zi.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iy.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fr.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hc.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qu.haigaiapp.cn

[H04] 自定义异常类型
来源：http://dw.colortex.cn

Py:   class MyError(Exception): pass
来源：http://av.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yy.9csxet.cn

JS:   class MyError extends Error {}
来源：http://mq.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://gn.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://nn.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ia.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://lk.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://ef.haigaiapp.cn

[H05] 捕获特定类型
来源：http://dt.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://rr.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://is.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://hc.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://na.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://qa.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tm.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://ty.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://be.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://du.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://os.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jc.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qn.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nw.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ah.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://le.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://tv.521024.cn

C#:   obj?.A?.B ?? default
来源：http://zm.lnxyls.cn

[H07] 断言
来源：http://fm.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://jn.nicolike.cn

PHP:  assert($x > 0);
来源：http://al.szsharing.cn

JS:   console.assert(x > 0);
来源：http://br.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://dq.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://rh.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mm.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tq.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://cr.521024.cn

[H08] 获取错误信息与堆栈
来源：http://wv.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://mq.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gm.hnjuh.cn

JS:   e.message;  e.stack
来源：http://ad.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tn.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://of.bjjhwx.cn

Go:   err.Error()
来源：http://vx.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://jj.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://qb.bjjhwx.cn

[H09] 带错误码的异常
来源：http://fg.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xn.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ob.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ds.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xh.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dz.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pn.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cg.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://os.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://tz.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://si.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://me.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bv.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://br.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nj.newstarts.cn

Go:   defer f.Close()
来源：http://ji.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gz.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xb.chemitech.net.cn

================================================================================
来源：http://uo.lnxyls.cn

I. 正则表达式
来源：http://df.9csxet.cn

================================================================================
来源：http://gm.gzmigu.cn

[I01] 判断是否匹配
来源：http://bj.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wo.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yl.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://bx.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://dx.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ad.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://os.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://ln.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kw.jctech888.com.cn

[I02] 提取所有匹配
来源：http://dr.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://qe.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ns.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pk.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://ow.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bw.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tp.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://td.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tc.nszjky.cn

[I03] 提取捕获分组
来源：http://jr.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dd.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ci.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://am.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ll.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vb.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bc.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yx.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wj.gzmigu.cn

[I04] 正则替换
来源：http://dr.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ok.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hl.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dc.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cr.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ig.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fr.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kk.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sw.bookmarksfly.cn

[I05] 按正则拆分
来源：http://vk.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kk.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uz.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://rw.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://sr.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://aj.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://da.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vk.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ro.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zr.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kj.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wg.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fz.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://be.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mn.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xz.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ui.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wl.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://eh.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ld.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wl.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rj.nicolike.cn

TS:   /error/gim
来源：http://kz.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pk.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://lr.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rt.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ib.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sk.nszjky.cn


<!-- 参考信息 -->