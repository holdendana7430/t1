代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://pe.jctech888.com.cn

Ruby: def self.f; end
来源：http://lp.hnjuh.cn

C#:   public static void F() {}
来源：http://ec.521024.cn

[G09] 接口 / 抽象类
来源：http://lq.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://yz.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://db.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yu.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://io.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://jy.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://he.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nx.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://eg.shtwfgs.cn

[G10] 访问控制
来源：http://hf.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://su.newstarts.cn

PHP:  public / protected / private
来源：http://wj.huanxung.cn

JS:   #private 字段；其余公开
来源：http://yw.nicolike.cn

TS:   public / protected / private
来源：http://vl.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://bo.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hg.521024.cn

Ruby: public / protected / private
来源：http://bg.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://tg.szsharing.cn

[G11] getter / setter
来源：http://hv.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://yi.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zc.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://pt.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://ff.521024.cn

Java: public String getName() { return name; }
来源：http://zi.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://va.nicolike.cn

Ruby: attr_accessor :name
来源：http://uw.hahajie.cn

C#:   public string Name { get; set; }
来源：http://ca.nszjky.cn

[G12] 对象转字符串
来源：http://ub.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://oy.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ol.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://oi.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://ey.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://lo.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sn.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://td.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://zl.szxytkj.cn

[G13] 判断对象类型
来源：http://al.huanxung.cn

Py:   isinstance(u, User)
来源：http://il.chemitech.net.cn

PHP:  $u instanceof User
来源：http://tp.szxytkj.cn

JS:   u instanceof User
来源：http://qt.colortex.cn

TS:   u instanceof User
来源：http://au.yuexingan06.cn

Java: u instanceof User
来源：http://st.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rb.huanxung.cn

Ruby: u.is_a?(User)
来源：http://fi.shtwfgs.cn

C#:   u is User
来源：http://rj.shtwfgs.cn

[G14] 数据类 / record
来源：http://pi.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ij.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://iz.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uz.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ea.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://gw.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://zp.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zj.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://jp.wgjwhj.cn

[G15] 枚举
来源：http://ka.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iu.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ck.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mq.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pd.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://ks.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yc.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://my.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vb.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://vu.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zu.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://re.gzmigu.cn

JS:   Object.entries(obj)
来源：http://xb.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://ax.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://af.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://en.szxytkj.cn

Ruby: obj.instance_variables
来源：http://js.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://gs.haigaiapp.cn

================================================================================
来源：http://of.hnjuh.cn

H. 异常与错误处理
来源：http://ia.bjjhwx.cn

================================================================================
来源：http://ou.nicolike.cn

[H01] try / catch 基础
来源：http://wj.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zq.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wa.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vu.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://df.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qa.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://br.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hc.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ex.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://am.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ti.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://me.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kw.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lo.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yo.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hh.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://le.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cj.szsharing.cn

[H03] 主动抛出异常
来源：http://ul.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://hv.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xa.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://fb.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://ln.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yv.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bg.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qg.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kd.muxihuayi.cn

[H04] 自定义异常类型
来源：http://eo.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://fe.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nv.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://sl.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://uo.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ul.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oz.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://rp.521024.cn

C#:   class MyException : Exception {}
来源：http://uj.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://aq.hahajie.cn

Py:   except ValueError as e:
来源：http://vg.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tp.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://lc.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://iv.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://vj.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pb.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://js.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vg.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://cv.huanxung.cn

Py:   value = d.get("k") or default
来源：http://xx.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://to.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wn.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eg.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yq.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jw.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://rs.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://wo.nszjky.cn

[H07] 断言
来源：http://ln.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://mp.9csxet.cn

PHP:  assert($x > 0);
来源：http://wb.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://ud.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://di.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://cr.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wk.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qu.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://bc.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://lm.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://wv.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://is.hnjuh.cn

JS:   e.message;  e.stack
来源：http://kk.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bb.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eg.huixinmuqiang.cn

Go:   err.Error()
来源：http://cf.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://du.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://ev.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://nh.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yz.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://us.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xc.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://in.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dw.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ql.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fd.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xy.9csxet.cn

[H10] 资源自动释放
来源：http://ga.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lz.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sv.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://he.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pn.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://to.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://sc.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uy.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kl.9csxet.cn

================================================================================
来源：http://pl.szxytkj.cn

I. 正则表达式
来源：http://jh.bjjhwx.cn

================================================================================
来源：http://yd.chemitech.net.cn

[I01] 判断是否匹配
来源：http://eh.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kh.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ql.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://kz.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://vi.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dh.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ae.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://mt.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://km.521024.cn

[I02] 提取所有匹配
来源：http://kr.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://pr.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://th.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://um.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://vi.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ek.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fy.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://gp.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zd.nszjky.cn

[I03] 提取捕获分组
来源：http://eg.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://av.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://er.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dn.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ve.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xy.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fp.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wf.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dq.shxzskj.cn

[I04] 正则替换
来源：http://cq.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hl.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rz.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ny.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tl.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tg.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jo.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tu.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bd.colortex.cn

[I05] 按正则拆分
来源：http://la.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kh.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wg.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://hx.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://hd.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://ag.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://re.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yg.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yw.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ql.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ru.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fq.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ap.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tj.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://up.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sn.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sl.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://az.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://om.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ci.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ei.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oo.panjiajie.cn

TS:   /error/gim
来源：http://ap.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zf.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bq.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://hf.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sf.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ne.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xh.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ce.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nr.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xu.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iz.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sh.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://es.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rv.hnjuh.cn

================================================================================
来源：http://px.yuexingan06.cn

J. 日期与时间
来源：http://ih.9csxet.cn

================================================================================
来源：http://vx.muxihuayi.cn

[J01] 获取当前时间
来源：http://sv.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ak.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://us.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://sk.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://oy.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ti.huixiangedu.cn

Go:   time.Now()
来源：http://ul.muxihuayi.cn

Ruby: Time.now
来源：http://ig.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://me.nszjky.cn

[J02] 格式化输出
来源：http://bf.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qn.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mb.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yu.shxzskj.cn

TS:   d.toISOString()
来源：http://br.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ai.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cb.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wn.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ka.asd995.cn

[J03] 字符串解析为日期
来源：http://lb.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bm.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lr.colortex.cn

JS:   new Date("2024-01-02")
来源：http://dm.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://cb.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vc.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ag.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://en.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wt.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://ed.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ai.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wn.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ei.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sk.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://af.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hq.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zn.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yf.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://ap.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://ky.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ne.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uy.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xc.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://cs.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aa.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://wn.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yp.521024.cn

[J06] 计算两时间之差
来源：http://pw.colortex.cn

Py:   (end - start).total_seconds()
来源：http://yz.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://ht.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ng.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jb.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jg.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://up.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://jk.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://xz.bjjhwx.cn


<!-- 参考信息 -->