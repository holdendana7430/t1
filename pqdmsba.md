代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://yq.haigaiapp.cn

Ruby: def self.f; end
来源：http://cq.shxzukj.cn

C#:   public static void F() {}
来源：http://nw.huanxung.cn

[G09] 接口 / 抽象类
来源：http://ma.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://lk.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mg.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://my.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://gq.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://td.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://ct.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ef.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://lv.szsharing.cn

[G10] 访问控制
来源：http://du.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://cw.chemitech.net.cn

PHP:  public / protected / private
来源：http://gn.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://hv.shtwfgs.cn

TS:   public / protected / private
来源：http://fc.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://cg.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xn.asd995.cn

Ruby: public / protected / private
来源：http://eq.521024.cn

C#:   public / protected / private / internal
来源：http://cc.haigaiapp.cn

[G11] getter / setter
来源：http://jz.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://uv.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://te.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://jj.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://zi.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://tq.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uq.szsharing.cn

Ruby: attr_accessor :name
来源：http://lo.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://tz.yuexingan06.cn

[G12] 对象转字符串
来源：http://fa.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://ha.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mx.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://ke.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://de.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://aa.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rh.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://kx.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://pn.bjjhwx.cn

[G13] 判断对象类型
来源：http://up.huanxung.cn

Py:   isinstance(u, User)
来源：http://wy.lnxyls.cn

PHP:  $u instanceof User
来源：http://rn.colortex.cn

JS:   u instanceof User
来源：http://sz.nicolike.cn

TS:   u instanceof User
来源：http://tp.shxzskj.cn

Java: u instanceof User
来源：http://pi.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://da.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://qh.yuntaijiaju.cn

C#:   u is User
来源：http://uh.shxzukj.cn

[G14] 数据类 / record
来源：http://yx.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ia.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://en.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lv.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://sb.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://oe.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://xk.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tb.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://nr.chemitech.net.cn

[G15] 枚举
来源：http://sb.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pk.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sp.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nv.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pf.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://pr.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cj.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://ji.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xe.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ys.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tk.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ye.asd995.cn

JS:   Object.entries(obj)
来源：http://uu.hnjuh.cn

TS:   Object.entries(obj)
来源：http://on.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mn.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vo.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://zi.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://vf.newstarts.cn

================================================================================
来源：http://kr.wgjwhj.cn

H. 异常与错误处理
来源：http://ms.nicolike.cn

================================================================================
来源：http://al.lnxyls.cn

[H01] try / catch 基础
来源：http://zh.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hf.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hl.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xw.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bu.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vh.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dl.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ev.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gi.huanxung.cn

[H02] finally / ensure 收尾
来源：http://qc.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aq.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hb.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mr.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gj.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ke.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qq.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zk.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gj.yuexingan06.cn

[H03] 主动抛出异常
来源：http://vi.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://hi.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lp.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://mc.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://iz.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oz.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://im.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nk.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xu.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://pe.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://ee.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cx.huanxung.cn

JS:   class MyError extends Error {}
来源：http://ym.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://fh.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://rt.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gc.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://ew.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://rb.nicolike.cn

[H05] 捕获特定类型
来源：http://ha.yuexingan06.cn

Py:   except ValueError as e:
来源：http://cv.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fb.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://xg.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://nw.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://st.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cp.521024.cn

Ruby: rescue ArgumentError => e
来源：http://zt.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sw.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://qh.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://ey.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://or.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://op.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xw.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bu.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ef.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://qc.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://xb.huixiangedu.cn

[H07] 断言
来源：http://sk.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://dg.huanxung.cn

PHP:  assert($x > 0);
来源：http://po.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://ul.nszjky.cn

TS:   console.assert(x > 0);
来源：http://pl.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://hx.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jd.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fo.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://wc.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://po.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://fm.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tm.nszjky.cn

JS:   e.message;  e.stack
来源：http://jd.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sj.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://io.panjiajie.cn

Go:   err.Error()
来源：http://op.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://ws.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://qb.9csxet.cn

[H09] 带错误码的异常
来源：http://aa.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://na.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zs.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mh.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vo.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jb.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://at.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vx.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rq.muxihuayi.cn

[H10] 资源自动释放
来源：http://jb.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wt.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kd.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wc.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vq.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://no.muxihuayi.cn

Go:   defer f.Close()
来源：http://lg.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ro.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pm.yuexingan06.cn

================================================================================
来源：http://dt.panjiajie.cn

I. 正则表达式
来源：http://pb.jctech888.com.cn

================================================================================
来源：http://mb.jctech888.com.cn

[I01] 判断是否匹配
来源：http://sb.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yp.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qz.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://kl.asd995.cn

TS:   /\d+/.test(s)
来源：http://np.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ct.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kj.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://wf.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dw.nszjky.cn

[I02] 提取所有匹配
来源：http://ae.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://nb.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ju.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xz.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://nh.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://er.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wp.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://fu.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nz.shtwfgs.cn

[I03] 提取捕获分组
来源：http://ib.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yk.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rm.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kq.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nz.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oy.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qu.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qs.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nc.chemitech.net.cn

[I04] 正则替换
来源：http://ye.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rv.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qs.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fv.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://or.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rx.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://by.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fw.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://de.muxihuayi.cn

[I05] 按正则拆分
来源：http://qm.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cw.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kh.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://gl.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://nj.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://rn.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oi.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://di.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wn.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ky.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fc.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ev.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sm.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sq.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ab.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yf.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pt.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zi.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://re.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wx.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vy.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dv.huixinmuqiang.cn

TS:   /error/gim
来源：http://wc.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bv.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ic.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://va.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kn.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://xx.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://td.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xy.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gq.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mo.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://io.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://at.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pj.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bn.szxytkj.cn

================================================================================
来源：http://tf.wgjwhj.cn

J. 日期与时间
来源：http://ja.newstarts.cn

================================================================================
来源：http://ec.colortex.cn

[J01] 获取当前时间
来源：http://ba.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zb.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fa.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://un.newstarts.cn

TS:   new Date();  Date.now()
来源：http://jt.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ke.hahajie.cn

Go:   time.Now()
来源：http://tt.nszjky.cn

Ruby: Time.now
来源：http://an.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pc.szxytkj.cn

[J02] 格式化输出
来源：http://gs.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pj.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://js.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hb.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://nx.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ax.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ii.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qo.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ud.colortex.cn

[J03] 字符串解析为日期
来源：http://mi.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hv.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ir.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://xd.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://fq.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cb.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lw.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://kf.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bc.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://nf.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mo.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fg.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rr.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://aw.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lf.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qa.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ep.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cn.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://hv.colortex.cn

Py:   now + timedelta(days=7)
来源：http://qo.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tb.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vq.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hh.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://pp.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ut.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://zr.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pa.shxzskj.cn

[J06] 计算两时间之差
来源：http://xe.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://ys.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://zx.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://di.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oh.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lg.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://mj.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://oo.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://my.yuexingan06.cn


<!-- 参考信息 -->