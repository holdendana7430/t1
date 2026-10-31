代发 wailian999

Ruby: @name = "x"
来源：http://pd.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://aq.szxytkj.cn

[G04] 定义方法
来源：http://sx.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://lr.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cw.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://mb.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://gj.muxihuayi.cn

Java: String greet() { return name; }
来源：http://ya.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fk.nszjky.cn

Ruby: def greet; @name; end
来源：http://lo.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://dp.9csxet.cn

[G05] 继承
来源：http://hc.521024.cn

Py:   class Admin(User): pass
来源：http://jd.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://ak.nicolike.cn

JS:   class Admin extends User {}
来源：http://ce.hahajie.cn

TS:   class Admin extends User {}
来源：http://ko.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://gv.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sq.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://ak.huanxung.cn

C#:   class Admin : User {}
来源：http://tx.huixiangedu.cn

[G06] 重写方法
来源：http://et.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://lw.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://go.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://va.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://kx.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://gy.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://by.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://wn.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://xv.gzmigu.cn

[G07] 调用父类方法
来源：http://cf.haigaiapp.cn

Py:   super().greet()
来源：http://dc.panjiajie.cn

PHP:  parent::greet();
来源：http://xi.hahajie.cn

JS:   super.greet();
来源：http://as.lnxyls.cn

TS:   super.greet();
来源：http://xl.colortex.cn

Java: super.greet();
来源：http://pi.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fi.bjjhwx.cn

Ruby: super
来源：http://nr.shxzskj.cn

C#:   base.Greet();
来源：http://qx.panjiajie.cn

[G08] 静态方法与属性
来源：http://lu.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ci.hnjuh.cn

PHP:  public static function f() {}
来源：http://sw.nszjky.cn

JS:   static f() {}
来源：http://mz.panjiajie.cn

TS:   static f(): void {}
来源：http://fm.shxzskj.cn

Java: static void f() {}
来源：http://cb.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sx.asd995.cn

Ruby: def self.f; end
来源：http://wm.haigaiapp.cn

C#:   public static void F() {}
来源：http://fo.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://uo.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://dp.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mq.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hs.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://bh.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://ej.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://mt.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fd.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://fq.asd995.cn

[G10] 访问控制
来源：http://nd.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://ys.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://um.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://ml.haigaiapp.cn

TS:   public / protected / private
来源：http://df.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://yk.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://go.szxytkj.cn

Ruby: public / protected / private
来源：http://pt.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://my.colortex.cn

[G11] getter / setter
来源：http://wu.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://hg.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bh.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://bc.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://rf.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://hl.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ka.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://fe.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://ku.9csxet.cn

[G12] 对象转字符串
来源：http://yd.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://xd.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oi.nszjky.cn

JS:   toString() { return this.name; }
来源：http://rt.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://ls.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://qt.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xd.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://km.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://fq.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://bp.panjiajie.cn

Py:   isinstance(u, User)
来源：http://ii.hahajie.cn

PHP:  $u instanceof User
来源：http://og.huanxung.cn

JS:   u instanceof User
来源：http://xd.huixiangedu.cn

TS:   u instanceof User
来源：http://ms.wgjwhj.cn

Java: u instanceof User
来源：http://cj.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://py.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://zm.jctech888.com.cn

C#:   u is User
来源：http://so.bookmarksfly.cn

[G14] 数据类 / record
来源：http://pt.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kz.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://hu.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tx.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://ep.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://fo.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://ha.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ux.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://vt.521024.cn

[G15] 枚举
来源：http://vx.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uz.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tz.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bd.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rh.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://so.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vt.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://zp.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ol.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://oj.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://de.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://xs.521024.cn

JS:   Object.entries(obj)
来源：http://cq.lnxyls.cn

TS:   Object.entries(obj)
来源：http://ub.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oq.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lj.szxytkj.cn

Ruby: obj.instance_variables
来源：http://pw.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://bk.huanxung.cn

================================================================================
来源：http://qa.huanxung.cn

H. 异常与错误处理
来源：http://nb.jianghongdianzi.cn

================================================================================
来源：http://ep.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://da.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qk.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vh.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vk.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hv.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nz.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pp.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xh.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rv.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://jf.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wr.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ba.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ks.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yy.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jg.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zu.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ql.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bd.yuexingan06.cn

[H03] 主动抛出异常
来源：http://dp.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://wv.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lo.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://oc.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://yk.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ma.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ql.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vx.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hc.jctech888.com.cn

[H04] 自定义异常类型
来源：http://ee.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://pp.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cn.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://yj.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://jm.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://ge.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vq.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://ps.asd995.cn

C#:   class MyException : Exception {}
来源：http://hg.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://yb.shtwfgs.cn

Py:   except ValueError as e:
来源：http://ab.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xx.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://de.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://ed.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://dr.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yj.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://zc.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dx.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://mu.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://us.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gf.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lw.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jg.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gb.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mc.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://cr.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://tj.bjjhwx.cn

[H07] 断言
来源：http://bt.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://va.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://ck.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://tz.hahajie.cn

TS:   console.assert(x > 0);
来源：http://lv.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://lr.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wc.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qr.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://by.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://mz.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://wd.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xe.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ad.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ez.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bj.chemitech.net.cn

Go:   err.Error()
来源：http://di.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ei.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://iy.huanxung.cn

[H09] 带错误码的异常
来源：http://yv.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kv.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ho.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qy.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vv.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ey.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vo.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gt.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uu.jctech888.com.cn

[H10] 资源自动释放
来源：http://vc.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wy.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bd.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xw.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://da.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://na.asd995.cn

Go:   defer f.Close()
来源：http://nd.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lm.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ax.lnxyls.cn

================================================================================
来源：http://aw.bookmarksfly.cn

I. 正则表达式
来源：http://ub.colortex.cn

================================================================================
来源：http://hx.521024.cn

[I01] 判断是否匹配
来源：http://st.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kg.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hw.hahajie.cn

JS:   /\d+/.test(s)
来源：http://sb.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://mj.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xx.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sd.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://vz.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://em.jctech888.com.cn

[I02] 提取所有匹配
来源：http://do.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://iq.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://as.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://la.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://ov.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nt.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://my.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://dn.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vc.9csxet.cn

[I03] 提取捕获分组
来源：http://tk.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hp.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ry.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gh.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ss.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://om.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ld.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wy.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tp.haigaiapp.cn

[I04] 正则替换
来源：http://dp.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gt.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yt.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qm.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wd.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ys.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xs.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xr.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sz.hnjuh.cn

[I05] 按正则拆分
来源：http://jv.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://du.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sl.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://jz.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://mt.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://by.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wy.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ti.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zr.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hk.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xd.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qv.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yv.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://br.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kl.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://od.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ms.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zs.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ry.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ln.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ns.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://so.yuntaijiaju.cn

TS:   /error/gim
来源：http://ii.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jr.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ce.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://se.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fi.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://cw.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ar.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zx.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kg.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ky.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bk.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://da.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ox.yuexingan06.cn

================================================================================
来源：http://sg.colortex.cn

J. 日期与时间
来源：http://sg.haigaiapp.cn

================================================================================
来源：http://ue.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://as.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://or.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ic.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ii.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://ro.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://la.shtwfgs.cn

Go:   time.Now()
来源：http://xi.huixinmuqiang.cn

Ruby: Time.now
来源：http://uu.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fz.521024.cn

[J02] 格式化输出
来源：http://xu.nicolike.cn


<!-- 参考信息 -->