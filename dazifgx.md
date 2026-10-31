代发 wailian999

JS:   super.greet();
来源：http://ep.szxytkj.cn

TS:   super.greet();
来源：http://gi.muxihuayi.cn

Java: super.greet();
来源：http://xz.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ed.shtwfgs.cn

Ruby: super
来源：http://yw.shxzskj.cn

C#:   base.Greet();
来源：http://qt.colortex.cn

[G08] 静态方法与属性
来源：http://qt.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zk.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://zn.chemitech.net.cn

JS:   static f() {}
来源：http://ab.shxzukj.cn

TS:   static f(): void {}
来源：http://he.bjjhwx.cn

Java: static void f() {}
来源：http://eh.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wt.asd995.cn

Ruby: def self.f; end
来源：http://ie.nicolike.cn

C#:   public static void F() {}
来源：http://nu.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://ep.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://cc.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://px.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uh.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://go.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://xn.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://km.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://we.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://gl.nicolike.cn

[G10] 访问控制
来源：http://id.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://lg.huixiangedu.cn

PHP:  public / protected / private
来源：http://xb.nszjky.cn

JS:   #private 字段；其余公开
来源：http://lq.yuexingan06.cn

TS:   public / protected / private
来源：http://aa.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://cy.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ey.asd995.cn

Ruby: public / protected / private
来源：http://tp.szsharing.cn

C#:   public / protected / private / internal
来源：http://er.shxzskj.cn

[G11] getter / setter
来源：http://vd.nszjky.cn

Py:   @property 与 @x.setter
来源：http://zx.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cl.hahajie.cn

JS:   get name() { return this._name; }
来源：http://tz.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://qw.szxytkj.cn

Java: public String getName() { return name; }
来源：http://cc.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ux.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://tv.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://pm.nicolike.cn

[G12] 对象转字符串
来源：http://ke.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://mr.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lf.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://uq.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://iv.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://rv.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ka.521024.cn

Ruby: def to_s; @name; end
来源：http://jx.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://eh.521024.cn

[G13] 判断对象类型
来源：http://lo.panjiajie.cn

Py:   isinstance(u, User)
来源：http://fw.huixiangedu.cn

PHP:  $u instanceof User
来源：http://mc.panjiajie.cn

JS:   u instanceof User
来源：http://re.shtwfgs.cn

TS:   u instanceof User
来源：http://yd.chemitech.net.cn

Java: u instanceof User
来源：http://kv.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cn.9csxet.cn

Ruby: u.is_a?(User)
来源：http://cz.yuexingan06.cn

C#:   u is User
来源：http://mz.nszjky.cn

[G14] 数据类 / record
来源：http://li.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yz.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://yt.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jd.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://fu.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://hx.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://mu.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mp.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://gb.huixinmuqiang.cn

[G15] 枚举
来源：http://tq.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cu.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tc.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lc.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gw.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://qd.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sj.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://ri.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uu.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://ae.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yc.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://jx.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://hi.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://ho.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ol.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tv.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://ll.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ig.shtwfgs.cn

================================================================================
来源：http://tv.yuntaijiaju.cn

H. 异常与错误处理
来源：http://rg.huixiangedu.cn

================================================================================
来源：http://dt.shxzukj.cn

[H01] try / catch 基础
来源：http://cr.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://si.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qx.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zb.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oc.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://up.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lv.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bo.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yg.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://py.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fz.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kn.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ca.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ey.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://my.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ml.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zf.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nv.colortex.cn

[H03] 主动抛出异常
来源：http://hy.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://nw.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ew.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://kn.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://bf.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dr.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qy.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vf.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ud.asd995.cn

[H04] 自定义异常类型
来源：http://nl.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://jp.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mi.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://tt.szsharing.cn

TS:   class MyError extends Error {}
来源：http://cg.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://zv.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yz.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://an.521024.cn

C#:   class MyException : Exception {}
来源：http://gi.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://fu.gzmigu.cn

Py:   except ValueError as e:
来源：http://rt.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zv.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ma.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://dz.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://vn.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fr.521024.cn

Ruby: rescue ArgumentError => e
来源：http://kj.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bs.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://zv.asd995.cn

Py:   value = d.get("k") or default
来源：http://yp.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mf.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://if.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sm.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://he.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ae.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://pq.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://ye.shxzskj.cn

[H07] 断言
来源：http://xd.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://au.9csxet.cn

PHP:  assert($x > 0);
来源：http://vd.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://cn.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://wl.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://yd.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vn.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pf.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://iu.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://ws.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://yc.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://me.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://kq.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dj.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lc.bookmarksfly.cn

Go:   err.Error()
来源：http://or.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://kt.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://fv.haigaiapp.cn

[H09] 带错误码的异常
来源：http://cd.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ig.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rs.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aw.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zn.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xj.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fh.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://so.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tg.shxzskj.cn

[H10] 资源自动释放
来源：http://bs.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ho.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gs.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jl.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://re.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jv.wgjwhj.cn

Go:   defer f.Close()
来源：http://zp.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bc.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bu.huixiangedu.cn

================================================================================
来源：http://rc.haigaiapp.cn

I. 正则表达式
来源：http://wq.chemitech.net.cn

================================================================================
来源：http://fl.asd995.cn

[I01] 判断是否匹配
来源：http://dx.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rm.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://an.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://ug.huanxung.cn

TS:   /\d+/.test(s)
来源：http://xi.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dy.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rt.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://pf.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pf.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://lv.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://lx.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bl.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ht.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://kt.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nn.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ua.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://ve.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vl.9csxet.cn

[I03] 提取捕获分组
来源：http://pt.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wz.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://le.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ow.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sg.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://av.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ly.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lf.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fr.newstarts.cn

[I04] 正则替换
来源：http://dy.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://py.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yh.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://aa.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ap.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ex.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nf.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iy.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gq.9csxet.cn

[I05] 按正则拆分
来源：http://dq.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dn.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zu.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://xt.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://im.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://dw.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://so.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tm.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yz.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bi.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qu.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://af.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mq.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://su.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gr.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mu.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ze.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rm.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://as.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://az.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lh.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ht.nicolike.cn

TS:   /error/gim
来源：http://zv.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nf.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dj.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://mw.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dg.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://no.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pm.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tf.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zz.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gf.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lb.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sl.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jr.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ak.szxytkj.cn

================================================================================
来源：http://xg.gzmigu.cn

J. 日期与时间
来源：http://co.hahajie.cn

================================================================================
来源：http://pt.lnxyls.cn

[J01] 获取当前时间
来源：http://sc.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://or.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ni.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://tc.huanxung.cn

TS:   new Date();  Date.now()
来源：http://hq.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pp.jctech888.com.cn

Go:   time.Now()
来源：http://lh.szxytkj.cn

Ruby: Time.now
来源：http://gi.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ye.asd995.cn

[J02] 格式化输出
来源：http://xm.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uo.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lq.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qe.shtwfgs.cn

TS:   d.toISOString()
来源：http://ir.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yc.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lt.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sl.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://on.panjiajie.cn

[J03] 字符串解析为日期
来源：http://pa.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://au.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mu.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://xg.colortex.cn

TS:   new Date("2024-01-02")
来源：http://hl.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mk.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ru.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://pi.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zw.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://qz.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uc.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sj.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ym.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ob.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sq.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mv.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ii.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pv.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ky.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://go.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jq.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mp.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ct.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://nn.shxzskj.cn


<!-- 参考信息 -->