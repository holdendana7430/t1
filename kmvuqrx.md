代发 wailian999

Py:   class Admin(User): pass
来源：http://tl.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://ck.shxzskj.cn

JS:   class Admin extends User {}
来源：http://bt.szsharing.cn

TS:   class Admin extends User {}
来源：http://eh.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://wo.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ud.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://ke.lnxyls.cn

C#:   class Admin : User {}
来源：http://uw.huixinmuqiang.cn

[G06] 重写方法
来源：http://bq.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://nz.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ah.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://ac.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://ge.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://iv.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ly.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://yk.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://cr.szsharing.cn

[G07] 调用父类方法
来源：http://bh.bookmarksfly.cn

Py:   super().greet()
来源：http://ew.huanxung.cn

PHP:  parent::greet();
来源：http://kq.hahajie.cn

JS:   super.greet();
来源：http://dl.haigaiapp.cn

TS:   super.greet();
来源：http://vb.szsharing.cn

Java: super.greet();
来源：http://xz.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ir.jctech888.com.cn

Ruby: super
来源：http://ea.9csxet.cn

C#:   base.Greet();
来源：http://be.9csxet.cn

[G08] 静态方法与属性
来源：http://fn.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ei.szxytkj.cn

PHP:  public static function f() {}
来源：http://oi.jctech888.com.cn

JS:   static f() {}
来源：http://kq.jctech888.com.cn

TS:   static f(): void {}
来源：http://yp.szxytkj.cn

Java: static void f() {}
来源：http://hm.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lw.hnjuh.cn

Ruby: def self.f; end
来源：http://if.hahajie.cn

C#:   public static void F() {}
来源：http://ko.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ao.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://rd.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wp.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ca.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://wh.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://nw.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://hl.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zp.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://xo.9csxet.cn

[G10] 访问控制
来源：http://pt.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ie.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://ib.newstarts.cn

JS:   #private 字段；其余公开
来源：http://ya.gzmigu.cn

TS:   public / protected / private
来源：http://jw.asd995.cn

Java: public / protected / private / 默认包级
来源：http://ov.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vw.yuexingan06.cn

Ruby: public / protected / private
来源：http://wt.hnjuh.cn

C#:   public / protected / private / internal
来源：http://dz.9csxet.cn

[G11] getter / setter
来源：http://ic.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://yv.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mj.szsharing.cn

JS:   get name() { return this._name; }
来源：http://vl.521024.cn

TS:   get name(): string { return this._name; }
来源：http://ju.asd995.cn

Java: public String getName() { return name; }
来源：http://wr.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ow.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://ni.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://yb.yuexingan06.cn

[G12] 对象转字符串
来源：http://dg.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://ix.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jh.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://hr.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://al.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://zr.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eq.asd995.cn

Ruby: def to_s; @name; end
来源：http://aa.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://rl.haigaiapp.cn

[G13] 判断对象类型
来源：http://it.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://fo.muxihuayi.cn

PHP:  $u instanceof User
来源：http://no.wgjwhj.cn

JS:   u instanceof User
来源：http://nn.jctech888.com.cn

TS:   u instanceof User
来源：http://xz.jctech888.com.cn

Java: u instanceof User
来源：http://ab.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nw.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://au.haigaiapp.cn

C#:   u is User
来源：http://ud.nszjky.cn

[G14] 数据类 / record
来源：http://qx.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ev.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://ry.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bj.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://cq.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://kk.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://ph.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ok.colortex.cn

C#:   record User(string Name, int Age);
来源：http://xo.shtwfgs.cn

[G15] 枚举
来源：http://nz.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jq.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jc.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fa.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xu.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://gp.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hk.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ab.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bi.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://vd.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tb.521024.cn

PHP:  get_object_vars($obj);
来源：http://eu.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://ur.shxzukj.cn

TS:   Object.entries(obj)
来源：http://qz.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://du.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bd.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://hj.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://ey.haigaiapp.cn

================================================================================
来源：http://rh.bjjhwx.cn

H. 异常与错误处理
来源：http://yy.jctech888.com.cn

================================================================================
来源：http://fc.panjiajie.cn

[H01] try / catch 基础
来源：http://ss.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jo.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ps.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oy.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nr.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cs.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://il.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bf.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lo.asd995.cn

[H02] finally / ensure 收尾
来源：http://dk.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ys.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jm.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hv.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pn.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jj.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cx.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jf.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yy.shtwfgs.cn

[H03] 主动抛出异常
来源：http://cy.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://uw.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jx.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://bs.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ni.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bt.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zz.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vo.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ej.szxytkj.cn

[H04] 自定义异常类型
来源：http://uk.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://un.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ni.nszjky.cn

JS:   class MyError extends Error {}
来源：http://xs.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://wz.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://qn.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fa.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://ab.huanxung.cn

C#:   class MyException : Exception {}
来源：http://th.asd995.cn

[H05] 捕获特定类型
来源：http://rb.jctech888.com.cn

Py:   except ValueError as e:
来源：http://oe.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://of.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://oa.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://pu.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://ke.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lb.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://bg.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://il.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://tl.szsharing.cn

Py:   value = d.get("k") or default
来源：http://ej.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ct.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kf.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wd.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wj.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wy.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://zu.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://ua.chemitech.net.cn

[H07] 断言
来源：http://th.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://kt.szxytkj.cn

PHP:  assert($x > 0);
来源：http://tq.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://ag.nicolike.cn

TS:   console.assert(x > 0);
来源：http://pk.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://ro.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uf.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yw.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://ge.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://ce.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://rt.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wh.nszjky.cn

JS:   e.message;  e.stack
来源：http://fp.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://px.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hu.bookmarksfly.cn

Go:   err.Error()
来源：http://vw.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://ip.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://lb.huanxung.cn

[H09] 带错误码的异常
来源：http://yq.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://df.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kx.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dh.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ws.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fd.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mp.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ic.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hk.521024.cn

[H10] 资源自动释放
来源：http://ev.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gr.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sk.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wv.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mp.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uy.hahajie.cn

Go:   defer f.Close()
来源：http://pd.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pe.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wh.haigaiapp.cn

================================================================================
来源：http://nj.haigaiapp.cn

I. 正则表达式
来源：http://cy.yuexingan06.cn

================================================================================
来源：http://nt.521024.cn

[I01] 判断是否匹配
来源：http://ng.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mv.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lo.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://qd.asd995.cn

TS:   /\d+/.test(s)
来源：http://no.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ro.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sw.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://ms.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ly.szsharing.cn

[I02] 提取所有匹配
来源：http://ll.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://gn.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ue.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hp.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://ia.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ww.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kx.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://vd.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mx.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://az.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wj.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://di.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fl.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aj.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wy.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jm.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://od.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kc.newstarts.cn

[I04] 正则替换
来源：http://rb.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tz.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gb.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nr.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tf.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://io.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bz.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vr.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yk.shtwfgs.cn

[I05] 按正则拆分
来源：http://mr.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ri.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jq.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://vn.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://bi.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://mx.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hc.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ni.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jm.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ti.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ge.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oj.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://le.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://im.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fi.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yc.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zl.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hj.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://lf.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ic.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hp.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pw.muxihuayi.cn

TS:   /error/gim
来源：http://ma.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sy.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ef.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://ke.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://st.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://sb.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fc.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wh.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ps.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fw.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uc.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aq.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xl.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wh.huanxung.cn

================================================================================
来源：http://hg.nicolike.cn

J. 日期与时间
来源：http://uk.muxihuayi.cn

================================================================================
来源：http://rx.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://gt.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wu.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gu.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://qp.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://lx.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vj.bookmarksfly.cn

Go:   time.Now()
来源：http://ah.asd995.cn

Ruby: Time.now
来源：http://ga.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pw.nszjky.cn

[J02] 格式化输出
来源：http://oa.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://po.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ic.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ka.huixiangedu.cn

TS:   d.toISOString()
来源：http://io.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hx.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yf.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://te.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cs.panjiajie.cn

[J03] 字符串解析为日期
来源：http://jd.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://is.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fz.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://ry.huixinmuqiang.cn


<!-- 参考信息 -->