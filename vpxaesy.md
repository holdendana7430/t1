代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://um.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qv.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fi.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://qj.newstarts.cn

Java: interface Shape { double area(); }
来源：http://ha.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://wr.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rm.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://eb.yuexingan06.cn

[G10] 访问控制
来源：http://rb.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://yz.asd995.cn

PHP:  public / protected / private
来源：http://dy.asd995.cn

JS:   #private 字段；其余公开
来源：http://yn.haigaiapp.cn

TS:   public / protected / private
来源：http://rp.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://gs.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wm.huixiangedu.cn

Ruby: public / protected / private
来源：http://qn.szsharing.cn

C#:   public / protected / private / internal
来源：http://hj.jctech888.com.cn

[G11] getter / setter
来源：http://iq.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://zo.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qh.nicolike.cn

JS:   get name() { return this._name; }
来源：http://cg.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://an.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://vj.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yi.nicolike.cn

Ruby: attr_accessor :name
来源：http://ci.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://lp.muxihuayi.cn

[G12] 对象转字符串
来源：http://lz.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://li.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jh.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://cg.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://ce.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://lq.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ja.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://do.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://gk.chemitech.net.cn

[G13] 判断对象类型
来源：http://kw.nicolike.cn

Py:   isinstance(u, User)
来源：http://cw.panjiajie.cn

PHP:  $u instanceof User
来源：http://of.gzmigu.cn

JS:   u instanceof User
来源：http://gu.asd995.cn

TS:   u instanceof User
来源：http://qq.521024.cn

Java: u instanceof User
来源：http://by.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mu.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://yf.huanxung.cn

C#:   u is User
来源：http://oy.haigaiapp.cn

[G14] 数据类 / record
来源：http://iy.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oq.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://pn.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uo.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://lo.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://ib.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://bw.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mw.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://ve.nicolike.cn

[G15] 枚举
来源：http://ge.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yy.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sv.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://us.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bk.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://sb.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pl.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://wl.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tz.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://jn.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qq.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://hn.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ky.shxzskj.cn

TS:   Object.entries(obj)
来源：http://ep.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fm.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://it.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://fu.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ls.shxzskj.cn

================================================================================
来源：http://qv.bookmarksfly.cn

H. 异常与错误处理
来源：http://ue.shtwfgs.cn

================================================================================
来源：http://ck.huanxung.cn

[H01] try / catch 基础
来源：http://gb.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lf.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ms.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rf.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bx.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nv.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yv.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lb.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://le.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://qh.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oh.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cb.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bs.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xn.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yh.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bw.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uc.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mb.szxytkj.cn

[H03] 主动抛出异常
来源：http://qf.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://bv.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://um.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://qh.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://rx.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://he.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kn.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ak.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tq.hahajie.cn

[H04] 自定义异常类型
来源：http://iv.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://zz.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://us.huanxung.cn

JS:   class MyError extends Error {}
来源：http://le.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://ta.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://gs.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sn.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ww.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://dc.wgjwhj.cn

[H05] 捕获特定类型
来源：http://lz.shxzukj.cn

Py:   except ValueError as e:
来源：http://ek.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oq.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://pg.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://ia.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://jn.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jl.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://gd.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://us.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://fn.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://nl.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ws.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://es.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tj.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ak.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fy.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://wh.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://up.nicolike.cn

[H07] 断言
来源：http://fj.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://ul.521024.cn

PHP:  assert($x > 0);
来源：http://wa.9csxet.cn

JS:   console.assert(x > 0);
来源：http://tz.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://tu.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://eu.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://en.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xa.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://kx.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://yp.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://bl.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ui.nicolike.cn

JS:   e.message;  e.stack
来源：http://zj.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yd.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qk.shxzskj.cn

Go:   err.Error()
来源：http://ef.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://ml.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://rw.jctech888.com.cn

[H09] 带错误码的异常
来源：http://iw.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rc.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gd.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://go.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dw.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vl.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yo.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wr.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fu.shxzukj.cn

[H10] 资源自动释放
来源：http://pt.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xd.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kk.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://op.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://at.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ej.jctech888.com.cn

Go:   defer f.Close()
来源：http://og.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lx.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eg.huanxung.cn

================================================================================
来源：http://pg.huixinmuqiang.cn

I. 正则表达式
来源：http://yq.bookmarksfly.cn

================================================================================
来源：http://et.huanxung.cn

[I01] 判断是否匹配
来源：http://aj.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rn.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zr.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://so.asd995.cn

TS:   /\d+/.test(s)
来源：http://oo.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xb.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cv.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://vi.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rt.colortex.cn

[I02] 提取所有匹配
来源：http://it.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://fz.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ss.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ds.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://eo.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ll.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vm.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://go.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ai.szxytkj.cn

[I03] 提取捕获分组
来源：http://te.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kt.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zv.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hl.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cw.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pz.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ny.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cy.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xj.nicolike.cn

[I04] 正则替换
来源：http://jl.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hh.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rb.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nj.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vz.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yz.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gv.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://we.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kh.jctech888.com.cn

[I05] 按正则拆分
来源：http://vs.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://la.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jq.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://oc.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://av.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://bo.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bu.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ml.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yr.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://li.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kx.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fv.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cs.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tv.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nt.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://or.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pg.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zq.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://xc.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xb.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ob.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dg.haigaiapp.cn

TS:   /error/gim
来源：http://gp.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bl.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iv.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://vw.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ew.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ug.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uw.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rr.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ye.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://go.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kn.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nn.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pv.szxytkj.cn

================================================================================
来源：http://xi.hnjuh.cn

J. 日期与时间
来源：http://zy.hahajie.cn

================================================================================
来源：http://jv.asd995.cn

[J01] 获取当前时间
来源：http://eb.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lb.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bc.nicolike.cn

JS:   new Date();  Date.now()
来源：http://xw.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://lv.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vr.szsharing.cn

Go:   time.Now()
来源：http://qs.huixiangedu.cn

Ruby: Time.now
来源：http://jq.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wf.haigaiapp.cn

[J02] 格式化输出
来源：http://oz.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cr.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kl.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qt.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://wp.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://de.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://se.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vs.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wf.gzmigu.cn

[J03] 字符串解析为日期
来源：http://xb.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://va.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tn.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://mp.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://gl.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://od.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sl.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://jr.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fe.newstarts.cn

[J04] 时间戳与日期互转
来源：http://qk.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oc.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ut.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ih.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yu.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wt.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pn.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ro.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gn.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://qv.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://uj.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oz.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ii.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://og.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://il.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dk.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://lh.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jt.bjjhwx.cn

[J06] 计算两时间之差
来源：http://xb.colortex.cn

Py:   (end - start).total_seconds()
来源：http://ib.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://em.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fo.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ny.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yt.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://jv.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://or.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://yj.bjjhwx.cn

[J07] 比较两个日期
来源：http://qe.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://yk.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cj.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ji.shxzukj.cn


<!-- 参考信息 -->