代发 wailian999

PHP:  public static function f() {}
来源：http://ya.szsharing.cn

JS:   static f() {}
来源：http://dj.chemitech.net.cn

TS:   static f(): void {}
来源：http://yk.shtwfgs.cn

Java: static void f() {}
来源：http://un.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gu.bookmarksfly.cn

Ruby: def self.f; end
来源：http://zs.chemitech.net.cn

C#:   public static void F() {}
来源：http://md.521024.cn

[G09] 接口 / 抽象类
来源：http://qj.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ol.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uz.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://da.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://wn.colortex.cn

Java: interface Shape { double area(); }
来源：http://vz.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://fd.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://df.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://eo.gzmigu.cn

[G10] 访问控制
来源：http://fg.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://fk.szxytkj.cn

PHP:  public / protected / private
来源：http://my.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://sm.wgjwhj.cn

TS:   public / protected / private
来源：http://qi.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://oc.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sl.shtwfgs.cn

Ruby: public / protected / private
来源：http://vk.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://vg.asd995.cn

[G11] getter / setter
来源：http://ud.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://th.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://el.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://gi.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://cm.huanxung.cn

Java: public String getName() { return name; }
来源：http://el.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gd.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://yx.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ih.gzmigu.cn

[G12] 对象转字符串
来源：http://rj.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://ky.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xl.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://fj.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://ei.521024.cn

Java: @Override public String toString() { return name; }
来源：http://bc.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ab.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://dn.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://hu.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://zi.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://db.yuexingan06.cn

PHP:  $u instanceof User
来源：http://il.huixiangedu.cn

JS:   u instanceof User
来源：http://tr.haigaiapp.cn

TS:   u instanceof User
来源：http://ys.yuexingan06.cn

Java: u instanceof User
来源：http://bp.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cm.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://ok.nicolike.cn

C#:   u is User
来源：http://ys.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://ky.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gh.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://kg.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kt.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://sr.colortex.cn

Java: record User(String name, int age) {}
来源：http://oo.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://pt.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ul.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://pw.9csxet.cn

[G15] 枚举
来源：http://vt.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sg.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uu.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sn.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rq.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://ac.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zw.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://sd.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://ml.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bp.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://mt.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://zk.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://ww.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jf.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uj.shxzukj.cn

Ruby: obj.instance_variables
来源：http://sg.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://cm.bjjhwx.cn

================================================================================
来源：http://zn.521024.cn

H. 异常与错误处理
来源：http://cb.9csxet.cn

================================================================================
来源：http://gw.shxzukj.cn

[H01] try / catch 基础
来源：http://ga.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qj.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uj.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lg.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qa.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ux.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://of.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gb.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ce.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://xr.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cv.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ew.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mp.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ru.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ud.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tz.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mu.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xx.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://dx.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://ms.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zn.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://ki.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://cn.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dh.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vc.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sx.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mm.lnxyls.cn

[H04] 自定义异常类型
来源：http://zx.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://ff.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bv.szsharing.cn

JS:   class MyError extends Error {}
来源：http://gg.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://ky.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://ym.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://st.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://sv.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://ii.chemitech.net.cn

[H05] 捕获特定类型
来源：http://vp.shxzukj.cn

Py:   except ValueError as e:
来源：http://yu.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sd.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://nm.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://ai.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://pt.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lh.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://fq.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hq.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://ep.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://jl.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qe.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fm.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qp.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xm.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pn.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://wq.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://qa.newstarts.cn

[H07] 断言
来源：http://kp.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://ft.asd995.cn

PHP:  assert($x > 0);
来源：http://sg.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://og.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://dr.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://mw.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qm.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vn.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://ya.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://ka.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://mv.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wn.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://kf.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oa.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jm.bjjhwx.cn

Go:   err.Error()
来源：http://xz.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://sa.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://lu.hnjuh.cn

[H09] 带错误码的异常
来源：http://xo.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nq.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rb.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qa.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rq.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rf.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jk.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gg.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://re.shxzukj.cn

[H10] 资源自动释放
来源：http://sq.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nn.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zm.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bq.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yx.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qh.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://ok.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pk.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ci.shtwfgs.cn

================================================================================
来源：http://km.jianghongdianzi.cn

I. 正则表达式
来源：http://an.jctech888.com.cn

================================================================================
来源：http://ya.colortex.cn

[I01] 判断是否匹配
来源：http://mc.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ia.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ur.szsharing.cn

JS:   /\d+/.test(s)
来源：http://mj.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://cc.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lx.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tq.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://cl.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://am.panjiajie.cn

[I02] 提取所有匹配
来源：http://gp.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://yx.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mz.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sd.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://uw.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ew.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sz.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://up.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ml.muxihuayi.cn

[I03] 提取捕获分组
来源：http://yy.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vv.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gj.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ii.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tf.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wa.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tn.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ww.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bk.muxihuayi.cn

[I04] 正则替换
来源：http://wx.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sp.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vx.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://op.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lu.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://po.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vu.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wo.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yg.yuexingan06.cn

[I05] 按正则拆分
来源：http://qa.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hu.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sa.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://wt.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://qd.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://zz.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zd.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cf.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uq.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tm.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ur.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ph.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qy.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wr.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://og.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ur.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vw.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://io.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://fa.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ck.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zi.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pk.wgjwhj.cn

TS:   /error/gim
来源：http://wm.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fz.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rk.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://sq.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hx.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://bt.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://df.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://og.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xa.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hc.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mp.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fh.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://af.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ni.lnxyls.cn

================================================================================
来源：http://lo.gzmigu.cn

J. 日期与时间
来源：http://pd.lnxyls.cn

================================================================================
来源：http://eq.bookmarksfly.cn

[J01] 获取当前时间
来源：http://sq.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ia.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vr.9csxet.cn

JS:   new Date();  Date.now()
来源：http://sc.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://rc.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zl.huixiangedu.cn

Go:   time.Now()
来源：http://iy.panjiajie.cn

Ruby: Time.now
来源：http://ke.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kn.szxytkj.cn

[J02] 格式化输出
来源：http://lb.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://td.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vw.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pu.hnjuh.cn

TS:   d.toISOString()
来源：http://qd.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ch.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://di.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nu.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hc.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://ft.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://go.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://on.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://mx.colortex.cn

TS:   new Date("2024-01-02")
来源：http://zc.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bh.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oh.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ev.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xx.newstarts.cn

[J04] 时间戳与日期互转
来源：http://cr.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xb.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xh.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rg.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cu.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tj.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vl.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wi.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nx.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://gj.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://xw.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xb.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yi.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hq.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://jl.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://ne.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yw.huixiangedu.cn

[J06] 计算两时间之差
来源：http://xq.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://qj.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://ib.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vp.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kk.asd995.cn


<!-- 参考信息 -->