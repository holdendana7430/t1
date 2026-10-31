代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://ub.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://of.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vi.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://qf.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://ax.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://pa.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hq.521024.cn

C#:   interface IShape { double Area(); }
来源：http://sc.wgjwhj.cn

[G10] 访问控制
来源：http://ug.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://ry.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://lg.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://bg.lnxyls.cn

TS:   public / protected / private
来源：http://wv.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://oq.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sj.hnjuh.cn

Ruby: public / protected / private
来源：http://en.huanxung.cn

C#:   public / protected / private / internal
来源：http://pu.yuexingan06.cn

[G11] getter / setter
来源：http://xu.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://mg.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iw.huanxung.cn

JS:   get name() { return this._name; }
来源：http://xu.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://el.nicolike.cn

Java: public String getName() { return name; }
来源：http://rn.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rm.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://is.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://kt.muxihuayi.cn

[G12] 对象转字符串
来源：http://pd.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://pn.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ui.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://ew.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://kr.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://uh.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://th.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://fm.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://rn.wgjwhj.cn

[G13] 判断对象类型
来源：http://xq.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://he.shtwfgs.cn

PHP:  $u instanceof User
来源：http://wc.9csxet.cn

JS:   u instanceof User
来源：http://mo.newstarts.cn

TS:   u instanceof User
来源：http://cl.huixiangedu.cn

Java: u instanceof User
来源：http://kz.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sd.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://vu.colortex.cn

C#:   u is User
来源：http://vf.wgjwhj.cn

[G14] 数据类 / record
来源：http://ox.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cr.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://hc.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dz.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://sk.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://dj.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://cs.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://en.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://gg.huanxung.cn

[G15] 枚举
来源：http://xg.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wp.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dh.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ct.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yb.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://eg.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ht.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://sb.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://py.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://qz.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uf.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://tm.huanxung.cn

JS:   Object.entries(obj)
来源：http://yh.newstarts.cn

TS:   Object.entries(obj)
来源：http://hs.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cj.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qh.newstarts.cn

Ruby: obj.instance_variables
来源：http://se.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://pi.shxzukj.cn

================================================================================
来源：http://om.gzmigu.cn

H. 异常与错误处理
来源：http://rv.huixiangedu.cn

================================================================================
来源：http://rm.colortex.cn

[H01] try / catch 基础
来源：http://dm.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kw.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bq.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ts.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jf.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cx.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dj.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dc.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vi.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://ac.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zg.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sx.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tm.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qj.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ol.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://un.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lr.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://th.521024.cn

[H03] 主动抛出异常
来源：http://oq.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://nz.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ll.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://av.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://hd.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ru.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mr.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qc.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://um.huanxung.cn

[H04] 自定义异常类型
来源：http://vz.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://wv.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wr.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://cl.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://tl.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://rp.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ym.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://pv.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://cm.muxihuayi.cn

[H05] 捕获特定类型
来源：http://ti.521024.cn

Py:   except ValueError as e:
来源：http://og.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rm.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://oz.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://bb.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://cr.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://py.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://ju.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nu.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://oj.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://re.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vz.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sf.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mm.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bw.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ga.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://bp.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://zq.szsharing.cn

[H07] 断言
来源：http://to.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://lm.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://xt.hahajie.cn

JS:   console.assert(x > 0);
来源：http://lw.9csxet.cn

TS:   console.assert(x > 0);
来源：http://wg.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://ba.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bq.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xu.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://pi.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://ij.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://un.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ox.nicolike.cn

JS:   e.message;  e.stack
来源：http://ju.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mv.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xp.szsharing.cn

Go:   err.Error()
来源：http://yc.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://oo.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://pl.colortex.cn

[H09] 带错误码的异常
来源：http://fk.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tb.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sa.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mp.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sn.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://za.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ta.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fz.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ya.shxzukj.cn

[H10] 资源自动释放
来源：http://ba.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rj.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oe.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://so.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vl.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zh.wgjwhj.cn

Go:   defer f.Close()
来源：http://ai.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nh.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fp.asd995.cn

================================================================================
来源：http://kf.panjiajie.cn

I. 正则表达式
来源：http://cz.gzmigu.cn

================================================================================
来源：http://xk.lnxyls.cn

[I01] 判断是否匹配
来源：http://jw.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bx.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ku.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://cp.nicolike.cn

TS:   /\d+/.test(s)
来源：http://ts.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zo.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ya.521024.cn

Ruby: s.match?(/\d+/)
来源：http://yw.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gd.shxzskj.cn

[I02] 提取所有匹配
来源：http://sd.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://zx.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wd.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ik.asd995.cn

TS:   s.match(/\d+/g)
来源：http://pk.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ab.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ah.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://yu.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fg.szxytkj.cn

[I03] 提取捕获分组
来源：http://lm.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ez.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dj.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tj.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://co.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sy.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://te.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ef.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sp.hahajie.cn

[I04] 正则替换
来源：http://bb.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cf.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fd.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zz.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qi.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tl.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ve.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kt.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tf.huixiangedu.cn

[I05] 按正则拆分
来源：http://rh.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ux.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fc.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://kb.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://nv.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://zb.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zi.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://px.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://br.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fc.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zv.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zm.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fk.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ny.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rb.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cs.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lt.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://go.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://oc.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vx.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ji.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://je.szxytkj.cn

TS:   /error/gim
来源：http://an.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dc.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bz.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://zd.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://va.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ov.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kn.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tb.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://df.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://en.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ms.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ek.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pk.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gs.nszjky.cn

================================================================================
来源：http://ws.9csxet.cn

J. 日期与时间
来源：http://xe.huixiangedu.cn

================================================================================
来源：http://ot.lnxyls.cn

[J01] 获取当前时间
来源：http://yi.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bu.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mc.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://ku.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://se.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://on.szsharing.cn

Go:   time.Now()
来源：http://ai.huanxung.cn

Ruby: Time.now
来源：http://tt.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vc.gzmigu.cn

[J02] 格式化输出
来源：http://mf.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wa.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ut.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ms.szsharing.cn

TS:   d.toISOString()
来源：http://xy.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ex.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wo.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pa.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xk.shxzukj.cn

[J03] 字符串解析为日期
来源：http://bg.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pn.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://al.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://kg.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://nl.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hz.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://to.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://vc.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wi.colortex.cn

[J04] 时间戳与日期互转
来源：http://rt.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jw.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tt.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ni.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cx.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ld.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://he.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ec.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ia.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://dd.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://kw.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mg.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gh.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fq.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://ez.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kg.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://um.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xn.huanxung.cn

[J06] 计算两时间之差
来源：http://sh.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://rs.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://li.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tz.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gf.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://li.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://zd.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://qe.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://xl.newstarts.cn

[J07] 比较两个日期
来源：http://jw.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://wo.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hh.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://to.9csxet.cn


<!-- 参考信息 -->