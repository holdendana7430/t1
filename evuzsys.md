代发 wailian999

Ruby: @name = "x"
来源：http://sl.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ru.asd995.cn

[G04] 定义方法
来源：http://ms.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://xy.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yo.9csxet.cn

JS:   greet() { return this.name; }
来源：http://yv.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://hs.521024.cn

Java: String greet() { return name; }
来源：http://lf.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nt.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://kp.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://ff.huixinmuqiang.cn

[G05] 继承
来源：http://io.newstarts.cn

Py:   class Admin(User): pass
来源：http://ws.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://iw.panjiajie.cn

JS:   class Admin extends User {}
来源：http://ed.shxzukj.cn

TS:   class Admin extends User {}
来源：http://hc.lnxyls.cn

Java: class Admin extends User {}
来源：http://ld.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ip.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://kt.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://pm.muxihuayi.cn

[G06] 重写方法
来源：http://pn.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://gw.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wc.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://nz.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ot.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://xe.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://we.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://qp.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://hy.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://bq.9csxet.cn

Py:   super().greet()
来源：http://ct.shxzskj.cn

PHP:  parent::greet();
来源：http://yr.haigaiapp.cn

JS:   super.greet();
来源：http://ap.shxzskj.cn

TS:   super.greet();
来源：http://yu.muxihuayi.cn

Java: super.greet();
来源：http://ve.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ys.szsharing.cn

Ruby: super
来源：http://ez.shxzskj.cn

C#:   base.Greet();
来源：http://pf.nszjky.cn

[G08] 静态方法与属性
来源：http://bs.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vw.muxihuayi.cn

PHP:  public static function f() {}
来源：http://dn.panjiajie.cn

JS:   static f() {}
来源：http://xb.nszjky.cn

TS:   static f(): void {}
来源：http://sv.shxzukj.cn

Java: static void f() {}
来源：http://bt.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dk.szsharing.cn

Ruby: def self.f; end
来源：http://sf.521024.cn

C#:   public static void F() {}
来源：http://fe.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://rq.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://au.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zu.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fx.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://ln.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://zj.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://tu.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xy.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://gy.newstarts.cn

[G10] 访问控制
来源：http://wn.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://jm.szsharing.cn

PHP:  public / protected / private
来源：http://id.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://my.shtwfgs.cn

TS:   public / protected / private
来源：http://iy.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://js.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hy.newstarts.cn

Ruby: public / protected / private
来源：http://iq.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://bq.jianghongdianzi.cn

[G11] getter / setter
来源：http://ux.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://hm.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yr.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://kz.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://sp.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://qp.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ak.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://ga.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ql.nszjky.cn

[G12] 对象转字符串
来源：http://vx.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://iy.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xn.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://ed.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://aq.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://zj.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uy.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://gh.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://lu.panjiajie.cn

[G13] 判断对象类型
来源：http://he.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://un.szxytkj.cn

PHP:  $u instanceof User
来源：http://aw.muxihuayi.cn

JS:   u instanceof User
来源：http://hk.nszjky.cn

TS:   u instanceof User
来源：http://ur.shxzukj.cn

Java: u instanceof User
来源：http://ch.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wi.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://sb.yuntaijiaju.cn

C#:   u is User
来源：http://vj.wgjwhj.cn

[G14] 数据类 / record
来源：http://kt.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sw.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://wq.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://id.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://wp.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://ax.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://nv.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cu.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://md.nicolike.cn

[G15] 枚举
来源：http://la.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lx.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dw.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nt.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://do.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://xh.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jz.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://lk.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ud.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://lj.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fc.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ul.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://fu.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://ox.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jw.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oq.9csxet.cn

Ruby: obj.instance_variables
来源：http://pp.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://kd.haigaiapp.cn

================================================================================
来源：http://hv.szxytkj.cn

H. 异常与错误处理
来源：http://il.9csxet.cn

================================================================================
来源：http://yk.shxzukj.cn

[H01] try / catch 基础
来源：http://ol.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pc.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wr.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dt.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fj.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gx.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xc.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ob.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ap.asd995.cn

[H02] finally / ensure 收尾
来源：http://zr.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://th.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zn.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zm.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tz.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ji.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ou.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ms.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kn.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://cu.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://wi.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rh.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://pe.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://up.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wp.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kc.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gu.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hg.jctech888.com.cn

[H04] 自定义异常类型
来源：http://vk.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://no.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yb.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://ys.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://ft.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://hl.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vl.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://pv.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://bo.9csxet.cn

[H05] 捕获特定类型
来源：http://dy.huanxung.cn

Py:   except ValueError as e:
来源：http://qs.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hb.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://tc.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://zn.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://ez.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ns.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://rt.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ik.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://qu.521024.cn

Py:   value = d.get("k") or default
来源：http://gf.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iq.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://re.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sb.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ga.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kp.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://ep.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://fu.asd995.cn

[H07] 断言
来源：http://hv.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://ui.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://fs.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://xw.szsharing.cn

TS:   console.assert(x > 0);
来源：http://wi.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://wk.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://df.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zu.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://le.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://gt.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://yj.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dg.newstarts.cn

JS:   e.message;  e.stack
来源：http://hv.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gw.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qw.521024.cn

Go:   err.Error()
来源：http://fx.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://xn.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://se.shxzskj.cn

[H09] 带错误码的异常
来源：http://xc.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tk.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ah.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ab.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eb.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hb.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vh.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ir.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lm.jctech888.com.cn

[H10] 资源自动释放
来源：http://xh.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ol.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://df.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qj.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wc.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wj.lnxyls.cn

Go:   defer f.Close()
来源：http://zd.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yf.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dc.muxihuayi.cn

================================================================================
来源：http://mv.szxytkj.cn

I. 正则表达式
来源：http://uv.521024.cn

================================================================================
来源：http://rl.lnxyls.cn

[I01] 判断是否匹配
来源：http://wr.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mo.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dm.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://uy.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://eo.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mz.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ii.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://dm.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ah.nszjky.cn

[I02] 提取所有匹配
来源：http://dj.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://xe.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zb.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ah.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://dj.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nd.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lg.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://rr.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gb.panjiajie.cn

[I03] 提取捕获分组
来源：http://ea.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ec.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tg.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mk.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nx.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fn.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ql.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eo.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yc.muxihuayi.cn

[I04] 正则替换
来源：http://vd.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lz.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kr.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kz.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oq.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cn.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ev.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ei.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kh.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://lb.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hl.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kd.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://hh.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://wc.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://wg.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yy.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rg.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qw.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ji.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qw.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hh.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rx.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://za.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lp.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gu.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://os.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wl.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://dc.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dn.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wn.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fv.colortex.cn

TS:   /error/gim
来源：http://ut.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jg.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yz.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://hn.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ce.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://wf.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oi.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://go.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dp.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bu.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hf.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://by.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pk.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://si.nicolike.cn

================================================================================
来源：http://hj.gzmigu.cn

J. 日期与时间
来源：http://fn.huanxung.cn

================================================================================
来源：http://tc.bookmarksfly.cn

[J01] 获取当前时间
来源：http://tp.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ob.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ya.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://bv.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://di.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ky.bookmarksfly.cn

Go:   time.Now()
来源：http://nj.muxihuayi.cn

Ruby: Time.now
来源：http://ew.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sd.huixiangedu.cn

[J02] 格式化输出
来源：http://nn.panjiajie.cn


<!-- 参考信息 -->