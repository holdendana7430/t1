代发 wailian999

PHP:  public static function f() {}
来源：http://oi.gzmigu.cn

JS:   static f() {}
来源：http://op.shtwfgs.cn

TS:   static f(): void {}
来源：http://nm.jianghongdianzi.cn

Java: static void f() {}
来源：http://ch.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oq.9csxet.cn

Ruby: def self.f; end
来源：http://eb.huixiangedu.cn

C#:   public static void F() {}
来源：http://rw.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://ql.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://of.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kg.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oq.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://cg.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://bt.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://lr.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tg.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://bx.haigaiapp.cn

[G10] 访问控制
来源：http://yu.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://kb.szsharing.cn

PHP:  public / protected / private
来源：http://lg.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://sl.hahajie.cn

TS:   public / protected / private
来源：http://kh.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://ou.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gj.bjjhwx.cn

Ruby: public / protected / private
来源：http://zw.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://wx.chemitech.net.cn

[G11] getter / setter
来源：http://xz.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://go.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ti.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://mq.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://tz.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://pm.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xq.521024.cn

Ruby: attr_accessor :name
来源：http://gc.nszjky.cn

C#:   public string Name { get; set; }
来源：http://oo.nszjky.cn

[G12] 对象转字符串
来源：http://nm.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://uu.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xw.colortex.cn

JS:   toString() { return this.name; }
来源：http://uj.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://xs.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://ld.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xv.nszjky.cn

Ruby: def to_s; @name; end
来源：http://li.521024.cn

C#:   public override string ToString() => Name;
来源：http://xh.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://pl.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://pq.hahajie.cn

PHP:  $u instanceof User
来源：http://fc.szxytkj.cn

JS:   u instanceof User
来源：http://ip.chemitech.net.cn

TS:   u instanceof User
来源：http://mv.hahajie.cn

Java: u instanceof User
来源：http://xx.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ua.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://gi.huixiangedu.cn

C#:   u is User
来源：http://aw.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://ho.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jz.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://wr.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uc.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://br.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://aw.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://jl.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://es.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://bh.muxihuayi.cn

[G15] 枚举
来源：http://ek.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nq.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ya.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lr.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rl.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://hs.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ig.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://iq.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fp.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://kk.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ss.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://uj.panjiajie.cn

JS:   Object.entries(obj)
来源：http://hu.szxytkj.cn

TS:   Object.entries(obj)
来源：http://ui.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kt.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zq.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://te.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://js.huixiangedu.cn

================================================================================
来源：http://vc.huanxung.cn

H. 异常与错误处理
来源：http://bw.gzmigu.cn

================================================================================
来源：http://bj.bookmarksfly.cn

[H01] try / catch 基础
来源：http://ta.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xr.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ck.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wn.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tz.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ev.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://il.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ib.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bu.huanxung.cn

[H02] finally / ensure 收尾
来源：http://du.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wl.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dj.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ej.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lg.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ax.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fl.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ow.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pa.muxihuayi.cn

[H03] 主动抛出异常
来源：http://bm.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://mr.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cs.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://zf.521024.cn

TS:   throw new Error("错误信息");
来源：http://xa.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mj.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://op.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cb.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qi.lnxyls.cn

[H04] 自定义异常类型
来源：http://ui.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://bt.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zo.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://kw.hahajie.cn

TS:   class MyError extends Error {}
来源：http://zr.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://bx.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xl.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://eh.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://pk.haigaiapp.cn

[H05] 捕获特定类型
来源：http://ay.huixiangedu.cn

Py:   except ValueError as e:
来源：http://qm.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ks.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://aa.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://zm.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://wu.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sj.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://ur.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uq.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://iu.huanxung.cn

Py:   value = d.get("k") or default
来源：http://am.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cv.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qy.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://se.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hc.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qc.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://lw.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://pd.muxihuayi.cn

[H07] 断言
来源：http://en.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://xm.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://zh.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://rd.colortex.cn

TS:   console.assert(x > 0);
来源：http://fq.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://tx.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rg.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oe.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://xx.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://cu.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://en.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pg.hahajie.cn

JS:   e.message;  e.stack
来源：http://dz.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nz.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kn.newstarts.cn

Go:   err.Error()
来源：http://gl.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://vk.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://lv.hahajie.cn

[H09] 带错误码的异常
来源：http://ul.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ut.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ov.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yq.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hx.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ax.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kv.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://py.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://js.521024.cn

[H10] 资源自动释放
来源：http://qv.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ok.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ti.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vd.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ci.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ah.gzmigu.cn

Go:   defer f.Close()
来源：http://wi.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ge.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uq.shxzskj.cn

================================================================================
来源：http://rz.bjjhwx.cn

I. 正则表达式
来源：http://xt.nszjky.cn

================================================================================
来源：http://qg.huanxung.cn

[I01] 判断是否匹配
来源：http://ep.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lj.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dq.szsharing.cn

JS:   /\d+/.test(s)
来源：http://ta.hahajie.cn

TS:   /\d+/.test(s)
来源：http://at.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dr.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jq.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://ua.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://up.nicolike.cn

[I02] 提取所有匹配
来源：http://su.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://ov.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cj.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hv.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://ps.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://te.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lb.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://ln.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ez.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://ux.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ml.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://on.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rl.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xn.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://je.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gy.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dl.jianghongdianzi.cn

[I04] 正则替换
来源：http://dh.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ig.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gq.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xa.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hw.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ag.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wn.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lm.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vx.muxihuayi.cn

[I05] 按正则拆分
来源：http://kd.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jk.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ru.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://nx.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://po.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://to.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nq.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fx.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dz.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iu.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qe.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gh.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qo.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rn.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rx.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qi.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iy.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ie.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://id.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kf.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ma.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bi.huanxung.cn

TS:   /error/gim
来源：http://hr.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yd.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cx.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ph.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wv.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://hj.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ny.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ob.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jn.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ro.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uh.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pp.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hm.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://to.jctech888.com.cn

================================================================================
来源：http://fa.shtwfgs.cn

J. 日期与时间
来源：http://yb.jctech888.com.cn

================================================================================
来源：http://jo.newstarts.cn

[J01] 获取当前时间
来源：http://gh.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xj.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lk.newstarts.cn

JS:   new Date();  Date.now()
来源：http://jd.newstarts.cn

TS:   new Date();  Date.now()
来源：http://iw.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cw.jctech888.com.cn

Go:   time.Now()
来源：http://hp.gzmigu.cn

Ruby: Time.now
来源：http://ns.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pj.panjiajie.cn

[J02] 格式化输出
来源：http://xf.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yk.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rx.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ds.9csxet.cn

TS:   d.toISOString()
来源：http://fn.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ra.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bs.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ia.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ri.lnxyls.cn

[J03] 字符串解析为日期
来源：http://gp.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dg.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hd.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://so.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://vy.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fj.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ic.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://lp.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rq.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://mb.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nv.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ti.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nw.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://un.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rc.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ij.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gy.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pr.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://kg.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://of.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sz.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bj.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ta.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://qy.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mf.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://vm.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yl.huixiangedu.cn

[J06] 计算两时间之差
来源：http://zm.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://ub.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://tj.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pd.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qj.shxzskj.cn


<!-- 参考信息 -->