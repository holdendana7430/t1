代发 wailian999

Ruby: @name = "x"
来源：http://mz.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ol.yuexingan06.cn

[G04] 定义方法
来源：http://xu.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://qx.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dz.nszjky.cn

JS:   greet() { return this.name; }
来源：http://ed.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://ra.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://am.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yy.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://bm.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://yu.szsharing.cn

[G05] 继承
来源：http://sl.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://zt.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://om.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://jc.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://kn.9csxet.cn

Java: class Admin extends User {}
来源：http://mx.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bl.colortex.cn

Ruby: class Admin < User; end
来源：http://qn.lnxyls.cn

C#:   class Admin : User {}
来源：http://ng.jianghongdianzi.cn

[G06] 重写方法
来源：http://dq.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://jv.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ak.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://ip.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://fs.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://jr.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wg.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://yi.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://cn.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://am.chemitech.net.cn

Py:   super().greet()
来源：http://rt.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://oj.huanxung.cn

JS:   super.greet();
来源：http://ma.huixiangedu.cn

TS:   super.greet();
来源：http://ds.szsharing.cn

Java: super.greet();
来源：http://lg.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xd.szsharing.cn

Ruby: super
来源：http://kg.lnxyls.cn

C#:   base.Greet();
来源：http://ct.huanxung.cn

[G08] 静态方法与属性
来源：http://ia.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sq.shxzskj.cn

PHP:  public static function f() {}
来源：http://qh.521024.cn

JS:   static f() {}
来源：http://pr.gzmigu.cn

TS:   static f(): void {}
来源：http://sc.szxytkj.cn

Java: static void f() {}
来源：http://id.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lw.shxzukj.cn

Ruby: def self.f; end
来源：http://yl.9csxet.cn

C#:   public static void F() {}
来源：http://pg.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://kb.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://mj.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cj.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rz.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://sa.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://du.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://yo.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lc.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://ke.huixiangedu.cn

[G10] 访问控制
来源：http://xx.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://cs.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://uc.hahajie.cn

JS:   #private 字段；其余公开
来源：http://nv.nszjky.cn

TS:   public / protected / private
来源：http://mn.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://do.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ge.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://qz.hahajie.cn

C#:   public / protected / private / internal
来源：http://hw.asd995.cn

[G11] getter / setter
来源：http://xn.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://yl.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vs.huanxung.cn

JS:   get name() { return this._name; }
来源：http://ex.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://sf.shxzukj.cn

Java: public String getName() { return name; }
来源：http://zr.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ir.panjiajie.cn

Ruby: attr_accessor :name
来源：http://om.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://je.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://kk.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://yd.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cr.nicolike.cn

JS:   toString() { return this.name; }
来源：http://gh.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://qt.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://hj.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eb.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://wc.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://gh.nszjky.cn

[G13] 判断对象类型
来源：http://gl.lnxyls.cn

Py:   isinstance(u, User)
来源：http://vv.szxytkj.cn

PHP:  $u instanceof User
来源：http://sv.newstarts.cn

JS:   u instanceof User
来源：http://fh.huixinmuqiang.cn

TS:   u instanceof User
来源：http://lt.nszjky.cn

Java: u instanceof User
来源：http://qe.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zj.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://sr.shxzskj.cn

C#:   u is User
来源：http://ip.newstarts.cn

[G14] 数据类 / record
来源：http://sg.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ua.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://dz.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ec.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://dt.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://sh.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://db.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gd.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://hq.colortex.cn

[G15] 枚举
来源：http://eg.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vy.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pr.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dz.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://za.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://sx.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://td.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://ol.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ch.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://pg.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jt.colortex.cn

PHP:  get_object_vars($obj);
来源：http://ty.nicolike.cn

JS:   Object.entries(obj)
来源：http://ks.9csxet.cn

TS:   Object.entries(obj)
来源：http://uc.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yt.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fp.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://yx.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://av.jctech888.com.cn

================================================================================
来源：http://kz.shxzukj.cn

H. 异常与错误处理
来源：http://cb.shtwfgs.cn

================================================================================
来源：http://ay.huixiangedu.cn

[H01] try / catch 基础
来源：http://ki.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lu.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nz.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qp.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yg.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dw.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gz.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pi.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bw.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://nk.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qm.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lf.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oc.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ds.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://go.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ah.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zo.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ao.nszjky.cn

[H03] 主动抛出异常
来源：http://lo.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://oy.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wp.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ss.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://kj.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jn.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pn.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://me.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ky.nicolike.cn

[H04] 自定义异常类型
来源：http://tr.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://bc.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lv.521024.cn

JS:   class MyError extends Error {}
来源：http://gq.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://fv.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://rp.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xt.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://li.huanxung.cn

C#:   class MyException : Exception {}
来源：http://bs.chemitech.net.cn

[H05] 捕获特定类型
来源：http://ty.hnjuh.cn

Py:   except ValueError as e:
来源：http://pl.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hx.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://ms.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://bl.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://ez.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zu.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://vf.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mi.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://im.huanxung.cn

Py:   value = d.get("k") or default
来源：http://te.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fc.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eu.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mf.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pm.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ls.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://yz.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://id.newstarts.cn

[H07] 断言
来源：http://hy.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://go.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://jx.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://kx.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://ky.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://as.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pu.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://be.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://hc.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://nq.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://pf.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xe.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://mf.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wg.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gg.9csxet.cn

Go:   err.Error()
来源：http://ap.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://qg.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://pt.521024.cn

[H09] 带错误码的异常
来源：http://zc.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dd.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vw.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://by.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lg.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fv.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kj.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oh.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xd.jctech888.com.cn

[H10] 资源自动释放
来源：http://xd.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://op.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gs.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zc.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wd.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ag.gzmigu.cn

Go:   defer f.Close()
来源：http://jf.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ru.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wj.lnxyls.cn

================================================================================
来源：http://uv.haigaiapp.cn

I. 正则表达式
来源：http://bb.colortex.cn

================================================================================
来源：http://pa.shtwfgs.cn

[I01] 判断是否匹配
来源：http://cq.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kq.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ks.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://ar.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://cy.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zu.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mo.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://ie.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ua.gzmigu.cn

[I02] 提取所有匹配
来源：http://rx.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://vt.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://or.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://al.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://gf.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kd.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ax.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://xu.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oc.gzmigu.cn

[I03] 提取捕获分组
来源：http://qc.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ak.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bn.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gt.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qa.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jw.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pt.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zw.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vz.shxzskj.cn

[I04] 正则替换
来源：http://pj.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bl.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iq.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yd.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qo.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://od.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fb.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qs.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lz.huixiangedu.cn

[I05] 按正则拆分
来源：http://jr.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yk.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cs.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://mo.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://pc.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://cm.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ug.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bl.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jg.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rz.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sp.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uw.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://he.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hy.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dv.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ln.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fh.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rw.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://vo.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ie.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bc.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://km.shxzukj.cn

TS:   /error/gim
来源：http://hr.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ga.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vr.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://ml.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ae.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://vv.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iv.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mb.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sm.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gv.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fu.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ay.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dw.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sl.hahajie.cn

================================================================================
来源：http://ov.panjiajie.cn

J. 日期与时间
来源：http://ak.colortex.cn

================================================================================
来源：http://jb.yuexingan06.cn

[J01] 获取当前时间
来源：http://rt.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uo.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ne.colortex.cn

JS:   new Date();  Date.now()
来源：http://ey.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://cr.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wi.huixinmuqiang.cn

Go:   time.Now()
来源：http://wg.nicolike.cn

Ruby: Time.now
来源：http://zg.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://am.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ia.newstarts.cn


<!-- 参考信息 -->