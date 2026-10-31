代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://oz.gzmigu.cn

[G07] 调用父类方法
来源：http://eu.nszjky.cn

Py:   super().greet()
来源：http://la.haigaiapp.cn

PHP:  parent::greet();
来源：http://uz.lnxyls.cn

JS:   super.greet();
来源：http://xb.lnxyls.cn

TS:   super.greet();
来源：http://tb.haigaiapp.cn

Java: super.greet();
来源：http://po.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nn.huixinmuqiang.cn

Ruby: super
来源：http://wt.nicolike.cn

C#:   base.Greet();
来源：http://zf.shtwfgs.cn

[G08] 静态方法与属性
来源：http://jl.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zb.chemitech.net.cn

PHP:  public static function f() {}
来源：http://rp.hahajie.cn

JS:   static f() {}
来源：http://sl.gzmigu.cn

TS:   static f(): void {}
来源：http://xc.shxzskj.cn

Java: static void f() {}
来源：http://oe.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lz.shtwfgs.cn

Ruby: def self.f; end
来源：http://bn.szsharing.cn

C#:   public static void F() {}
来源：http://gu.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://bc.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://lh.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hw.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jl.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://dc.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://wa.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://zl.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ii.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://ha.shxzukj.cn

[G10] 访问控制
来源：http://ot.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://uy.gzmigu.cn

PHP:  public / protected / private
来源：http://rd.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://oe.lnxyls.cn

TS:   public / protected / private
来源：http://gm.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://ud.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gt.colortex.cn

Ruby: public / protected / private
来源：http://ym.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://cd.jctech888.com.cn

[G11] getter / setter
来源：http://zg.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://li.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ng.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://vx.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://gl.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://ug.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fg.hahajie.cn

Ruby: attr_accessor :name
来源：http://ho.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://zi.nicolike.cn

[G12] 对象转字符串
来源：http://pw.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://gy.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uq.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://da.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://fw.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://vd.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pg.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://rx.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://uh.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://jl.nicolike.cn

Py:   isinstance(u, User)
来源：http://qt.bjjhwx.cn

PHP:  $u instanceof User
来源：http://oz.chemitech.net.cn

JS:   u instanceof User
来源：http://hn.szsharing.cn

TS:   u instanceof User
来源：http://ac.bookmarksfly.cn

Java: u instanceof User
来源：http://gb.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pa.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://td.muxihuayi.cn

C#:   u is User
来源：http://fm.shxzskj.cn

[G14] 数据类 / record
来源：http://si.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rq.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://rt.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qh.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://lz.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://qa.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://fl.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tc.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://cn.yuexingan06.cn

[G15] 枚举
来源：http://sr.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sw.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jc.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qx.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lw.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://jb.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qi.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://et.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bo.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://fq.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yf.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://oc.9csxet.cn

JS:   Object.entries(obj)
来源：http://af.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://ba.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qu.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xf.9csxet.cn

Ruby: obj.instance_variables
来源：http://iy.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://xd.shxzskj.cn

================================================================================
来源：http://de.muxihuayi.cn

H. 异常与错误处理
来源：http://ho.521024.cn

================================================================================
来源：http://wj.bookmarksfly.cn

[H01] try / catch 基础
来源：http://fc.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://td.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ed.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uz.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pn.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ql.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lq.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gf.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wu.newstarts.cn

[H02] finally / ensure 收尾
来源：http://ow.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hp.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mw.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hs.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rb.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ug.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uo.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ln.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mv.shtwfgs.cn

[H03] 主动抛出异常
来源：http://fh.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://ff.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gf.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://gu.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://dl.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rl.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pw.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fi.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oq.lnxyls.cn

[H04] 自定义异常类型
来源：http://mj.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://mu.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xx.9csxet.cn

JS:   class MyError extends Error {}
来源：http://rz.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ks.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://wg.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://so.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://po.huanxung.cn

C#:   class MyException : Exception {}
来源：http://ez.colortex.cn

[H05] 捕获特定类型
来源：http://ki.hnjuh.cn

Py:   except ValueError as e:
来源：http://vt.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://an.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://gt.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://di.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://sp.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xa.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://tj.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bj.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ql.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://fc.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zm.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wj.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://we.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vp.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ok.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://yr.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://ek.szsharing.cn

[H07] 断言
来源：http://ax.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://zr.colortex.cn

PHP:  assert($x > 0);
来源：http://vp.nszjky.cn

JS:   console.assert(x > 0);
来源：http://tn.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://cf.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ce.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nz.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ku.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://sr.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://jz.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://nr.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pu.nicolike.cn

JS:   e.message;  e.stack
来源：http://sy.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qh.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eh.shtwfgs.cn

Go:   err.Error()
来源：http://hn.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://ao.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://no.shxzukj.cn

[H09] 带错误码的异常
来源：http://xl.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dw.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wx.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fw.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mx.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ev.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nc.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ff.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uf.muxihuayi.cn

[H10] 资源自动释放
来源：http://ih.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://do.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ei.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qn.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mc.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kc.bookmarksfly.cn

Go:   defer f.Close()
来源：http://ou.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xi.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zj.asd995.cn

================================================================================
来源：http://kx.bjjhwx.cn

I. 正则表达式
来源：http://ln.jctech888.com.cn

================================================================================
来源：http://lo.muxihuayi.cn

[I01] 判断是否匹配
来源：http://wb.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cu.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zb.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://zj.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://ka.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dn.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mj.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://ei.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fa.wgjwhj.cn

[I02] 提取所有匹配
来源：http://jb.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://lq.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vv.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uc.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://yd.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nc.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wh.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://mh.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hj.521024.cn

[I03] 提取捕获分组
来源：http://vj.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hq.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xc.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ml.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gx.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bf.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ei.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dt.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ai.chemitech.net.cn

[I04] 正则替换
来源：http://iu.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gz.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gy.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ys.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zp.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ln.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ks.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jv.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zb.newstarts.cn

[I05] 按正则拆分
来源：http://km.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wl.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mt.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://es.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://nq.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://ro.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rf.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hv.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oo.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wp.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ab.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nf.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cf.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bo.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oy.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rx.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sv.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zf.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://td.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hn.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jw.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hw.panjiajie.cn

TS:   /error/gim
来源：http://cu.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://et.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dc.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://yd.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dz.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://dj.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kl.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sh.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rd.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hd.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://se.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zp.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fx.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sm.jianghongdianzi.cn

================================================================================
来源：http://cg.yuntaijiaju.cn

J. 日期与时间
来源：http://yp.9csxet.cn

================================================================================
来源：http://pv.szxytkj.cn

[J01] 获取当前时间
来源：http://yq.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qo.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sj.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://ki.521024.cn

TS:   new Date();  Date.now()
来源：http://ef.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ff.szxytkj.cn

Go:   time.Now()
来源：http://nd.shxzukj.cn

Ruby: Time.now
来源：http://fr.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ho.shxzukj.cn

[J02] 格式化输出
来源：http://fa.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pm.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rv.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sj.nicolike.cn

TS:   d.toISOString()
来源：http://mp.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sy.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cl.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ou.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tg.gzmigu.cn

[J03] 字符串解析为日期
来源：http://nt.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pd.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vx.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://lr.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://hf.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lk.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jr.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://da.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mz.nicolike.cn

[J04] 时间戳与日期互转
来源：http://is.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ak.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ie.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fy.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xq.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sr.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nn.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ge.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jy.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://aq.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://mu.gzmigu.cn


<!-- 参考信息 -->