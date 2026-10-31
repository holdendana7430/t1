代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://cr.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kg.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cz.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://tt.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://ji.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://en.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rq.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://dj.shxzskj.cn

[G10] 访问控制
来源：http://ta.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://sw.newstarts.cn

PHP:  public / protected / private
来源：http://so.521024.cn

JS:   #private 字段；其余公开
来源：http://ba.9csxet.cn

TS:   public / protected / private
来源：http://li.521024.cn

Java: public / protected / private / 默认包级
来源：http://cb.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ll.huixiangedu.cn

Ruby: public / protected / private
来源：http://gh.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://qc.hahajie.cn

[G11] getter / setter
来源：http://rv.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ko.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wg.asd995.cn

JS:   get name() { return this._name; }
来源：http://un.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://bg.nszjky.cn

Java: public String getName() { return name; }
来源：http://bi.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ro.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://cf.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://ej.hnjuh.cn

[G12] 对象转字符串
来源：http://ec.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://ti.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sz.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://vr.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://xk.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://fa.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sg.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://ed.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://om.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://ji.asd995.cn

Py:   isinstance(u, User)
来源：http://ie.lnxyls.cn

PHP:  $u instanceof User
来源：http://ud.huixinmuqiang.cn

JS:   u instanceof User
来源：http://tf.521024.cn

TS:   u instanceof User
来源：http://ss.nicolike.cn

Java: u instanceof User
来源：http://ts.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zk.asd995.cn

Ruby: u.is_a?(User)
来源：http://hj.jctech888.com.cn

C#:   u is User
来源：http://dz.nicolike.cn

[G14] 数据类 / record
来源：http://iq.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qt.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://xf.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bs.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://ty.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://zx.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://mc.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cx.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://jg.shxzskj.cn

[G15] 枚举
来源：http://zi.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wp.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ld.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fi.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aq.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://ks.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pb.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://ch.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ij.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://ex.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sj.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://nw.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://bf.shxzukj.cn

TS:   Object.entries(obj)
来源：http://dj.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bs.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ac.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://dr.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://cl.huanxung.cn

================================================================================
来源：http://ia.shxzukj.cn

H. 异常与错误处理
来源：http://mm.szsharing.cn

================================================================================
来源：http://pf.nszjky.cn

[H01] try / catch 基础
来源：http://fz.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://si.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oi.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ie.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bi.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iy.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sd.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mc.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qq.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://nh.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vp.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pr.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pw.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sv.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ra.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rt.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gn.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lk.shtwfgs.cn

[H03] 主动抛出异常
来源：http://ao.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://wz.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kd.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://vx.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://tk.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tj.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mp.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gp.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ye.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://sm.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://ks.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pq.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://ie.hahajie.cn

TS:   class MyError extends Error {}
来源：http://uy.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://ax.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ko.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://rg.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://lg.colortex.cn

[H05] 捕获特定类型
来源：http://lu.haigaiapp.cn

Py:   except ValueError as e:
来源：http://hy.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qq.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://hv.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://tg.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ct.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qu.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://iu.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ja.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://wq.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://gv.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tz.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ch.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ql.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vz.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nu.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://aq.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://bz.huanxung.cn

[H07] 断言
来源：http://jp.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://qv.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://cp.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://zv.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://yd.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://dz.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mw.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rq.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://hc.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://en.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://tj.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gf.szxytkj.cn

JS:   e.message;  e.stack
来源：http://ez.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kk.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jn.haigaiapp.cn

Go:   err.Error()
来源：http://ut.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://sg.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://qw.panjiajie.cn

[H09] 带错误码的异常
来源：http://zy.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jh.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xp.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xy.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xh.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mt.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ge.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nv.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bw.jctech888.com.cn

[H10] 资源自动释放
来源：http://fs.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gz.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://om.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pn.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wg.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tv.huanxung.cn

Go:   defer f.Close()
来源：http://og.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hv.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nh.lnxyls.cn

================================================================================
来源：http://fp.haigaiapp.cn

I. 正则表达式
来源：http://jo.colortex.cn

================================================================================
来源：http://ft.panjiajie.cn

[I01] 判断是否匹配
来源：http://qt.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tt.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vf.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://gs.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://gb.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mc.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qz.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://hb.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lt.szsharing.cn

[I02] 提取所有匹配
来源：http://qc.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://ym.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://am.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fy.521024.cn

TS:   s.match(/\d+/g)
来源：http://ak.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ya.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uc.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://zo.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hi.shxzskj.cn

[I03] 提取捕获分组
来源：http://iw.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pj.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://io.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://em.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ba.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dn.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hm.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fk.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rw.panjiajie.cn

[I04] 正则替换
来源：http://ed.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kt.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xp.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ff.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ov.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yc.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wr.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://np.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aw.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://es.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ug.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wm.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://qm.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://gw.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://tu.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ei.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mo.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vn.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ic.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kp.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lg.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ok.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dj.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wl.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xs.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tm.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sv.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://fr.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xx.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://go.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wo.chemitech.net.cn

TS:   /error/gim
来源：http://xr.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oi.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pw.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://eb.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yr.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://lr.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pj.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mk.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dv.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xt.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hu.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bo.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lo.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cl.jianghongdianzi.cn

================================================================================
来源：http://ni.521024.cn

J. 日期与时间
来源：http://qi.newstarts.cn

================================================================================
来源：http://vt.chemitech.net.cn

[J01] 获取当前时间
来源：http://ld.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rr.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://re.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://xf.9csxet.cn

TS:   new Date();  Date.now()
来源：http://uf.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ov.asd995.cn

Go:   time.Now()
来源：http://td.521024.cn

Ruby: Time.now
来源：http://nw.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vy.haigaiapp.cn

[J02] 格式化输出
来源：http://vh.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://js.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yz.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yc.shxzukj.cn

TS:   d.toISOString()
来源：http://op.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zd.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ro.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uu.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ak.szsharing.cn

[J03] 字符串解析为日期
来源：http://ig.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ty.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fs.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://jc.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://gj.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ht.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qi.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://pa.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ns.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://ww.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://az.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://at.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oa.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vv.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tn.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iz.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://op.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yw.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://fo.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://kr.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ua.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hg.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pe.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://fk.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nb.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://pp.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rx.lnxyls.cn

[J06] 计算两时间之差
来源：http://pw.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://ao.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://ur.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cf.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yk.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bu.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://kw.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://fo.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://tb.colortex.cn

[J07] 比较两个日期
来源：http://uf.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://pb.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bk.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ss.lnxyls.cn


<!-- 参考信息 -->