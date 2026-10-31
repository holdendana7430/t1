代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://ya.panjiajie.cn

Ruby: def self.f; end
来源：http://jg.wgjwhj.cn

C#:   public static void F() {}
来源：http://fe.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://nb.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://zx.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qr.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vc.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://iu.nszjky.cn

Java: interface Shape { double area(); }
来源：http://fm.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://qh.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mj.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://ef.yuntaijiaju.cn

[G10] 访问控制
来源：http://hk.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://kd.wgjwhj.cn

PHP:  public / protected / private
来源：http://gm.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://on.bjjhwx.cn

TS:   public / protected / private
来源：http://lu.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://yf.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://au.lnxyls.cn

Ruby: public / protected / private
来源：http://lk.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://fh.bjjhwx.cn

[G11] getter / setter
来源：http://yr.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://xa.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tg.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://gw.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://zu.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://ej.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nt.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://vr.9csxet.cn

C#:   public string Name { get; set; }
来源：http://lt.jctech888.com.cn

[G12] 对象转字符串
来源：http://hd.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://ia.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gs.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://qe.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://ii.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://yt.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tx.colortex.cn

Ruby: def to_s; @name; end
来源：http://pq.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://jn.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://vt.nicolike.cn

Py:   isinstance(u, User)
来源：http://qg.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://na.asd995.cn

JS:   u instanceof User
来源：http://bk.huixinmuqiang.cn

TS:   u instanceof User
来源：http://yw.hnjuh.cn

Java: u instanceof User
来源：http://uy.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pa.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://ja.bookmarksfly.cn

C#:   u is User
来源：http://lg.gzmigu.cn

[G14] 数据类 / record
来源：http://qc.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nl.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://jy.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://my.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://jj.szsharing.cn

Java: record User(String name, int age) {}
来源：http://ps.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://im.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cu.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://bo.521024.cn

[G15] 枚举
来源：http://vt.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://to.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dg.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hd.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ig.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://qw.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ih.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://yf.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ge.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://fk.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sl.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://tp.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://ik.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://cg.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://el.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ni.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://zp.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://na.panjiajie.cn

================================================================================
来源：http://ym.hnjuh.cn

H. 异常与错误处理
来源：http://ev.bjjhwx.cn

================================================================================
来源：http://jh.colortex.cn

[H01] try / catch 基础
来源：http://io.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vp.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aj.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pc.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tv.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ow.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lg.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tx.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://io.newstarts.cn

[H02] finally / ensure 收尾
来源：http://kp.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rp.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tc.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tt.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zp.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uf.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nd.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zp.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qt.newstarts.cn

[H03] 主动抛出异常
来源：http://ek.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://px.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yd.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://ic.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://et.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yn.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ed.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rl.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ql.panjiajie.cn

[H04] 自定义异常类型
来源：http://qe.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://iz.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jc.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://gu.newstarts.cn

TS:   class MyError extends Error {}
来源：http://yb.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://sy.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ei.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://xa.newstarts.cn

C#:   class MyException : Exception {}
来源：http://rk.521024.cn

[H05] 捕获特定类型
来源：http://ae.asd995.cn

Py:   except ValueError as e:
来源：http://lg.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cu.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://ub.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://gc.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://ud.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://po.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://hr.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nf.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://kj.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://jy.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ow.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pj.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jx.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pl.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://of.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://gt.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://sf.huixiangedu.cn

[H07] 断言
来源：http://bc.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://jv.panjiajie.cn

PHP:  assert($x > 0);
来源：http://qf.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://vv.nicolike.cn

TS:   console.assert(x > 0);
来源：http://za.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://kh.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lr.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mr.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://ib.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://dp.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://ut.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://in.colortex.cn

JS:   e.message;  e.stack
来源：http://id.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ar.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ar.huixiangedu.cn

Go:   err.Error()
来源：http://bi.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://do.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://nl.szxytkj.cn

[H09] 带错误码的异常
来源：http://hr.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mh.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ez.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zv.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lu.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ri.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gm.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xi.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xw.hnjuh.cn

[H10] 资源自动释放
来源：http://fe.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ng.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gn.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rf.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xw.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oj.hnjuh.cn

Go:   defer f.Close()
来源：http://ud.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jm.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ml.panjiajie.cn

================================================================================
来源：http://og.bookmarksfly.cn

I. 正则表达式
来源：http://vv.shtwfgs.cn

================================================================================
来源：http://jo.haigaiapp.cn

[I01] 判断是否匹配
来源：http://gv.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sh.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qo.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://bd.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://iy.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://li.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yb.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://yp.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rc.bjjhwx.cn

[I02] 提取所有匹配
来源：http://rm.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://ie.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rh.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bm.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://ky.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ok.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pr.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://ud.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zj.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://su.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ji.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jc.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qs.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lk.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ei.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ud.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eu.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://um.panjiajie.cn

[I04] 正则替换
来源：http://hx.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://om.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rf.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qp.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://en.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wl.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jo.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hg.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vs.colortex.cn

[I05] 按正则拆分
来源：http://ro.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ja.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ia.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://tg.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://lx.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://cp.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wp.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yy.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ug.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ir.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ma.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eo.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hh.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ha.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://er.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dv.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bw.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dj.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://mt.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cc.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yc.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ps.haigaiapp.cn

TS:   /error/gim
来源：http://yy.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vq.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hq.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://cg.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xu.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://dw.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ul.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qa.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lf.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tj.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ru.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kj.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://im.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zh.yuexingan06.cn

================================================================================
来源：http://mj.jctech888.com.cn

J. 日期与时间
来源：http://ky.yuntaijiaju.cn

================================================================================
来源：http://yg.hahajie.cn

[J01] 获取当前时间
来源：http://ux.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ed.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://us.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://gx.521024.cn

TS:   new Date();  Date.now()
来源：http://zz.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gt.gzmigu.cn

Go:   time.Now()
来源：http://uu.521024.cn

Ruby: Time.now
来源：http://ou.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vi.chemitech.net.cn

[J02] 格式化输出
来源：http://nu.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ku.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oz.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hv.nicolike.cn

TS:   d.toISOString()
来源：http://lk.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pc.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xe.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lp.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bl.huanxung.cn

[J03] 字符串解析为日期
来源：http://zh.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qo.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://np.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://eg.asd995.cn

TS:   new Date("2024-01-02")
来源：http://rp.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gw.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xk.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://fc.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uw.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://hi.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nm.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://al.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nk.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cz.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mj.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nx.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ck.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zh.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://lu.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://ah.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vp.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://al.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ai.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://xe.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ih.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://me.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sv.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://iy.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://bm.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://ge.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uo.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wg.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ae.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://bq.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://dh.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://tg.huanxung.cn


<!-- 参考信息 -->