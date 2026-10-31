代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://vc.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ft.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rx.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://tq.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://dn.muxihuayi.cn

[G07] 调用父类方法
来源：http://os.bookmarksfly.cn

Py:   super().greet()
来源：http://pd.szsharing.cn

PHP:  parent::greet();
来源：http://qo.nszjky.cn

JS:   super.greet();
来源：http://rx.panjiajie.cn

TS:   super.greet();
来源：http://vx.haigaiapp.cn

Java: super.greet();
来源：http://zc.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nz.bookmarksfly.cn

Ruby: super
来源：http://vq.yuexingan06.cn

C#:   base.Greet();
来源：http://zd.jctech888.com.cn

[G08] 静态方法与属性
来源：http://jv.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wr.colortex.cn

PHP:  public static function f() {}
来源：http://by.521024.cn

JS:   static f() {}
来源：http://oo.gzmigu.cn

TS:   static f(): void {}
来源：http://jm.huanxung.cn

Java: static void f() {}
来源：http://as.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gh.521024.cn

Ruby: def self.f; end
来源：http://hl.nszjky.cn

C#:   public static void F() {}
来源：http://tx.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://ks.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://xo.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ba.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bn.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://vw.colortex.cn

Java: interface Shape { double area(); }
来源：http://cs.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://xa.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ap.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://hl.huanxung.cn

[G10] 访问控制
来源：http://hh.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://by.yuexingan06.cn

PHP:  public / protected / private
来源：http://zb.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://yc.yuntaijiaju.cn

TS:   public / protected / private
来源：http://qp.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://hk.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qg.jctech888.com.cn

Ruby: public / protected / private
来源：http://iq.huanxung.cn

C#:   public / protected / private / internal
来源：http://oo.panjiajie.cn

[G11] getter / setter
来源：http://my.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://nx.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pe.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://le.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://lz.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://rw.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rz.panjiajie.cn

Ruby: attr_accessor :name
来源：http://yu.asd995.cn

C#:   public string Name { get; set; }
来源：http://nq.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://sp.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://pu.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://as.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://rr.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://jf.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://tt.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zm.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://kq.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://tc.bookmarksfly.cn

[G13] 判断对象类型
来源：http://oh.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://gx.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://ds.521024.cn

JS:   u instanceof User
来源：http://mr.colortex.cn

TS:   u instanceof User
来源：http://jk.shxzukj.cn

Java: u instanceof User
来源：http://no.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yk.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://ex.shtwfgs.cn

C#:   u is User
来源：http://cs.asd995.cn

[G14] 数据类 / record
来源：http://gz.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qj.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://bg.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yt.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://gl.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://lk.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://wi.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yq.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://sc.jianghongdianzi.cn

[G15] 枚举
来源：http://na.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qj.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nr.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jg.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cv.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://he.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yk.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://gw.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vf.colortex.cn

[G16] 对象转数组 / 字典
来源：http://db.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dh.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://is.huanxung.cn

JS:   Object.entries(obj)
来源：http://vx.szsharing.cn

TS:   Object.entries(obj)
来源：http://os.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gh.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nu.9csxet.cn

Ruby: obj.instance_variables
来源：http://kc.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://gq.shxzukj.cn

================================================================================
来源：http://pd.szxytkj.cn

H. 异常与错误处理
来源：http://ln.newstarts.cn

================================================================================
来源：http://xb.muxihuayi.cn

[H01] try / catch 基础
来源：http://sl.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xf.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pr.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eq.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ca.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hl.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kz.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hn.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oi.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://qi.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xg.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xo.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jg.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tb.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hq.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gv.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oa.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lg.shxzukj.cn

[H03] 主动抛出异常
来源：http://ag.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://xx.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fl.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://lu.colortex.cn

TS:   throw new Error("错误信息");
来源：http://zv.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mp.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lu.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lk.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://co.newstarts.cn

[H04] 自定义异常类型
来源：http://ao.colortex.cn

Py:   class MyError(Exception): pass
来源：http://il.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qg.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://dw.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://dp.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://rz.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iz.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://cr.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://zo.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://vp.521024.cn

Py:   except ValueError as e:
来源：http://pv.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hs.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://hq.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://jp.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://ps.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dl.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://fo.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mo.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://ci.huanxung.cn

Py:   value = d.get("k") or default
来源：http://xl.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://my.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ds.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xy.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wp.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uh.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://hz.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://vz.huanxung.cn

[H07] 断言
来源：http://fd.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://yh.panjiajie.cn

PHP:  assert($x > 0);
来源：http://nj.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://sc.colortex.cn

TS:   console.assert(x > 0);
来源：http://zf.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://qh.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qr.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tx.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ie.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://to.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://sn.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gv.gzmigu.cn

JS:   e.message;  e.stack
来源：http://zh.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xd.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iw.nszjky.cn

Go:   err.Error()
来源：http://om.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ey.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://xf.panjiajie.cn

[H09] 带错误码的异常
来源：http://pi.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://az.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jz.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xi.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qo.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dn.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ko.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kd.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rt.hahajie.cn

[H10] 资源自动释放
来源：http://zz.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jb.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jx.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zk.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jm.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ad.muxihuayi.cn

Go:   defer f.Close()
来源：http://xd.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://az.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kp.huixiangedu.cn

================================================================================
来源：http://kg.haigaiapp.cn

I. 正则表达式
来源：http://ba.hahajie.cn

================================================================================
来源：http://ij.wgjwhj.cn

[I01] 判断是否匹配
来源：http://il.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ac.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sm.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://ll.colortex.cn

TS:   /\d+/.test(s)
来源：http://zf.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qn.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gf.521024.cn

Ruby: s.match?(/\d+/)
来源：http://ng.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lh.hnjuh.cn

[I02] 提取所有匹配
来源：http://xb.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://dj.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lc.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sw.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://ug.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sq.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vs.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://vb.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gk.nszjky.cn

[I03] 提取捕获分组
来源：http://bn.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sm.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zi.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lo.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hc.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jh.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://re.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tc.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ic.chemitech.net.cn

[I04] 正则替换
来源：http://do.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sp.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pv.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mk.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ry.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hx.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qe.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mp.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://om.lnxyls.cn

[I05] 按正则拆分
来源：http://kc.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://re.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xl.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://nt.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://eq.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://de.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lm.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yd.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lk.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ky.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dd.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ko.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nv.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iy.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rv.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ct.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ev.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://aw.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ip.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oq.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fc.9csxet.cn

TS:   /error/gim
来源：http://oz.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bm.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pu.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://ad.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dx.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://vn.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://on.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eu.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ol.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://np.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kz.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sl.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ji.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uz.lnxyls.cn

================================================================================
来源：http://ni.yuexingan06.cn

J. 日期与时间
来源：http://uj.jianghongdianzi.cn

================================================================================
来源：http://ya.newstarts.cn

[J01] 获取当前时间
来源：http://sz.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fd.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jf.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://rj.nicolike.cn

TS:   new Date();  Date.now()
来源：http://aa.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ly.shxzskj.cn

Go:   time.Now()
来源：http://xs.huixinmuqiang.cn

Ruby: Time.now
来源：http://bh.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hb.colortex.cn

[J02] 格式化输出
来源：http://df.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ym.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vd.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eg.muxihuayi.cn

TS:   d.toISOString()
来源：http://fj.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sl.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bu.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sg.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ci.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://cs.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yi.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pb.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://sh.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://uj.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jy.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://va.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://lc.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qp.9csxet.cn

[J04] 时间戳与日期互转
来源：http://jh.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rk.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mw.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vj.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kh.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://om.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uu.hahajie.cn


<!-- 参考信息 -->