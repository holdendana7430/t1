代发 wailian999

PHP:  public static function f() {}
来源：http://nr.chemitech.net.cn

JS:   static f() {}
来源：http://yy.haigaiapp.cn

TS:   static f(): void {}
来源：http://bv.shxzukj.cn

Java: static void f() {}
来源：http://jt.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yc.jctech888.com.cn

Ruby: def self.f; end
来源：http://ia.9csxet.cn

C#:   public static void F() {}
来源：http://yq.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://bp.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://hs.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yn.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tz.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://ns.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://ge.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ae.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dh.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://pe.shxzskj.cn

[G10] 访问控制
来源：http://cd.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://rq.hahajie.cn

PHP:  public / protected / private
来源：http://yq.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://bf.newstarts.cn

TS:   public / protected / private
来源：http://wt.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://ir.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sg.shtwfgs.cn

Ruby: public / protected / private
来源：http://hv.szsharing.cn

C#:   public / protected / private / internal
来源：http://mt.hnjuh.cn

[G11] getter / setter
来源：http://ch.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://bd.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fy.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://nt.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://mw.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://rs.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zg.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://nq.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://na.colortex.cn

[G12] 对象转字符串
来源：http://ra.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://tx.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://om.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://aq.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://tq.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://iy.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lx.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://ik.colortex.cn

C#:   public override string ToString() => Name;
来源：http://fl.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://qu.hnjuh.cn

Py:   isinstance(u, User)
来源：http://pf.newstarts.cn

PHP:  $u instanceof User
来源：http://gr.nicolike.cn

JS:   u instanceof User
来源：http://qc.gzmigu.cn

TS:   u instanceof User
来源：http://hb.shxzskj.cn

Java: u instanceof User
来源：http://pc.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ks.huanxung.cn

Ruby: u.is_a?(User)
来源：http://gx.shxzskj.cn

C#:   u is User
来源：http://bk.nszjky.cn

[G14] 数据类 / record
来源：http://oh.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ga.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://or.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ww.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://lm.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://uw.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://el.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xs.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://ec.nicolike.cn

[G15] 枚举
来源：http://yl.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jo.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ij.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ej.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ah.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://ll.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ek.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://cm.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ke.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://eo.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ai.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://dh.nicolike.cn

JS:   Object.entries(obj)
来源：http://ji.colortex.cn

TS:   Object.entries(obj)
来源：http://vx.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yx.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mb.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://yp.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ac.szxytkj.cn

================================================================================
来源：http://ci.9csxet.cn

H. 异常与错误处理
来源：http://fq.bjjhwx.cn

================================================================================
来源：http://na.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://rp.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mo.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tq.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ee.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dq.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dv.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lf.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://js.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://py.colortex.cn

[H02] finally / ensure 收尾
来源：http://os.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uu.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jd.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://up.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tw.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ea.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://en.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ha.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zb.szsharing.cn

[H03] 主动抛出异常
来源：http://fd.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://ju.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jn.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://pv.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://cy.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ht.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cd.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ad.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yr.shxzskj.cn

[H04] 自定义异常类型
来源：http://xn.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://do.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dl.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://mv.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://eg.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://py.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oz.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://jt.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://rt.huanxung.cn

[H05] 捕获特定类型
来源：http://am.shtwfgs.cn

Py:   except ValueError as e:
来源：http://hi.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sv.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ru.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://et.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://fz.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pa.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://ma.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ps.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://jy.nicolike.cn

Py:   value = d.get("k") or default
来源：http://da.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ee.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cb.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ji.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oc.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tr.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://gd.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://rm.chemitech.net.cn

[H07] 断言
来源：http://qg.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ua.shxzskj.cn

PHP:  assert($x > 0);
来源：http://wp.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://lf.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://gl.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://vi.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xc.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ey.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://fs.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://st.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://vi.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wy.lnxyls.cn

JS:   e.message;  e.stack
来源：http://ix.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jd.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dz.shtwfgs.cn

Go:   err.Error()
来源：http://qs.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://yd.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://dw.jctech888.com.cn

[H09] 带错误码的异常
来源：http://mx.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ce.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rp.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nu.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ke.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://er.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eq.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://aa.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yh.nszjky.cn

[H10] 资源自动释放
来源：http://gy.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yx.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ni.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zg.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xh.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sg.huixiangedu.cn

Go:   defer f.Close()
来源：http://hb.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fs.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iz.lnxyls.cn

================================================================================
来源：http://il.9csxet.cn

I. 正则表达式
来源：http://xj.lnxyls.cn

================================================================================
来源：http://ds.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://yk.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ih.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bx.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://gu.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://be.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fq.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zu.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://wx.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fr.shxzskj.cn

[I02] 提取所有匹配
来源：http://na.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://be.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://el.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xn.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://xk.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tc.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ag.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://zj.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lx.asd995.cn

[I03] 提取捕获分组
来源：http://bv.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iu.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jk.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xx.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yb.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fu.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hq.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xf.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://im.wgjwhj.cn

[I04] 正则替换
来源：http://mk.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fn.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hq.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uo.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sc.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ph.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tt.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hr.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sm.chemitech.net.cn

[I05] 按正则拆分
来源：http://wm.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yy.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cn.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://jt.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://hz.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://iw.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bi.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zt.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hm.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fg.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hl.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oa.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bb.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://od.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rj.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ry.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wp.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eq.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://xq.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wd.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ag.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://os.shxzskj.cn

TS:   /error/gim
来源：http://nm.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cv.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ka.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://gt.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wn.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://ra.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jh.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yf.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mw.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xt.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bg.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kv.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rh.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gk.szsharing.cn

================================================================================
来源：http://xc.shtwfgs.cn

J. 日期与时间
来源：http://hm.bjjhwx.cn

================================================================================
来源：http://jf.newstarts.cn

[J01] 获取当前时间
来源：http://wk.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tg.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xe.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://wg.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://hm.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ll.gzmigu.cn

Go:   time.Now()
来源：http://ut.nicolike.cn

Ruby: Time.now
来源：http://mo.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lj.haigaiapp.cn

[J02] 格式化输出
来源：http://pa.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://da.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dn.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ex.jctech888.com.cn

TS:   d.toISOString()
来源：http://xo.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gb.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sl.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ry.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xd.shxzukj.cn

[J03] 字符串解析为日期
来源：http://fh.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ip.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qf.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://fc.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://bi.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mg.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pu.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://ov.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nl.asd995.cn

[J04] 时间戳与日期互转
来源：http://pq.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zd.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://on.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ce.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qq.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wb.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bv.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kt.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zd.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://gg.521024.cn

Py:   now + timedelta(days=7)
来源：http://kc.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hj.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ix.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://so.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ft.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tm.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://lx.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fn.wgjwhj.cn

[J06] 计算两时间之差
来源：http://uq.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://oh.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://kp.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gc.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ib.huixinmuqiang.cn


<!-- 参考信息 -->