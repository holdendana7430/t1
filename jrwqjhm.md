代发 wailian999

Java: interface Shape { double area(); }
来源：http://qd.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://cd.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vb.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://qx.gzmigu.cn

[G10] 访问控制
来源：http://tf.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ry.newstarts.cn

PHP:  public / protected / private
来源：http://hl.asd995.cn

JS:   #private 字段；其余公开
来源：http://yf.gzmigu.cn

TS:   public / protected / private
来源：http://pq.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://zi.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lz.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://wl.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://en.jianghongdianzi.cn

[G11] getter / setter
来源：http://ze.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://pe.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rd.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://xf.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://cm.521024.cn

Java: public String getName() { return name; }
来源：http://on.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ee.asd995.cn

Ruby: attr_accessor :name
来源：http://lt.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://lg.hnjuh.cn

[G12] 对象转字符串
来源：http://hg.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://dz.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fm.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://cl.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://wk.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://eu.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yd.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://xp.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://lj.wgjwhj.cn

[G13] 判断对象类型
来源：http://zm.shxzskj.cn

Py:   isinstance(u, User)
来源：http://cz.shtwfgs.cn

PHP:  $u instanceof User
来源：http://by.hnjuh.cn

JS:   u instanceof User
来源：http://vm.yuntaijiaju.cn

TS:   u instanceof User
来源：http://hw.yuexingan06.cn

Java: u instanceof User
来源：http://oe.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nd.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://tf.szsharing.cn

C#:   u is User
来源：http://ei.shtwfgs.cn

[G14] 数据类 / record
来源：http://cp.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rt.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://bs.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wg.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://st.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://tj.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://gl.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ax.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://xu.gzmigu.cn

[G15] 枚举
来源：http://ru.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nz.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dw.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gk.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ty.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://jo.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lc.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://kx.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vv.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://xi.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uv.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://rz.hahajie.cn

JS:   Object.entries(obj)
来源：http://gp.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://wa.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mh.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dq.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://es.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://yx.huixiangedu.cn

================================================================================
来源：http://lw.shtwfgs.cn

H. 异常与错误处理
来源：http://zm.shtwfgs.cn

================================================================================
来源：http://be.huanxung.cn

[H01] try / catch 基础
来源：http://nk.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jb.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ua.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mx.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yc.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nv.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hm.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oi.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jy.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://uf.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tw.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wm.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jb.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mb.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ff.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pt.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gn.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zt.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://jw.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://bx.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yl.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://nv.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://wt.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sq.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vq.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ri.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wm.haigaiapp.cn

[H04] 自定义异常类型
来源：http://vl.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://an.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rw.asd995.cn

JS:   class MyError extends Error {}
来源：http://bq.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://lv.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://at.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rj.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ut.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://da.521024.cn

[H05] 捕获特定类型
来源：http://pd.lnxyls.cn

Py:   except ValueError as e:
来源：http://pm.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qp.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://fg.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://cd.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://ck.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rl.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://ve.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lo.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://eh.hahajie.cn

Py:   value = d.get("k") or default
来源：http://rv.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cq.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xb.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hm.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qw.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kj.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ad.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://jw.hahajie.cn

[H07] 断言
来源：http://ga.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://al.newstarts.cn

PHP:  assert($x > 0);
来源：http://qs.nicolike.cn

JS:   console.assert(x > 0);
来源：http://ya.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://jk.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://ad.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ui.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ws.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://as.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://rj.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://cy.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kh.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://to.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kn.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bk.9csxet.cn

Go:   err.Error()
来源：http://rl.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://ep.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://fx.newstarts.cn

[H09] 带错误码的异常
来源：http://jo.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hh.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xv.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pv.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cy.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vk.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zd.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://be.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bx.panjiajie.cn

[H10] 资源自动释放
来源：http://ym.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://js.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ka.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oy.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cz.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://js.panjiajie.cn

Go:   defer f.Close()
来源：http://tk.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ma.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jk.szsharing.cn

================================================================================
来源：http://fo.szxytkj.cn

I. 正则表达式
来源：http://ay.shtwfgs.cn

================================================================================
来源：http://qe.9csxet.cn

[I01] 判断是否匹配
来源：http://ou.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wn.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lt.huanxung.cn

JS:   /\d+/.test(s)
来源：http://xf.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://bf.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nr.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ed.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://ey.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ys.nicolike.cn

[I02] 提取所有匹配
来源：http://lq.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://rq.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wz.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xz.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://te.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lm.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nj.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://jt.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fo.wgjwhj.cn

[I03] 提取捕获分组
来源：http://tf.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fk.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ar.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hs.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yd.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lj.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zl.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ys.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kj.szxytkj.cn

[I04] 正则替换
来源：http://ix.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tl.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hm.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ai.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wt.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xv.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uz.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lr.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://az.szxytkj.cn

[I05] 按正则拆分
来源：http://nr.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nt.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hj.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://uc.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://cq.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://nv.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bu.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iw.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gb.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gw.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rn.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://av.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wj.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xy.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xm.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://os.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qt.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sv.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://pm.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sl.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://um.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ci.yuexingan06.cn

TS:   /error/gim
来源：http://ov.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pl.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gx.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://pl.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://an.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ux.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oj.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ut.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ww.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ph.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://io.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://se.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ae.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lb.jctech888.com.cn

================================================================================
来源：http://gl.szxytkj.cn

J. 日期与时间
来源：http://ou.shtwfgs.cn

================================================================================
来源：http://bl.shtwfgs.cn

[J01] 获取当前时间
来源：http://zc.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sv.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ql.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://bi.nicolike.cn

TS:   new Date();  Date.now()
来源：http://jt.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zl.9csxet.cn

Go:   time.Now()
来源：http://hi.haigaiapp.cn

Ruby: Time.now
来源：http://yc.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rq.nszjky.cn

[J02] 格式化输出
来源：http://gi.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://za.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://le.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wn.shtwfgs.cn

TS:   d.toISOString()
来源：http://mi.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://el.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ua.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fj.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vv.nszjky.cn

[J03] 字符串解析为日期
来源：http://xh.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ar.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dc.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://hl.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://pq.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ev.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fu.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://xb.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xz.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://kj.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wb.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ux.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fy.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hx.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cv.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zg.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ud.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fo.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://ns.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://yf.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://se.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eo.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://ir.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hy.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://ep.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://km.panjiajie.cn

[J06] 计算两时间之差
来源：http://hc.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://fm.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://rs.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fg.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://od.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wy.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://cc.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://ux.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://wl.chemitech.net.cn

[J07] 比较两个日期
来源：http://do.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://fz.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eg.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ob.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fp.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://am.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mb.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gs.hnjuh.cn


<!-- 参考信息 -->