代发 wailian999

Ruby: super
来源：http://ri.szxytkj.cn

C#:   base.Greet();
来源：http://uf.hahajie.cn

[G08] 静态方法与属性
来源：http://cm.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sz.huixiangedu.cn

PHP:  public static function f() {}
来源：http://pi.szxytkj.cn

JS:   static f() {}
来源：http://ul.muxihuayi.cn

TS:   static f(): void {}
来源：http://nk.hnjuh.cn

Java: static void f() {}
来源：http://pw.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wc.asd995.cn

Ruby: def self.f; end
来源：http://jk.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://de.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://np.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://cm.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dc.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zw.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://cp.szsharing.cn

Java: interface Shape { double area(); }
来源：http://lk.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://ov.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rf.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://eq.lnxyls.cn

[G10] 访问控制
来源：http://up.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://qm.shtwfgs.cn

PHP:  public / protected / private
来源：http://za.nszjky.cn

JS:   #private 字段；其余公开
来源：http://vu.yuntaijiaju.cn

TS:   public / protected / private
来源：http://ru.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://nz.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lo.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://po.521024.cn

C#:   public / protected / private / internal
来源：http://sz.yuntaijiaju.cn

[G11] getter / setter
来源：http://ag.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://oy.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://is.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://bf.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://la.newstarts.cn

Java: public String getName() { return name; }
来源：http://ip.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sd.gzmigu.cn

Ruby: attr_accessor :name
来源：http://hg.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://hy.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://jn.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://vi.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xu.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://dr.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://qi.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://ad.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wa.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://ls.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://ar.panjiajie.cn

[G13] 判断对象类型
来源：http://lr.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://ar.nszjky.cn

PHP:  $u instanceof User
来源：http://vb.shtwfgs.cn

JS:   u instanceof User
来源：http://vw.hnjuh.cn

TS:   u instanceof User
来源：http://wm.wgjwhj.cn

Java: u instanceof User
来源：http://ft.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dv.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://fb.panjiajie.cn

C#:   u is User
来源：http://tp.panjiajie.cn

[G14] 数据类 / record
来源：http://um.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rt.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://kb.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://su.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://aq.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://pm.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://df.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lu.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://de.jianghongdianzi.cn

[G15] 枚举
来源：http://hr.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zc.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tm.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xs.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pe.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://iq.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mz.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://yg.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vh.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://ef.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dy.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://vj.nicolike.cn

JS:   Object.entries(obj)
来源：http://jw.521024.cn

TS:   Object.entries(obj)
来源：http://tm.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ou.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zf.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://ak.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://cs.jianghongdianzi.cn

================================================================================
来源：http://wp.9csxet.cn

H. 异常与错误处理
来源：http://yt.shxzukj.cn

================================================================================
来源：http://um.szsharing.cn

[H01] try / catch 基础
来源：http://pi.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hb.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://do.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qq.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wz.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ze.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ra.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://le.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jr.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://us.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://og.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lq.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yr.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ny.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qd.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kb.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://da.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ci.newstarts.cn

[H03] 主动抛出异常
来源：http://xn.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://sj.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cq.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://df.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://iw.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oo.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zt.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lp.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tq.yuexingan06.cn

[H04] 自定义异常类型
来源：http://tv.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://xw.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pv.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ab.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://tm.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://yu.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mg.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://gi.colortex.cn

C#:   class MyException : Exception {}
来源：http://jn.shxzskj.cn

[H05] 捕获特定类型
来源：http://am.szxytkj.cn

Py:   except ValueError as e:
来源：http://sq.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ed.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://om.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://zs.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://mg.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vr.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://uw.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cf.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://oa.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://gg.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zu.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zg.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eo.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yv.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zw.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://pg.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://kb.521024.cn

[H07] 断言
来源：http://wr.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://nz.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://my.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://qv.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://ls.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://xc.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rq.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xw.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://gb.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://ax.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://jy.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dx.szxytkj.cn

JS:   e.message;  e.stack
来源：http://lm.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pp.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fv.hahajie.cn

Go:   err.Error()
来源：http://lq.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://yc.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://ci.yuexingan06.cn

[H09] 带错误码的异常
来源：http://ml.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hv.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dx.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vx.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bo.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hp.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ds.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ij.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://id.521024.cn

[H10] 资源自动释放
来源：http://zy.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sa.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cm.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ir.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wp.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ud.szxytkj.cn

Go:   defer f.Close()
来源：http://wy.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tm.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jn.huanxung.cn

================================================================================
来源：http://qo.gzmigu.cn

I. 正则表达式
来源：http://vu.chemitech.net.cn

================================================================================
来源：http://rd.huanxung.cn

[I01] 判断是否匹配
来源：http://xz.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yc.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cb.9csxet.cn

JS:   /\d+/.test(s)
来源：http://ye.colortex.cn

TS:   /\d+/.test(s)
来源：http://iz.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xx.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ys.521024.cn

Ruby: s.match?(/\d+/)
来源：http://wp.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yv.wgjwhj.cn

[I02] 提取所有匹配
来源：http://uf.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://ew.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gt.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vz.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://lz.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jk.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ml.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ef.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fs.521024.cn

[I03] 提取捕获分组
来源：http://jo.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ns.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ct.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qy.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bx.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sa.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://he.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ll.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zr.szsharing.cn

[I04] 正则替换
来源：http://fy.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://es.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gy.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pv.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tr.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gm.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ni.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mg.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gy.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://fo.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xs.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://he.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://jf.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://me.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://uf.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bj.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wi.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pi.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fl.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ph.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xa.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xi.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fu.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://go.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qu.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ex.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ux.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://kd.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kg.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rd.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ll.huixiangedu.cn

TS:   /error/gim
来源：http://fo.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oh.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://no.521024.cn

Ruby: s.scan(/error/i)
来源：http://qz.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ry.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://cy.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uq.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fm.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://al.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://an.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uj.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wp.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lx.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mq.shxzukj.cn

================================================================================
来源：http://gu.bookmarksfly.cn

J. 日期与时间
来源：http://ln.huixiangedu.cn

================================================================================
来源：http://kc.hahajie.cn

[J01] 获取当前时间
来源：http://ah.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dt.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zb.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://eu.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://gf.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bu.nicolike.cn

Go:   time.Now()
来源：http://en.bjjhwx.cn

Ruby: Time.now
来源：http://iu.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nm.lnxyls.cn

[J02] 格式化输出
来源：http://gx.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ml.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zc.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bq.haigaiapp.cn

TS:   d.toISOString()
来源：http://kk.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ay.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://du.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gh.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ou.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://jv.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ki.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cx.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://ht.colortex.cn

TS:   new Date("2024-01-02")
来源：http://qg.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fw.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ua.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://aj.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ng.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ek.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gi.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sm.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xp.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://my.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://en.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://if.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://es.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zl.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://ni.asd995.cn

Py:   now + timedelta(days=7)
来源：http://yr.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kn.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bz.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oo.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://qf.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kh.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://pr.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fo.shxzukj.cn

[J06] 计算两时间之差
来源：http://pg.panjiajie.cn


<!-- 参考信息 -->