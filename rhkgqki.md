代发 wailian999

Py:   class Admin(User): pass
来源：http://yf.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://kl.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://he.shxzukj.cn

TS:   class Admin extends User {}
来源：http://sz.szxytkj.cn

Java: class Admin extends User {}
来源：http://ew.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ve.nicolike.cn

Ruby: class Admin < User; end
来源：http://zm.shtwfgs.cn

C#:   class Admin : User {}
来源：http://lt.hahajie.cn

[G06] 重写方法
来源：http://vr.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://ji.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gq.asd995.cn

JS:   greet() { return "admin"; }
来源：http://ru.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://be.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://zw.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fj.asd995.cn

Ruby: def greet; "admin"; end
来源：http://fv.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://ja.colortex.cn

[G07] 调用父类方法
来源：http://ua.asd995.cn

Py:   super().greet()
来源：http://ip.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://lh.9csxet.cn

JS:   super.greet();
来源：http://zd.jianghongdianzi.cn

TS:   super.greet();
来源：http://aw.szxytkj.cn

Java: super.greet();
来源：http://nu.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wt.hnjuh.cn

Ruby: super
来源：http://jw.panjiajie.cn

C#:   base.Greet();
来源：http://wi.9csxet.cn

[G08] 静态方法与属性
来源：http://yj.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ic.nicolike.cn

PHP:  public static function f() {}
来源：http://xh.shtwfgs.cn

JS:   static f() {}
来源：http://fh.yuexingan06.cn

TS:   static f(): void {}
来源：http://iy.shxzukj.cn

Java: static void f() {}
来源：http://pd.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kb.huanxung.cn

Ruby: def self.f; end
来源：http://bs.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://yv.huanxung.cn

[G09] 接口 / 抽象类
来源：http://vo.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://cd.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ds.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rz.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://ga.szsharing.cn

Java: interface Shape { double area(); }
来源：http://sc.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://hv.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iy.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://pq.shxzukj.cn

[G10] 访问控制
来源：http://cy.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://ec.wgjwhj.cn

PHP:  public / protected / private
来源：http://pe.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://ix.wgjwhj.cn

TS:   public / protected / private
来源：http://jn.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://gi.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pg.9csxet.cn

Ruby: public / protected / private
来源：http://fe.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://yc.newstarts.cn

[G11] getter / setter
来源：http://av.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://yq.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ti.huanxung.cn

JS:   get name() { return this._name; }
来源：http://ng.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://ic.shxzukj.cn

Java: public String getName() { return name; }
来源：http://ni.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zr.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://sd.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://dc.shxzukj.cn

[G12] 对象转字符串
来源：http://ka.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://aq.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fu.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://dm.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://cg.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://ex.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gj.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://xj.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://wk.chemitech.net.cn

[G13] 判断对象类型
来源：http://hj.521024.cn

Py:   isinstance(u, User)
来源：http://qc.shtwfgs.cn

PHP:  $u instanceof User
来源：http://cf.szsharing.cn

JS:   u instanceof User
来源：http://ce.huanxung.cn

TS:   u instanceof User
来源：http://hb.gzmigu.cn

Java: u instanceof User
来源：http://lv.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xe.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://jm.bjjhwx.cn

C#:   u is User
来源：http://pq.nszjky.cn

[G14] 数据类 / record
来源：http://lj.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zo.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://dq.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lm.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://hd.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://ov.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://ru.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bz.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://ko.panjiajie.cn

[G15] 枚举
来源：http://jv.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rm.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kh.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qe.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xe.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://ra.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bf.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://rb.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tp.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://bw.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yc.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://lu.newstarts.cn

JS:   Object.entries(obj)
来源：http://ih.huanxung.cn

TS:   Object.entries(obj)
来源：http://rg.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://he.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sc.521024.cn

Ruby: obj.instance_variables
来源：http://up.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://gt.huanxung.cn

================================================================================
来源：http://im.lnxyls.cn

H. 异常与错误处理
来源：http://lm.szxytkj.cn

================================================================================
来源：http://jk.shxzskj.cn

[H01] try / catch 基础
来源：http://yj.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dw.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vy.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wa.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lt.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fk.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gh.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ix.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tf.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://vz.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fv.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qc.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ll.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vs.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cl.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gx.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lj.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mi.hnjuh.cn

[H03] 主动抛出异常
来源：http://vx.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://oi.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dm.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://fh.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://ld.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sx.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ks.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qw.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fg.wgjwhj.cn

[H04] 自定义异常类型
来源：http://mh.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ag.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vl.huanxung.cn

JS:   class MyError extends Error {}
来源：http://da.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://je.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://jw.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sv.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://hg.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://pq.hahajie.cn

[H05] 捕获特定类型
来源：http://ap.521024.cn

Py:   except ValueError as e:
来源：http://bn.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ak.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://xe.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://pw.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://lb.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ib.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://yb.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oc.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://nu.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://ej.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lj.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fd.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vd.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yc.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qh.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://pf.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://ch.chemitech.net.cn

[H07] 断言
来源：http://ep.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://rm.newstarts.cn

PHP:  assert($x > 0);
来源：http://wr.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://ba.9csxet.cn

TS:   console.assert(x > 0);
来源：http://gs.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://ah.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rn.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ff.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://rp.521024.cn

[H08] 获取错误信息与堆栈
来源：http://hw.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://on.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xn.szsharing.cn

JS:   e.message;  e.stack
来源：http://tj.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tf.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nf.nicolike.cn

Go:   err.Error()
来源：http://wx.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://gy.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://if.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://va.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://td.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hh.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gw.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wc.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yr.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gu.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://on.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ns.nszjky.cn

[H10] 资源自动释放
来源：http://vv.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://el.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xr.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ky.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://md.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xt.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://no.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nj.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ss.shxzukj.cn

================================================================================
来源：http://px.jctech888.com.cn

I. 正则表达式
来源：http://ar.panjiajie.cn

================================================================================
来源：http://va.huixiangedu.cn

[I01] 判断是否匹配
来源：http://mw.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xw.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ia.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://is.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://ed.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ar.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tq.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://hu.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rn.huanxung.cn

[I02] 提取所有匹配
来源：http://is.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://io.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wr.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jj.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://ed.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ws.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://de.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://tf.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oc.521024.cn

[I03] 提取捕获分组
来源：http://ix.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wl.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fb.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pl.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ac.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://be.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fo.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xa.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uw.huixinmuqiang.cn

[I04] 正则替换
来源：http://ue.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vv.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ja.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kp.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xk.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gr.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cg.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://up.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gp.9csxet.cn

[I05] 按正则拆分
来源：http://pq.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fu.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jb.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://yv.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://kt.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://yo.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rr.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ke.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bx.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ex.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nx.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tx.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jt.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yj.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ye.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rs.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ta.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jc.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://dt.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gc.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://io.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lj.521024.cn

TS:   /error/gim
来源：http://my.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pf.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ce.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://sd.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ty.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://iu.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zd.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fh.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tx.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vw.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zc.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rl.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tn.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ka.huixiangedu.cn

================================================================================
来源：http://gz.newstarts.cn

J. 日期与时间
来源：http://mz.yuntaijiaju.cn

================================================================================
来源：http://yg.bookmarksfly.cn

[J01] 获取当前时间
来源：http://pf.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://su.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ni.521024.cn

JS:   new Date();  Date.now()
来源：http://em.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://cw.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zl.gzmigu.cn

Go:   time.Now()
来源：http://ky.521024.cn

Ruby: Time.now
来源：http://nb.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fs.521024.cn

[J02] 格式化输出
来源：http://jn.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hv.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yb.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ol.huixiangedu.cn

TS:   d.toISOString()
来源：http://re.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vr.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pm.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kh.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vs.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://rd.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://so.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wn.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://ve.shtwfgs.cn


<!-- 参考信息 -->