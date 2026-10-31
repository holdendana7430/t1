代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://bn.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://kv.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://bw.hnjuh.cn

Java: String greet() { return name; }
来源：http://kx.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ej.asd995.cn

Ruby: def greet; @name; end
来源：http://ld.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://xy.bookmarksfly.cn

[G05] 继承
来源：http://lm.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://ks.asd995.cn

PHP:  class Admin extends User {}
来源：http://ae.asd995.cn

JS:   class Admin extends User {}
来源：http://qn.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://pp.muxihuayi.cn

Java: class Admin extends User {}
来源：http://mi.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rq.colortex.cn

Ruby: class Admin < User; end
来源：http://pw.shxzskj.cn

C#:   class Admin : User {}
来源：http://am.panjiajie.cn

[G06] 重写方法
来源：http://gn.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://kj.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ja.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://en.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://hr.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://xd.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hp.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://wc.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://zc.jctech888.com.cn

[G07] 调用父类方法
来源：http://il.nicolike.cn

Py:   super().greet()
来源：http://vk.muxihuayi.cn

PHP:  parent::greet();
来源：http://mj.colortex.cn

JS:   super.greet();
来源：http://as.hnjuh.cn

TS:   super.greet();
来源：http://up.huanxung.cn

Java: super.greet();
来源：http://tp.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rh.panjiajie.cn

Ruby: super
来源：http://tr.nicolike.cn

C#:   base.Greet();
来源：http://io.wgjwhj.cn

[G08] 静态方法与属性
来源：http://lm.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bh.yuexingan06.cn

PHP:  public static function f() {}
来源：http://vl.bjjhwx.cn

JS:   static f() {}
来源：http://ot.szxytkj.cn

TS:   static f(): void {}
来源：http://vr.huixiangedu.cn

Java: static void f() {}
来源：http://ln.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wx.jctech888.com.cn

Ruby: def self.f; end
来源：http://zs.muxihuayi.cn

C#:   public static void F() {}
来源：http://dq.huanxung.cn

[G09] 接口 / 抽象类
来源：http://jf.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://af.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qy.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lk.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://ld.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://ht.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://ce.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lu.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://if.hnjuh.cn

[G10] 访问控制
来源：http://oq.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://as.shtwfgs.cn

PHP:  public / protected / private
来源：http://be.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ks.haigaiapp.cn

TS:   public / protected / private
来源：http://vw.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://cn.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lq.huanxung.cn

Ruby: public / protected / private
来源：http://ug.szsharing.cn

C#:   public / protected / private / internal
来源：http://dz.521024.cn

[G11] getter / setter
来源：http://ut.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://dc.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mq.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://ax.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://uz.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://tu.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ba.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://xj.asd995.cn

C#:   public string Name { get; set; }
来源：http://rw.lnxyls.cn

[G12] 对象转字符串
来源：http://dl.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://ik.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yw.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://qi.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://fq.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://xo.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://er.szsharing.cn

Ruby: def to_s; @name; end
来源：http://am.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://il.hahajie.cn

[G13] 判断对象类型
来源：http://za.asd995.cn

Py:   isinstance(u, User)
来源：http://mi.muxihuayi.cn

PHP:  $u instanceof User
来源：http://kx.huixiangedu.cn

JS:   u instanceof User
来源：http://lf.shxzukj.cn

TS:   u instanceof User
来源：http://tv.newstarts.cn

Java: u instanceof User
来源：http://mn.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mo.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://cx.huanxung.cn

C#:   u is User
来源：http://qm.szxytkj.cn

[G14] 数据类 / record
来源：http://yt.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gb.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://zx.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ez.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://nx.asd995.cn

Java: record User(String name, int age) {}
来源：http://hn.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://hx.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ua.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://hz.nszjky.cn

[G15] 枚举
来源：http://hs.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lb.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vc.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oy.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ic.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://qr.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nm.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://bk.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sp.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://hl.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tm.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://zr.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://jf.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://yi.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wz.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://be.9csxet.cn

Ruby: obj.instance_variables
来源：http://nc.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://xc.chemitech.net.cn

================================================================================
来源：http://zh.haigaiapp.cn

H. 异常与错误处理
来源：http://kg.szxytkj.cn

================================================================================
来源：http://sf.bookmarksfly.cn

[H01] try / catch 基础
来源：http://er.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ze.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://df.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tq.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dd.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pk.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yd.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ez.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zi.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://xu.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ev.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kl.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://of.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jp.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ad.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pr.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gp.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ba.asd995.cn

[H03] 主动抛出异常
来源：http://lr.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://ws.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eu.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://rq.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://mr.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hk.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yb.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wq.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qd.panjiajie.cn

[H04] 自定义异常类型
来源：http://zk.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://qd.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pg.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://gh.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ht.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://sg.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qe.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://pe.szsharing.cn

C#:   class MyException : Exception {}
来源：http://gw.shxzskj.cn

[H05] 捕获特定类型
来源：http://xz.panjiajie.cn

Py:   except ValueError as e:
来源：http://rp.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ca.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://kw.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://vs.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://yd.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://of.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://uj.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hi.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://in.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://bh.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fc.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ol.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hr.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zn.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ot.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://pj.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://wc.hahajie.cn

[H07] 断言
来源：http://vb.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://wq.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://du.9csxet.cn

JS:   console.assert(x > 0);
来源：http://ox.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://mz.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://hb.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bb.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://km.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://iw.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://tq.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://us.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vh.gzmigu.cn

JS:   e.message;  e.stack
来源：http://cy.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ve.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vn.jctech888.com.cn

Go:   err.Error()
来源：http://fu.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://zq.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://kc.szsharing.cn

[H09] 带错误码的异常
来源：http://we.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zx.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ak.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ev.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://da.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sv.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qt.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aj.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rz.bjjhwx.cn

[H10] 资源自动释放
来源：http://qa.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qr.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ys.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hs.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bc.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ij.asd995.cn

Go:   defer f.Close()
来源：http://bi.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yj.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rh.muxihuayi.cn

================================================================================
来源：http://gr.jianghongdianzi.cn

I. 正则表达式
来源：http://wk.huanxung.cn

================================================================================
来源：http://fx.shtwfgs.cn

[I01] 判断是否匹配
来源：http://vp.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://us.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tk.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://ww.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://tn.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lf.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://by.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://yj.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mu.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://at.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://xu.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ou.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ni.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://ob.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tr.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://en.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://go.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qi.panjiajie.cn

[I03] 提取捕获分组
来源：http://pl.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jm.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ux.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kt.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hl.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sb.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rz.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qx.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wo.haigaiapp.cn

[I04] 正则替换
来源：http://zs.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://un.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bk.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xk.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pn.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jb.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hp.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ic.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cf.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://vn.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sd.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://td.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://en.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://er.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://mi.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xg.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xd.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ax.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://di.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ht.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rr.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rl.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rb.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://na.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://po.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xv.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://id.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://he.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rj.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bj.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ss.9csxet.cn

TS:   /error/gim
来源：http://wx.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bg.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kl.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://my.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://px.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://ke.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uk.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sp.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dp.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ft.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ib.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ne.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hm.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ba.nszjky.cn

================================================================================
来源：http://mv.haigaiapp.cn

J. 日期与时间
来源：http://uc.hahajie.cn

================================================================================
来源：http://hz.jctech888.com.cn

[J01] 获取当前时间
来源：http://wx.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wj.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lu.huanxung.cn

JS:   new Date();  Date.now()
来源：http://vs.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://gr.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://go.bookmarksfly.cn

Go:   time.Now()
来源：http://xt.huixiangedu.cn

Ruby: Time.now
来源：http://sf.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wf.shxzskj.cn

[J02] 格式化输出
来源：http://bl.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yx.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://em.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bg.lnxyls.cn

TS:   d.toISOString()
来源：http://vn.huixiangedu.cn


<!-- 参考信息 -->