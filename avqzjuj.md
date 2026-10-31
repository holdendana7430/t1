代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://kx.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://ks.hahajie.cn

C#:   public string Greet() => Name;
来源：http://ow.muxihuayi.cn

[G05] 继承
来源：http://uh.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://no.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://ka.shxzukj.cn

JS:   class Admin extends User {}
来源：http://xy.gzmigu.cn

TS:   class Admin extends User {}
来源：http://nn.nicolike.cn

Java: class Admin extends User {}
来源：http://ve.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tx.9csxet.cn

Ruby: class Admin < User; end
来源：http://xs.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ub.yuntaijiaju.cn

[G06] 重写方法
来源：http://vn.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://zt.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://up.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://xr.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://kl.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://cb.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qa.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://ai.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://gy.szxytkj.cn

[G07] 调用父类方法
来源：http://rg.nszjky.cn

Py:   super().greet()
来源：http://hq.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://wd.huixiangedu.cn

JS:   super.greet();
来源：http://vw.bookmarksfly.cn

TS:   super.greet();
来源：http://to.9csxet.cn

Java: super.greet();
来源：http://wk.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bd.nicolike.cn

Ruby: super
来源：http://aa.szsharing.cn

C#:   base.Greet();
来源：http://pi.szxytkj.cn

[G08] 静态方法与属性
来源：http://kj.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zx.chemitech.net.cn

PHP:  public static function f() {}
来源：http://gd.chemitech.net.cn

JS:   static f() {}
来源：http://zi.lnxyls.cn

TS:   static f(): void {}
来源：http://ov.yuexingan06.cn

Java: static void f() {}
来源：http://lh.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nj.huixiangedu.cn

Ruby: def self.f; end
来源：http://yz.huixiangedu.cn

C#:   public static void F() {}
来源：http://cf.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://ra.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://mt.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xl.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jv.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://mu.9csxet.cn

Java: interface Shape { double area(); }
来源：http://jj.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://kr.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kw.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://hx.hahajie.cn

[G10] 访问控制
来源：http://gk.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://hv.wgjwhj.cn

PHP:  public / protected / private
来源：http://uk.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ga.szsharing.cn

TS:   public / protected / private
来源：http://cl.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://px.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ld.szxytkj.cn

Ruby: public / protected / private
来源：http://lc.gzmigu.cn

C#:   public / protected / private / internal
来源：http://wb.shtwfgs.cn

[G11] getter / setter
来源：http://nf.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://xh.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qp.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://ot.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://br.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://qz.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mp.asd995.cn

Ruby: attr_accessor :name
来源：http://be.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://wh.yuexingan06.cn

[G12] 对象转字符串
来源：http://oo.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://gr.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fu.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://yv.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://vo.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://jr.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gn.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://xs.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://uv.newstarts.cn

[G13] 判断对象类型
来源：http://ea.nicolike.cn

Py:   isinstance(u, User)
来源：http://xt.colortex.cn

PHP:  $u instanceof User
来源：http://nt.bjjhwx.cn

JS:   u instanceof User
来源：http://sg.newstarts.cn

TS:   u instanceof User
来源：http://rs.nicolike.cn

Java: u instanceof User
来源：http://lm.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rl.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://sd.jianghongdianzi.cn

C#:   u is User
来源：http://ll.9csxet.cn

[G14] 数据类 / record
来源：http://un.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jj.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://co.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kh.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://ol.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ce.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://ly.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://px.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://ec.chemitech.net.cn

[G15] 枚举
来源：http://dy.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hh.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://az.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hr.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zj.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://pf.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wu.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://dq.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kr.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://ws.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ws.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://el.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://ao.szsharing.cn

TS:   Object.entries(obj)
来源：http://yo.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lg.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ji.shxzukj.cn

Ruby: obj.instance_variables
来源：http://tu.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://td.wgjwhj.cn

================================================================================
来源：http://yh.wgjwhj.cn

H. 异常与错误处理
来源：http://xc.asd995.cn

================================================================================
来源：http://sa.gzmigu.cn

[H01] try / catch 基础
来源：http://ek.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mj.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qa.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kt.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ez.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tq.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aw.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kz.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://id.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://kb.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://km.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nw.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yf.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://du.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ub.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xe.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dl.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lv.nszjky.cn

[H03] 主动抛出异常
来源：http://md.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://iq.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ry.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://tc.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://vv.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xj.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fx.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vf.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bg.hahajie.cn

[H04] 自定义异常类型
来源：http://kq.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://ya.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nw.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://sp.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://hw.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://fh.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qw.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://ga.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://hp.shxzskj.cn

[H05] 捕获特定类型
来源：http://pl.haigaiapp.cn

Py:   except ValueError as e:
来源：http://yq.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nv.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://hi.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://xs.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://bf.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ef.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://bq.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tr.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://je.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://dx.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yw.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wp.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vf.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://if.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://py.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://av.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://gf.jianghongdianzi.cn

[H07] 断言
来源：http://fq.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://bg.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://ne.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://de.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://sv.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://zd.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pt.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ax.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://fr.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://cg.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://zl.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gq.hahajie.cn

JS:   e.message;  e.stack
来源：http://nh.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://au.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kt.colortex.cn

Go:   err.Error()
来源：http://qr.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://sa.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://gz.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://vs.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ah.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gj.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zq.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tn.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wf.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ye.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fa.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ws.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://cx.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nu.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ey.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sm.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lo.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fq.jctech888.com.cn

Go:   defer f.Close()
来源：http://kb.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ve.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pm.hnjuh.cn

================================================================================
来源：http://tq.nicolike.cn

I. 正则表达式
来源：http://fr.asd995.cn

================================================================================
来源：http://pc.yuexingan06.cn

[I01] 判断是否匹配
来源：http://np.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lb.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hh.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://vy.asd995.cn

TS:   /\d+/.test(s)
来源：http://we.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zo.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hr.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://ae.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ez.huixiangedu.cn

[I02] 提取所有匹配
来源：http://um.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://sc.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bt.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aq.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://kd.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zt.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://af.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://by.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rn.haigaiapp.cn

[I03] 提取捕获分组
来源：http://fc.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vu.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pe.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ju.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jv.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://np.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qz.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zl.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://la.bookmarksfly.cn

[I04] 正则替换
来源：http://rk.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gq.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://im.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gm.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sv.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vm.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bo.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zf.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jb.shxzskj.cn

[I05] 按正则拆分
来源：http://ae.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tv.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yq.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ot.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://vf.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://fh.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bh.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fu.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pf.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yo.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://in.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://as.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yi.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://in.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nf.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iz.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kq.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sd.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://ho.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ku.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tl.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://in.jctech888.com.cn

TS:   /error/gim
来源：http://ps.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://do.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://id.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://hn.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sd.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://rk.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bx.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zj.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yd.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uv.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bz.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nx.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iz.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zo.bookmarksfly.cn

================================================================================
来源：http://do.chemitech.net.cn

J. 日期与时间
来源：http://at.jianghongdianzi.cn

================================================================================
来源：http://pb.nicolike.cn

[J01] 获取当前时间
来源：http://fa.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xg.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wr.nicolike.cn

JS:   new Date();  Date.now()
来源：http://jt.521024.cn

TS:   new Date();  Date.now()
来源：http://yz.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ho.hahajie.cn

Go:   time.Now()
来源：http://zq.hnjuh.cn

Ruby: Time.now
来源：http://ip.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pv.hahajie.cn

[J02] 格式化输出
来源：http://gp.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nn.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://de.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jm.jctech888.com.cn

TS:   d.toISOString()
来源：http://gz.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ke.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wj.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tm.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hu.colortex.cn


<!-- 参考信息 -->