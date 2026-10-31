代发 wailian999

JS:   super.greet();
来源：http://ev.hnjuh.cn

TS:   super.greet();
来源：http://gt.newstarts.cn

Java: super.greet();
来源：http://qk.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gi.newstarts.cn

Ruby: super
来源：http://xt.521024.cn

C#:   base.Greet();
来源：http://ui.muxihuayi.cn

[G08] 静态方法与属性
来源：http://gr.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eg.huanxung.cn

PHP:  public static function f() {}
来源：http://cw.huixiangedu.cn

JS:   static f() {}
来源：http://fy.szxytkj.cn

TS:   static f(): void {}
来源：http://dw.yuexingan06.cn

Java: static void f() {}
来源：http://vo.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jw.chemitech.net.cn

Ruby: def self.f; end
来源：http://om.bjjhwx.cn

C#:   public static void F() {}
来源：http://ge.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://zk.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://vv.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dq.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ev.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://fc.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://dp.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://oi.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mm.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://gt.hnjuh.cn

[G10] 访问控制
来源：http://lt.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://cj.szsharing.cn

PHP:  public / protected / private
来源：http://jr.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://vh.shxzukj.cn

TS:   public / protected / private
来源：http://yt.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://py.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://le.jctech888.com.cn

Ruby: public / protected / private
来源：http://to.nicolike.cn

C#:   public / protected / private / internal
来源：http://ko.yuexingan06.cn

[G11] getter / setter
来源：http://en.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://by.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zm.asd995.cn

JS:   get name() { return this._name; }
来源：http://ps.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://lc.szsharing.cn

Java: public String getName() { return name; }
来源：http://ya.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rk.asd995.cn

Ruby: attr_accessor :name
来源：http://yf.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://hq.nszjky.cn

[G12] 对象转字符串
来源：http://ja.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://tr.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lj.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://du.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://kl.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://ko.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uz.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://ej.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://qw.shxzukj.cn

[G13] 判断对象类型
来源：http://ju.nicolike.cn

Py:   isinstance(u, User)
来源：http://nj.wgjwhj.cn

PHP:  $u instanceof User
来源：http://ox.colortex.cn

JS:   u instanceof User
来源：http://lr.lnxyls.cn

TS:   u instanceof User
来源：http://ab.nszjky.cn

Java: u instanceof User
来源：http://mb.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lf.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://aw.521024.cn

C#:   u is User
来源：http://he.newstarts.cn

[G14] 数据类 / record
来源：http://uw.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aq.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://si.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gg.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://hy.521024.cn

Java: record User(String name, int age) {}
来源：http://ar.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://nm.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://py.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://mv.bjjhwx.cn

[G15] 枚举
来源：http://pw.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zu.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://am.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bf.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sc.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://pv.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qe.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://vj.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ou.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://av.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://je.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://mu.szxytkj.cn

JS:   Object.entries(obj)
来源：http://xx.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://bf.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ih.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ol.szsharing.cn

Ruby: obj.instance_variables
来源：http://gf.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://bn.huixinmuqiang.cn

================================================================================
来源：http://nr.jianghongdianzi.cn

H. 异常与错误处理
来源：http://vy.shtwfgs.cn

================================================================================
来源：http://xb.521024.cn

[H01] try / catch 基础
来源：http://rw.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mb.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zz.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ux.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ga.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sh.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xd.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iv.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zy.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://ll.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zh.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ht.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uq.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ev.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pq.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gl.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vp.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lx.szsharing.cn

[H03] 主动抛出异常
来源：http://kr.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://xm.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cw.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://nq.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://jq.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wd.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sj.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ch.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://db.nicolike.cn

[H04] 自定义异常类型
来源：http://ap.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://zz.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yd.huanxung.cn

JS:   class MyError extends Error {}
来源：http://vz.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://il.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://xn.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ah.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://xc.szsharing.cn

C#:   class MyException : Exception {}
来源：http://bq.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://mq.nszjky.cn

Py:   except ValueError as e:
来源：http://eu.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eb.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://mu.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://ne.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://rh.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oe.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://ds.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pr.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://ge.colortex.cn

Py:   value = d.get("k") or default
来源：http://il.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vu.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ne.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nt.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ju.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dm.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://kf.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://nv.bjjhwx.cn

[H07] 断言
来源：http://nh.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://es.hahajie.cn

PHP:  assert($x > 0);
来源：http://vx.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://oa.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://ri.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://qr.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ig.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gz.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://sj.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://hz.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://rr.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://td.szsharing.cn

JS:   e.message;  e.stack
来源：http://on.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://za.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nh.hahajie.cn

Go:   err.Error()
来源：http://wp.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://vo.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://rv.wgjwhj.cn

[H09] 带错误码的异常
来源：http://zi.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://to.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jj.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aw.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yl.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kz.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ul.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ta.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cz.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://kn.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ct.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rd.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oh.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oj.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zr.hahajie.cn

Go:   defer f.Close()
来源：http://dc.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lp.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ut.jctech888.com.cn

================================================================================
来源：http://eb.shxzskj.cn

I. 正则表达式
来源：http://yf.chemitech.net.cn

================================================================================
来源：http://to.panjiajie.cn

[I01] 判断是否匹配
来源：http://he.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fj.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sa.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://ru.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://ry.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bq.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fp.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://eh.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fk.jctech888.com.cn

[I02] 提取所有匹配
来源：http://nj.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://yy.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vl.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rk.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://xf.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mg.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qh.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://tf.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zi.521024.cn

[I03] 提取捕获分组
来源：http://we.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oc.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ad.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ln.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yk.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rg.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wk.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cu.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vv.szxytkj.cn

[I04] 正则替换
来源：http://yk.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ok.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://er.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bl.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mt.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ms.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tc.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vj.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hu.haigaiapp.cn

[I05] 按正则拆分
来源：http://tt.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xh.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://er.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://bo.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://vd.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://yo.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rp.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zc.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xl.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gl.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xx.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jj.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nw.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ue.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ku.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kl.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://av.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tl.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://qf.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ml.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wa.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://az.9csxet.cn

TS:   /error/gim
来源：http://dd.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lo.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wr.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://eb.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ou.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://rh.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ne.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fm.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://di.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kg.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bo.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uc.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yv.muxihuayi.cn

================================================================================
来源：http://iw.hahajie.cn

J. 日期与时间
来源：http://xz.shtwfgs.cn

================================================================================
来源：http://il.gzmigu.cn

[J01] 获取当前时间
来源：http://md.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nu.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yj.hahajie.cn

JS:   new Date();  Date.now()
来源：http://eb.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://jz.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cm.bjjhwx.cn

Go:   time.Now()
来源：http://dl.muxihuayi.cn

Ruby: Time.now
来源：http://bv.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ce.yuexingan06.cn

[J02] 格式化输出
来源：http://zs.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://av.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://il.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hq.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://gj.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vp.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xn.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wm.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pb.szsharing.cn

[J03] 字符串解析为日期
来源：http://ua.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zr.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kq.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://qo.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://sh.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dy.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rg.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://kq.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ol.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://wx.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://em.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ix.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wb.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lv.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uo.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ol.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ht.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://za.521024.cn

[J05] 时间加减（加 7 天）
来源：http://yj.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://gq.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ns.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ul.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zv.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://gs.bjjhwx.cn


<!-- 参考信息 -->