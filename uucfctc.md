代发 wailian999

JS:   super.greet();
来源：http://hq.yuexingan06.cn

TS:   super.greet();
来源：http://fh.hahajie.cn

Java: super.greet();
来源：http://lv.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xs.huixiangedu.cn

Ruby: super
来源：http://pb.huixinmuqiang.cn

C#:   base.Greet();
来源：http://yg.newstarts.cn

[G08] 静态方法与属性
来源：http://vd.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fj.colortex.cn

PHP:  public static function f() {}
来源：http://bn.hahajie.cn

JS:   static f() {}
来源：http://ca.shxzskj.cn

TS:   static f(): void {}
来源：http://xx.yuexingan06.cn

Java: static void f() {}
来源：http://pr.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pl.yuexingan06.cn

Ruby: def self.f; end
来源：http://os.szxytkj.cn

C#:   public static void F() {}
来源：http://oy.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://sz.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://rf.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gr.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://si.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://qj.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ty.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rh.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://vl.asd995.cn

[G10] 访问控制
来源：http://yc.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://mh.gzmigu.cn

PHP:  public / protected / private
来源：http://kn.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://gf.lnxyls.cn

TS:   public / protected / private
来源：http://sx.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://hb.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uw.shxzukj.cn

Ruby: public / protected / private
来源：http://xt.9csxet.cn

C#:   public / protected / private / internal
来源：http://xo.chemitech.net.cn

[G11] getter / setter
来源：http://bd.hahajie.cn

Py:   @property 与 @x.setter
来源：http://eo.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ew.nicolike.cn

JS:   get name() { return this._name; }
来源：http://zm.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://uw.shxzukj.cn

Java: public String getName() { return name; }
来源：http://cv.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mq.hahajie.cn

Ruby: attr_accessor :name
来源：http://wy.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://rg.bjjhwx.cn

[G12] 对象转字符串
来源：http://yg.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://zy.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zm.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://sl.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://dn.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://sj.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rt.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://im.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://zq.huanxung.cn

[G13] 判断对象类型
来源：http://qa.lnxyls.cn

Py:   isinstance(u, User)
来源：http://wf.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://dg.colortex.cn

JS:   u instanceof User
来源：http://cl.newstarts.cn

TS:   u instanceof User
来源：http://ui.yuexingan06.cn

Java: u instanceof User
来源：http://ou.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nd.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://rn.bookmarksfly.cn

C#:   u is User
来源：http://vf.nicolike.cn

[G14] 数据类 / record
来源：http://sr.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rr.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://df.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ir.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://mb.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://jx.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://hv.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://db.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://ol.lnxyls.cn

[G15] 枚举
来源：http://zs.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bd.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ym.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xu.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uj.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://xq.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fi.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://iy.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jh.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://fm.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yr.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://fp.521024.cn

JS:   Object.entries(obj)
来源：http://dv.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ja.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hj.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dc.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://dn.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://vd.panjiajie.cn

================================================================================
来源：http://qx.hnjuh.cn

H. 异常与错误处理
来源：http://yn.asd995.cn

================================================================================
来源：http://wv.panjiajie.cn

[H01] try / catch 基础
来源：http://hz.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://il.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://of.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bt.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rj.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wg.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ih.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sz.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ht.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://rc.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cn.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vw.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qw.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rg.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cu.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://he.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://to.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yp.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://ft.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://ad.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wu.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://yv.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://wb.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mb.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ob.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xl.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kp.muxihuayi.cn

[H04] 自定义异常类型
来源：http://tz.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://gh.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sc.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://it.9csxet.cn

TS:   class MyError extends Error {}
来源：http://uv.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://bh.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nb.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://ah.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://go.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://da.nszjky.cn

Py:   except ValueError as e:
来源：http://xx.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cz.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://eb.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://kr.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ed.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xu.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://uv.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cv.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://my.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://dd.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pd.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ma.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zb.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://if.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ey.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://qo.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://ii.yuexingan06.cn

[H07] 断言
来源：http://ul.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://wg.lnxyls.cn

PHP:  assert($x > 0);
来源：http://gr.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://fc.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://xn.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://ng.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sz.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qq.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://sz.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://wz.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://uv.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xo.shxzskj.cn

JS:   e.message;  e.stack
来源：http://it.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zh.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hx.szxytkj.cn

Go:   err.Error()
来源：http://xn.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://mg.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://bl.shxzskj.cn

[H09] 带错误码的异常
来源：http://ga.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ba.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ah.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pg.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ct.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lj.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vk.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uz.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zh.lnxyls.cn

[H10] 资源自动释放
来源：http://td.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bq.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nd.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lu.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ms.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vo.nszjky.cn

Go:   defer f.Close()
来源：http://wf.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bk.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ow.9csxet.cn

================================================================================
来源：http://po.chemitech.net.cn

I. 正则表达式
来源：http://fs.521024.cn

================================================================================
来源：http://hq.muxihuayi.cn

[I01] 判断是否匹配
来源：http://ey.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pc.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ee.newstarts.cn

JS:   /\d+/.test(s)
来源：http://rz.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://qt.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ao.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ew.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://zx.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://em.shxzskj.cn

[I02] 提取所有匹配
来源：http://jh.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://up.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xk.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nh.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://ym.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vv.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://in.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://zy.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vx.lnxyls.cn

[I03] 提取捕获分组
来源：http://qr.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vw.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qd.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rl.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oo.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wv.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sk.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zi.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xw.hahajie.cn

[I04] 正则替换
来源：http://et.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wa.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xk.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yw.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ob.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qf.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rh.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://id.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://im.shxzukj.cn

[I05] 按正则拆分
来源：http://ng.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wz.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lc.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://aa.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://og.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://kq.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bm.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wj.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wn.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wg.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tr.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qm.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mt.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ko.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ko.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yf.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jg.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dy.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://ca.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bm.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fy.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zw.colortex.cn

TS:   /error/gim
来源：http://mv.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ty.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ag.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://cb.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qq.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://qi.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sx.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zs.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://og.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tm.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lk.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wp.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xo.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cw.huixiangedu.cn

================================================================================
来源：http://ws.shxzukj.cn

J. 日期与时间
来源：http://zi.bjjhwx.cn

================================================================================
来源：http://bd.newstarts.cn

[J01] 获取当前时间
来源：http://qw.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rv.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://us.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://im.szsharing.cn

TS:   new Date();  Date.now()
来源：http://wr.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jb.521024.cn

Go:   time.Now()
来源：http://fv.wgjwhj.cn

Ruby: Time.now
来源：http://xq.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ya.nicolike.cn

[J02] 格式化输出
来源：http://ao.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://px.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ez.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pw.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://xm.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rb.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fh.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ps.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tf.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://lk.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hu.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hw.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://ky.asd995.cn

TS:   new Date("2024-01-02")
来源：http://do.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tj.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://he.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://sj.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yb.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://cw.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pw.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oy.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cv.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jy.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zr.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bc.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qs.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tv.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://gd.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://mm.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://er.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://da.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oy.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://qz.shtwfgs.cn


<!-- 参考信息 -->