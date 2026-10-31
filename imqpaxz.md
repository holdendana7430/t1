代发 wailian999

Java: interface Shape { double area(); }
来源：http://rz.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://xv.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tm.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://ky.muxihuayi.cn

[G10] 访问控制
来源：http://tp.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://sc.hnjuh.cn

PHP:  public / protected / private
来源：http://jg.nicolike.cn

JS:   #private 字段；其余公开
来源：http://ot.huixiangedu.cn

TS:   public / protected / private
来源：http://ar.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://uo.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://px.shtwfgs.cn

Ruby: public / protected / private
来源：http://hr.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://sy.nicolike.cn

[G11] getter / setter
来源：http://pg.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://jm.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qb.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://wl.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://ue.newstarts.cn

Java: public String getName() { return name; }
来源：http://kt.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fs.shxzskj.cn

Ruby: attr_accessor :name
来源：http://sz.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ok.yuexingan06.cn

[G12] 对象转字符串
来源：http://vr.colortex.cn

Py:   def __str__(self): return self.name
来源：http://nh.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ju.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://ku.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://zg.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://pl.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gy.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://et.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://zj.szsharing.cn

[G13] 判断对象类型
来源：http://mw.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://ui.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://nd.hnjuh.cn

JS:   u instanceof User
来源：http://il.hnjuh.cn

TS:   u instanceof User
来源：http://yx.521024.cn

Java: u instanceof User
来源：http://uv.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jw.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://ds.szxytkj.cn

C#:   u is User
来源：http://lj.521024.cn

[G14] 数据类 / record
来源：http://vq.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ns.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://ea.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cl.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://qy.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://eh.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://al.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vu.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://dc.shxzukj.cn

[G15] 枚举
来源：http://bq.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mg.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rn.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nq.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ov.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://qh.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vj.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://ac.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gi.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://wr.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vj.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://hh.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://td.nszjky.cn

TS:   Object.entries(obj)
来源：http://rc.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mn.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nr.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://vc.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ar.muxihuayi.cn

================================================================================
来源：http://fg.gzmigu.cn

H. 异常与错误处理
来源：http://vy.huixiangedu.cn

================================================================================
来源：http://yi.nicolike.cn

[H01] try / catch 基础
来源：http://rg.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kh.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uv.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qy.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://of.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yl.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nt.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ry.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ub.hahajie.cn

[H02] finally / ensure 收尾
来源：http://is.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pm.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wv.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lx.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sz.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vs.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ys.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mg.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oh.shxzukj.cn

[H03] 主动抛出异常
来源：http://pb.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://ex.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xa.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://gw.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://fa.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qx.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ta.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nz.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kv.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://ew.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://zf.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nk.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://qi.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://vy.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://il.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ep.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://rc.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://br.hnjuh.cn

[H05] 捕获特定类型
来源：http://ho.shtwfgs.cn

Py:   except ValueError as e:
来源：http://mt.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ht.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://tp.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://qs.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ew.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qn.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://qe.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://io.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://me.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://ib.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qh.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wx.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hg.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ut.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zd.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://ps.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://kt.szsharing.cn

[H07] 断言
来源：http://on.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ns.huanxung.cn

PHP:  assert($x > 0);
来源：http://tr.huanxung.cn

JS:   console.assert(x > 0);
来源：http://sd.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://yt.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://qa.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sf.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ss.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://bt.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://ff.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://lb.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rq.shxzukj.cn

JS:   e.message;  e.stack
来源：http://gp.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://an.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eq.asd995.cn

Go:   err.Error()
来源：http://wr.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://bt.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://nb.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://tz.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yk.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qr.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ft.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cf.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uj.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fv.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://in.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jk.haigaiapp.cn

[H10] 资源自动释放
来源：http://oo.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fo.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pp.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fn.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pe.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fk.panjiajie.cn

Go:   defer f.Close()
来源：http://yf.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bf.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sz.muxihuayi.cn

================================================================================
来源：http://fy.bookmarksfly.cn

I. 正则表达式
来源：http://ho.nicolike.cn

================================================================================
来源：http://sp.521024.cn

[I01] 判断是否匹配
来源：http://sq.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bo.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yv.521024.cn

JS:   /\d+/.test(s)
来源：http://ay.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://co.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sl.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hq.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://yx.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yn.newstarts.cn

[I02] 提取所有匹配
来源：http://md.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://au.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xk.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zx.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://az.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ro.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rc.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://uk.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qu.nicolike.cn

[I03] 提取捕获分组
来源：http://xa.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xp.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jc.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yh.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pn.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hu.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dx.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://if.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mv.bookmarksfly.cn

[I04] 正则替换
来源：http://xv.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bt.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://py.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vl.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://es.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://so.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vq.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cb.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qy.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://mj.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sx.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dk.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://gc.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ok.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://up.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rp.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ns.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ud.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rj.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nm.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eh.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ip.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mw.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wi.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bz.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mo.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xt.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://uo.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ps.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ww.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wm.szxytkj.cn

TS:   /error/gim
来源：http://tq.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dn.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eb.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://ff.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mk.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://nm.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://il.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wr.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rv.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yu.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tc.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gb.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://at.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jf.shxzukj.cn

================================================================================
来源：http://sv.nicolike.cn

J. 日期与时间
来源：http://yp.panjiajie.cn

================================================================================
来源：http://ol.muxihuayi.cn

[J01] 获取当前时间
来源：http://uy.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nq.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fs.huanxung.cn

JS:   new Date();  Date.now()
来源：http://rt.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://vi.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ii.newstarts.cn

Go:   time.Now()
来源：http://on.haigaiapp.cn

Ruby: Time.now
来源：http://hp.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gs.colortex.cn

[J02] 格式化输出
来源：http://ko.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cn.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xd.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pa.hahajie.cn

TS:   d.toISOString()
来源：http://ct.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qy.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ps.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gs.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xz.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://ag.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yk.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nn.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://mb.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://qt.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dd.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ra.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://wx.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gm.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://rm.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dy.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bw.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ck.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mu.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dx.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tv.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://na.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zu.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://be.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://wx.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tv.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qx.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ax.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://bq.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ag.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ra.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://do.nicolike.cn

[J06] 计算两时间之差
来源：http://wt.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://mv.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://tf.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ml.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hm.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zn.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://hc.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://bz.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://mm.nszjky.cn

[J07] 比较两个日期
来源：http://dl.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://mj.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ub.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ej.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hw.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gs.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hf.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jv.szxytkj.cn


<!-- 参考信息 -->