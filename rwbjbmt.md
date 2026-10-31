代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://na.szsharing.cn

[G03] 实例属性
来源：http://iy.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://zr.colortex.cn

PHP:  public string $name = "x";
来源：http://tg.yuexingan06.cn

JS:   this.name = "x";
来源：http://ac.shxzukj.cn

TS:   name: string = "x";
来源：http://je.szsharing.cn

Java: private String name;
来源：http://yy.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://of.hahajie.cn

Ruby: @name = "x"
来源：http://xj.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://sx.yuexingan06.cn

[G04] 定义方法
来源：http://ue.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://ji.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lu.hahajie.cn

JS:   greet() { return this.name; }
来源：http://wj.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://fm.hahajie.cn

Java: String greet() { return name; }
来源：http://iv.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zi.nicolike.cn

Ruby: def greet; @name; end
来源：http://wn.newstarts.cn

C#:   public string Greet() => Name;
来源：http://oe.hnjuh.cn

[G05] 继承
来源：http://cw.asd995.cn

Py:   class Admin(User): pass
来源：http://yl.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://bc.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://gb.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://cs.lnxyls.cn

Java: class Admin extends User {}
来源：http://fg.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://od.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://bn.shxzukj.cn

C#:   class Admin : User {}
来源：http://im.hahajie.cn

[G06] 重写方法
来源：http://yc.521024.cn

Py:   def greet(self): return "admin"
来源：http://mq.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dj.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://rr.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://qs.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://pq.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://so.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://sm.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://bk.newstarts.cn

[G07] 调用父类方法
来源：http://he.yuntaijiaju.cn

Py:   super().greet()
来源：http://bw.panjiajie.cn

PHP:  parent::greet();
来源：http://je.huanxung.cn

JS:   super.greet();
来源：http://do.lnxyls.cn

TS:   super.greet();
来源：http://pi.shxzukj.cn

Java: super.greet();
来源：http://ak.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rg.huixiangedu.cn

Ruby: super
来源：http://rd.521024.cn

C#:   base.Greet();
来源：http://ik.nicolike.cn

[G08] 静态方法与属性
来源：http://jk.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://en.hnjuh.cn

PHP:  public static function f() {}
来源：http://sp.newstarts.cn

JS:   static f() {}
来源：http://mn.newstarts.cn

TS:   static f(): void {}
来源：http://fx.lnxyls.cn

Java: static void f() {}
来源：http://il.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xb.shtwfgs.cn

Ruby: def self.f; end
来源：http://zg.colortex.cn

C#:   public static void F() {}
来源：http://iw.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://xt.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://jo.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qd.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://af.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://cu.colortex.cn

Java: interface Shape { double area(); }
来源：http://uo.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://zh.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://of.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://ma.hnjuh.cn

[G10] 访问控制
来源：http://ga.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://bv.szxytkj.cn

PHP:  public / protected / private
来源：http://ft.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://zn.shtwfgs.cn

TS:   public / protected / private
来源：http://ps.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://oo.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://co.yuexingan06.cn

Ruby: public / protected / private
来源：http://mo.521024.cn

C#:   public / protected / private / internal
来源：http://ba.hnjuh.cn

[G11] getter / setter
来源：http://ep.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ws.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jh.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://tr.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://rc.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://kp.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ep.lnxyls.cn

Ruby: attr_accessor :name
来源：http://on.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://uq.521024.cn

[G12] 对象转字符串
来源：http://mh.asd995.cn

Py:   def __str__(self): return self.name
来源：http://vw.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://re.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://iy.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://gs.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://um.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pu.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://pl.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://hw.wgjwhj.cn

[G13] 判断对象类型
来源：http://ct.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://fq.muxihuayi.cn

PHP:  $u instanceof User
来源：http://my.yuexingan06.cn

JS:   u instanceof User
来源：http://tp.newstarts.cn

TS:   u instanceof User
来源：http://ks.muxihuayi.cn

Java: u instanceof User
来源：http://xl.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kf.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://yi.muxihuayi.cn

C#:   u is User
来源：http://az.jctech888.com.cn

[G14] 数据类 / record
来源：http://hi.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tw.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://jb.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://io.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://kg.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://pu.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://kl.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lo.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://ig.shtwfgs.cn

[G15] 枚举
来源：http://cf.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xk.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ww.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ap.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tn.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://mc.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ql.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://my.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://be.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://vf.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wn.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://zl.hnjuh.cn

JS:   Object.entries(obj)
来源：http://zu.nszjky.cn

TS:   Object.entries(obj)
来源：http://xh.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iy.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wy.asd995.cn

Ruby: obj.instance_variables
来源：http://nd.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://dm.hahajie.cn

================================================================================
来源：http://zd.haigaiapp.cn

H. 异常与错误处理
来源：http://qw.hahajie.cn

================================================================================
来源：http://qe.hnjuh.cn

[H01] try / catch 基础
来源：http://ty.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gp.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ju.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://df.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xj.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bu.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://re.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wo.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uz.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://cb.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gq.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qh.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://od.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fn.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rr.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qg.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wn.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gy.szxytkj.cn

[H03] 主动抛出异常
来源：http://qt.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://af.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ox.asd995.cn

JS:   throw new Error("错误信息");
来源：http://ia.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://qi.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xg.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lc.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lq.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cn.huanxung.cn

[H04] 自定义异常类型
来源：http://xq.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://yx.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ty.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://ek.nszjky.cn

TS:   class MyError extends Error {}
来源：http://ob.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://tx.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qb.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://hd.hahajie.cn

C#:   class MyException : Exception {}
来源：http://gx.bjjhwx.cn

[H05] 捕获特定类型
来源：http://kz.bjjhwx.cn

Py:   except ValueError as e:
来源：http://xv.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uu.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://lx.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://mt.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://pi.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://py.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://si.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rs.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://ig.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://ky.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cf.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ka.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rn.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ar.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cu.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://lp.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://hc.jctech888.com.cn

[H07] 断言
来源：http://rr.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ct.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://zc.colortex.cn

JS:   console.assert(x > 0);
来源：http://st.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://yf.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://ks.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://df.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://be.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://hm.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://es.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://qh.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ck.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ok.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://km.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sr.shxzukj.cn

Go:   err.Error()
来源：http://fh.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://yf.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://wt.jctech888.com.cn

[H09] 带错误码的异常
来源：http://up.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://da.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nz.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pk.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dd.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zp.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xl.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lb.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://it.colortex.cn

[H10] 资源自动释放
来源：http://vp.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oq.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jg.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bx.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gl.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fb.bjjhwx.cn

Go:   defer f.Close()
来源：http://fv.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kr.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hk.nszjky.cn

================================================================================
来源：http://ko.wgjwhj.cn

I. 正则表达式
来源：http://rz.nicolike.cn

================================================================================
来源：http://an.lnxyls.cn

[I01] 判断是否匹配
来源：http://qo.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://px.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ce.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://wu.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://iq.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fn.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uc.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://gs.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dj.colortex.cn

[I02] 提取所有匹配
来源：http://bs.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://vg.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hu.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://al.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://hq.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mg.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ek.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://cb.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://km.nszjky.cn

[I03] 提取捕获分组
来源：http://pj.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eu.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zk.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qn.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ca.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zq.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ge.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uq.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zm.hnjuh.cn

[I04] 正则替换
来源：http://wx.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ek.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fj.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wh.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xz.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ya.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vb.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://st.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bs.newstarts.cn

[I05] 按正则拆分
来源：http://rn.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rh.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yu.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ei.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://uc.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://qr.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yt.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yg.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bc.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ev.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qk.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jq.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dg.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lp.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uz.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fl.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ap.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gn.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://cx.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nv.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oc.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dn.bjjhwx.cn

TS:   /error/gim
来源：http://ea.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://af.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rf.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://jw.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ju.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://vy.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kr.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xf.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://in.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kn.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eg.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dz.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ch.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fb.muxihuayi.cn

================================================================================
来源：http://wy.asd995.cn

J. 日期与时间
来源：http://zn.bjjhwx.cn

================================================================================
来源：http://im.hnjuh.cn

[J01] 获取当前时间
来源：http://ed.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ub.muxihuayi.cn


<!-- 参考信息 -->