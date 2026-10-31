代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://qf.panjiajie.cn

Ruby: def greet; @name; end
来源：http://vf.huanxung.cn

C#:   public string Greet() => Name;
来源：http://md.colortex.cn

[G05] 继承
来源：http://lm.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://hx.huanxung.cn

PHP:  class Admin extends User {}
来源：http://se.asd995.cn

JS:   class Admin extends User {}
来源：http://lk.hahajie.cn

TS:   class Admin extends User {}
来源：http://mb.shxzskj.cn

Java: class Admin extends User {}
来源：http://lc.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ci.nicolike.cn

Ruby: class Admin < User; end
来源：http://nt.shxzukj.cn

C#:   class Admin : User {}
来源：http://cx.newstarts.cn

[G06] 重写方法
来源：http://jz.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://gf.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ek.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://vx.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://cv.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://bp.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ae.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ab.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://pw.nicolike.cn

[G07] 调用父类方法
来源：http://av.hnjuh.cn

Py:   super().greet()
来源：http://ax.haigaiapp.cn

PHP:  parent::greet();
来源：http://uh.hnjuh.cn

JS:   super.greet();
来源：http://ev.shtwfgs.cn

TS:   super.greet();
来源：http://zk.huixiangedu.cn

Java: super.greet();
来源：http://af.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tg.szsharing.cn

Ruby: super
来源：http://mt.huanxung.cn

C#:   base.Greet();
来源：http://et.hahajie.cn

[G08] 静态方法与属性
来源：http://tx.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://np.szxytkj.cn

PHP:  public static function f() {}
来源：http://tv.bjjhwx.cn

JS:   static f() {}
来源：http://df.newstarts.cn

TS:   static f(): void {}
来源：http://uf.shxzukj.cn

Java: static void f() {}
来源：http://ap.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tb.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://sy.gzmigu.cn

C#:   public static void F() {}
来源：http://io.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://ma.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://ld.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aj.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tc.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://dz.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://np.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://yv.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ys.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://je.newstarts.cn

[G10] 访问控制
来源：http://qs.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://bv.bookmarksfly.cn

PHP:  public / protected / private
来源：http://ci.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://zf.szsharing.cn

TS:   public / protected / private
来源：http://rr.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://dq.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xu.bookmarksfly.cn

Ruby: public / protected / private
来源：http://om.9csxet.cn

C#:   public / protected / private / internal
来源：http://mh.bjjhwx.cn

[G11] getter / setter
来源：http://gh.521024.cn

Py:   @property 与 @x.setter
来源：http://qr.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jr.szsharing.cn

JS:   get name() { return this._name; }
来源：http://mx.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://gf.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://sq.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sg.521024.cn

Ruby: attr_accessor :name
来源：http://ag.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://yp.szsharing.cn

[G12] 对象转字符串
来源：http://hx.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://dx.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uk.asd995.cn

JS:   toString() { return this.name; }
来源：http://mc.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://em.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://rk.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gy.asd995.cn

Ruby: def to_s; @name; end
来源：http://sp.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://yk.bjjhwx.cn

[G13] 判断对象类型
来源：http://wz.hnjuh.cn

Py:   isinstance(u, User)
来源：http://zn.wgjwhj.cn

PHP:  $u instanceof User
来源：http://wa.haigaiapp.cn

JS:   u instanceof User
来源：http://ce.nicolike.cn

TS:   u instanceof User
来源：http://pv.panjiajie.cn

Java: u instanceof User
来源：http://gu.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cj.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://yk.chemitech.net.cn

C#:   u is User
来源：http://bl.newstarts.cn

[G14] 数据类 / record
来源：http://rk.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pg.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://uz.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://to.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://ab.szsharing.cn

Java: record User(String name, int age) {}
来源：http://li.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://vq.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tw.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://ua.hnjuh.cn

[G15] 枚举
来源：http://qn.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uz.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ud.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rz.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ql.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://sp.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pg.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://mk.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gn.colortex.cn

[G16] 对象转数组 / 字典
来源：http://om.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xj.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://yk.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://aw.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://ap.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zt.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yv.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://op.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ev.nszjky.cn

================================================================================
来源：http://bj.haigaiapp.cn

H. 异常与错误处理
来源：http://zg.colortex.cn

================================================================================
来源：http://ge.asd995.cn

[H01] try / catch 基础
来源：http://ur.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pv.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ll.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oy.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xa.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kj.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xa.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hn.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mp.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://pr.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xc.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zf.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://en.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xn.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sm.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qu.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tb.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ns.chemitech.net.cn

[H03] 主动抛出异常
来源：http://lg.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://kl.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iu.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://fy.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://sq.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://il.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dz.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pj.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rg.nszjky.cn

[H04] 自定义异常类型
来源：http://kp.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://xw.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://re.nicolike.cn

JS:   class MyError extends Error {}
来源：http://ux.nicolike.cn

TS:   class MyError extends Error {}
来源：http://lg.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://ue.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ff.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://gt.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://tm.9csxet.cn

[H05] 捕获特定类型
来源：http://vj.haigaiapp.cn

Py:   except ValueError as e:
来源：http://ce.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lx.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://sf.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://fw.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://sh.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ma.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://ib.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://po.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://iu.nszjky.cn

Py:   value = d.get("k") or default
来源：http://ab.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ws.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dn.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jr.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dl.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dk.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://tt.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://ch.nicolike.cn

[H07] 断言
来源：http://ou.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://ko.shxzukj.cn

PHP:  assert($x > 0);
来源：http://bs.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://vw.521024.cn

TS:   console.assert(x > 0);
来源：http://wk.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://bk.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pr.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ch.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://wh.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://ch.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://yx.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vd.nicolike.cn

JS:   e.message;  e.stack
来源：http://wo.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ft.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kn.huixinmuqiang.cn

Go:   err.Error()
来源：http://gn.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://xm.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://fj.chemitech.net.cn

[H09] 带错误码的异常
来源：http://as.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lm.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xd.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wk.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zd.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lb.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ok.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ha.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ph.chemitech.net.cn

[H10] 资源自动释放
来源：http://qs.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qt.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://re.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eo.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ph.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vb.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://ig.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ll.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oh.szsharing.cn

================================================================================
来源：http://gc.huixinmuqiang.cn

I. 正则表达式
来源：http://ea.shxzukj.cn

================================================================================
来源：http://gg.yuexingan06.cn

[I01] 判断是否匹配
来源：http://tv.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://or.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://he.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://hh.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://gk.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zn.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fj.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://ar.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ti.hahajie.cn

[I02] 提取所有匹配
来源：http://ag.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://lh.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pv.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ke.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://kd.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ug.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vt.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://ah.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vf.asd995.cn

[I03] 提取捕获分组
来源：http://gj.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aj.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zc.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vw.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eq.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://de.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ap.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ao.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nc.nicolike.cn

[I04] 正则替换
来源：http://ug.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gk.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dt.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nz.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dp.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xl.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yh.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fy.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pp.yuexingan06.cn

[I05] 按正则拆分
来源：http://ik.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yi.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ck.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://nk.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://aj.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://gi.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jn.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yq.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://by.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pf.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iz.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ox.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fr.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qc.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zd.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mt.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://an.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uv.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://si.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fv.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jl.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uk.yuexingan06.cn

TS:   /error/gim
来源：http://qk.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cz.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ke.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://zf.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bt.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://rn.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ua.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zc.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fe.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jb.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tt.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nk.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fk.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ls.yuntaijiaju.cn

================================================================================
来源：http://rn.newstarts.cn

J. 日期与时间
来源：http://no.huanxung.cn

================================================================================
来源：http://jn.huixiangedu.cn

[J01] 获取当前时间
来源：http://zm.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://no.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bw.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://vi.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://sg.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wo.shtwfgs.cn

Go:   time.Now()
来源：http://zk.newstarts.cn

Ruby: Time.now
来源：http://ef.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://as.jianghongdianzi.cn

[J02] 格式化输出
来源：http://ob.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pi.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kf.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cc.huanxung.cn

TS:   d.toISOString()
来源：http://yr.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qu.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ki.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ua.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ss.nicolike.cn


<!-- 参考信息 -->