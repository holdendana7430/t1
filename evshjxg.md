代发 wailian999

PHP:  public static function f() {}
来源：http://uy.wgjwhj.cn

JS:   static f() {}
来源：http://hk.panjiajie.cn

TS:   static f(): void {}
来源：http://yd.nicolike.cn

Java: static void f() {}
来源：http://nf.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ui.wgjwhj.cn

Ruby: def self.f; end
来源：http://yc.hahajie.cn

C#:   public static void F() {}
来源：http://av.9csxet.cn

[G09] 接口 / 抽象类
来源：http://wb.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://dq.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://du.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://le.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://wf.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://mk.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://oe.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://um.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://wa.huixinmuqiang.cn

[G10] 访问控制
来源：http://ef.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://qi.muxihuayi.cn

PHP:  public / protected / private
来源：http://kx.szsharing.cn

JS:   #private 字段；其余公开
来源：http://we.colortex.cn

TS:   public / protected / private
来源：http://jk.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://mr.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mu.gzmigu.cn

Ruby: public / protected / private
来源：http://eg.521024.cn

C#:   public / protected / private / internal
来源：http://rd.gzmigu.cn

[G11] getter / setter
来源：http://yj.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://sd.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nj.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://sz.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://bs.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://gv.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xe.shxzskj.cn

Ruby: attr_accessor :name
来源：http://at.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ro.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://fy.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://bn.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ec.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://ae.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://oz.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://hx.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://su.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://xj.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://xr.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://rn.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://by.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://ft.shtwfgs.cn

JS:   u instanceof User
来源：http://kx.shxzukj.cn

TS:   u instanceof User
来源：http://rq.gzmigu.cn

Java: u instanceof User
来源：http://ui.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rb.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ae.haigaiapp.cn

C#:   u is User
来源：http://qn.yuexingan06.cn

[G14] 数据类 / record
来源：http://rm.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ux.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://fp.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ji.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://te.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://mh.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://nm.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mq.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://ep.nszjky.cn

[G15] 枚举
来源：http://rf.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lc.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dt.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ai.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cd.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://bh.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fx.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://fk.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bj.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://or.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kl.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://db.colortex.cn

JS:   Object.entries(obj)
来源：http://ud.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://eg.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rm.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ho.hahajie.cn

Ruby: obj.instance_variables
来源：http://ok.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://qm.shxzskj.cn

================================================================================
来源：http://rh.gzmigu.cn

H. 异常与错误处理
来源：http://gp.yuntaijiaju.cn

================================================================================
来源：http://zp.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://ce.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cn.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kp.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sf.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oz.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hi.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wr.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sf.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ea.9csxet.cn

[H02] finally / ensure 收尾
来源：http://zf.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ev.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qe.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ot.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qb.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://my.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xq.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hs.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://db.muxihuayi.cn

[H03] 主动抛出异常
来源：http://by.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://vg.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xi.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://yz.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://op.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pa.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zg.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yd.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pz.jctech888.com.cn

[H04] 自定义异常类型
来源：http://rw.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://qc.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zu.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://pc.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://aw.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://ft.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pm.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://gd.colortex.cn

C#:   class MyException : Exception {}
来源：http://cw.hahajie.cn

[H05] 捕获特定类型
来源：http://pu.chemitech.net.cn

Py:   except ValueError as e:
来源：http://rh.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iy.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://pv.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://tr.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://un.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://il.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://yq.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ok.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://pe.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://kc.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ys.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tt.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qo.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wm.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gh.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://vi.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://pe.haigaiapp.cn

[H07] 断言
来源：http://wz.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://un.9csxet.cn

PHP:  assert($x > 0);
来源：http://rz.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://cc.asd995.cn

TS:   console.assert(x > 0);
来源：http://cz.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://xj.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kx.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iq.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ak.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://qn.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://bu.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rn.gzmigu.cn

JS:   e.message;  e.stack
来源：http://bg.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ru.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hq.yuntaijiaju.cn

Go:   err.Error()
来源：http://iw.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://bv.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://su.hahajie.cn

[H09] 带错误码的异常
来源：http://ka.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rf.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bi.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://km.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ew.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sb.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vy.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kw.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rc.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://bp.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kn.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sj.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sa.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ir.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wq.newstarts.cn

Go:   defer f.Close()
来源：http://vs.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rr.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://js.haigaiapp.cn

================================================================================
来源：http://az.shtwfgs.cn

I. 正则表达式
来源：http://rz.hnjuh.cn

================================================================================
来源：http://in.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://ye.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yd.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qx.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://zm.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://sv.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fv.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ge.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://ye.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cq.muxihuayi.cn

[I02] 提取所有匹配
来源：http://ia.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://kh.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rd.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bv.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://rz.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sp.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pf.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://if.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mf.wgjwhj.cn

[I03] 提取捕获分组
来源：http://xm.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zn.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ug.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://na.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jt.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zp.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dq.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dz.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ms.colortex.cn

[I04] 正则替换
来源：http://cj.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wk.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nf.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ri.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://do.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ln.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://am.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uz.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qv.wgjwhj.cn

[I05] 按正则拆分
来源：http://ei.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xg.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qf.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://nn.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://pb.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://fx.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://be.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cr.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sl.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nq.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bg.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wk.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kg.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vm.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ma.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ky.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ym.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vj.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://hp.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lt.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ul.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iq.asd995.cn

TS:   /error/gim
来源：http://sv.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kb.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hk.521024.cn

Ruby: s.scan(/error/i)
来源：http://ch.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pn.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://cl.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yo.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uw.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zp.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ff.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qe.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yl.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kg.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nk.szsharing.cn

================================================================================
来源：http://uh.shxzskj.cn

J. 日期与时间
来源：http://gy.gzmigu.cn

================================================================================
来源：http://qr.asd995.cn

[J01] 获取当前时间
来源：http://up.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pr.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yd.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://ie.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://mb.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://di.hnjuh.cn

Go:   time.Now()
来源：http://em.shxzukj.cn

Ruby: Time.now
来源：http://zg.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kt.huixiangedu.cn

[J02] 格式化输出
来源：http://ou.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tz.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://up.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xd.wgjwhj.cn

TS:   d.toISOString()
来源：http://hy.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kx.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jh.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mq.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zk.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://qc.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yc.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zc.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://qj.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://tj.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wg.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wd.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://uw.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://go.szsharing.cn

[J04] 时间戳与日期互转
来源：http://pf.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://el.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ni.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rt.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ul.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://js.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vu.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lc.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qv.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://rj.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://fl.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fd.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oe.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nh.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://nr.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xz.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://yv.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zn.szsharing.cn

[J06] 计算两时间之差
来源：http://py.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://bj.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://wu.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ot.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://th.szxytkj.cn


<!-- 参考信息 -->