代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wx.chemitech.net.cn

Ruby: def self.f; end
来源：http://lu.shtwfgs.cn

C#:   public static void F() {}
来源：http://qe.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://vt.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://ps.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fc.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://br.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://lk.asd995.cn

Java: interface Shape { double area(); }
来源：http://hm.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://jd.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yc.521024.cn

C#:   interface IShape { double Area(); }
来源：http://ns.yuntaijiaju.cn

[G10] 访问控制
来源：http://ed.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://ut.jctech888.com.cn

PHP:  public / protected / private
来源：http://dk.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://xw.shxzukj.cn

TS:   public / protected / private
来源：http://su.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://fd.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xj.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://mk.szsharing.cn

C#:   public / protected / private / internal
来源：http://kx.jianghongdianzi.cn

[G11] getter / setter
来源：http://ta.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://ye.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cz.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://cg.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://rd.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://gw.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pb.colortex.cn

Ruby: attr_accessor :name
来源：http://bd.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://cl.muxihuayi.cn

[G12] 对象转字符串
来源：http://bb.521024.cn

Py:   def __str__(self): return self.name
来源：http://ap.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qe.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://vy.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://pe.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://vt.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mq.newstarts.cn

Ruby: def to_s; @name; end
来源：http://iq.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://zv.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://ju.shxzukj.cn

Py:   isinstance(u, User)
来源：http://jx.hahajie.cn

PHP:  $u instanceof User
来源：http://fs.chemitech.net.cn

JS:   u instanceof User
来源：http://kh.bookmarksfly.cn

TS:   u instanceof User
来源：http://qf.wgjwhj.cn

Java: u instanceof User
来源：http://jc.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ks.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://cx.shxzskj.cn

C#:   u is User
来源：http://fm.yuexingan06.cn

[G14] 数据类 / record
来源：http://io.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aw.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://ib.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rw.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://jq.newstarts.cn

Java: record User(String name, int age) {}
来源：http://rt.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://op.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rc.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://lm.colortex.cn

[G15] 枚举
来源：http://av.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uh.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pk.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ao.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uz.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://pi.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nm.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://sa.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wl.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://cw.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sl.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://sh.521024.cn

JS:   Object.entries(obj)
来源：http://yt.gzmigu.cn

TS:   Object.entries(obj)
来源：http://kv.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ox.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ph.hnjuh.cn

Ruby: obj.instance_variables
来源：http://tq.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://vc.bookmarksfly.cn

================================================================================
来源：http://de.huixinmuqiang.cn

H. 异常与错误处理
来源：http://rf.lnxyls.cn

================================================================================
来源：http://mr.bjjhwx.cn

[H01] try / catch 基础
来源：http://ef.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sx.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://he.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qo.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://up.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ex.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iv.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gz.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ze.colortex.cn

[H02] finally / ensure 收尾
来源：http://dc.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gw.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mm.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jw.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oo.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rw.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bn.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tz.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gi.haigaiapp.cn

[H03] 主动抛出异常
来源：http://kv.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://jj.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gx.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://kh.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://jb.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bh.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qo.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mf.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://el.asd995.cn

[H04] 自定义异常类型
来源：http://qo.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://hf.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zc.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://lk.521024.cn

TS:   class MyError extends Error {}
来源：http://kq.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://ze.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aq.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://dr.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://yv.muxihuayi.cn

[H05] 捕获特定类型
来源：http://yr.wgjwhj.cn

Py:   except ValueError as e:
来源：http://qg.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://za.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://oe.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://vo.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://ed.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vn.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://gj.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://za.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://nl.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://yx.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rk.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jb.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tf.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pc.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pa.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://cc.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://mb.colortex.cn

[H07] 断言
来源：http://mj.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://os.huanxung.cn

PHP:  assert($x > 0);
来源：http://rj.huanxung.cn

JS:   console.assert(x > 0);
来源：http://in.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://vr.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://tu.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rw.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vu.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://im.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://kq.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://gq.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ar.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://oe.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yf.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mv.asd995.cn

Go:   err.Error()
来源：http://uh.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://lh.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://qq.wgjwhj.cn

[H09] 带错误码的异常
来源：http://tt.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kj.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ew.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gq.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ra.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vt.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ma.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tj.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zt.huanxung.cn

[H10] 资源自动释放
来源：http://jt.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ko.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wf.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ya.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ea.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jm.521024.cn

Go:   defer f.Close()
来源：http://yl.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rj.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ud.haigaiapp.cn

================================================================================
来源：http://iu.521024.cn

I. 正则表达式
来源：http://po.nicolike.cn

================================================================================
来源：http://in.szsharing.cn

[I01] 判断是否匹配
来源：http://za.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qi.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://el.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://zn.colortex.cn

TS:   /\d+/.test(s)
来源：http://ws.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tg.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qd.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://pn.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wv.szsharing.cn

[I02] 提取所有匹配
来源：http://bb.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://lk.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gh.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qj.asd995.cn

TS:   s.match(/\d+/g)
来源：http://cj.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lh.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vq.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://or.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xo.huixiangedu.cn

[I03] 提取捕获分组
来源：http://nn.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pf.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xw.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lr.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://os.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://af.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xs.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ks.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nd.bjjhwx.cn

[I04] 正则替换
来源：http://zn.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hf.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jz.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eg.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xw.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ga.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lk.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rj.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ol.colortex.cn

[I05] 按正则拆分
来源：http://sr.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vo.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://qp.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://ak.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://pl.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ge.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ie.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cc.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cq.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lt.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fz.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wd.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vk.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jp.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dz.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://in.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://or.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://ar.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rh.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qr.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dv.jianghongdianzi.cn

TS:   /error/gim
来源：http://tx.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yy.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bb.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://tm.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ss.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://na.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aq.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rg.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yh.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wq.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kq.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xf.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ed.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mo.lnxyls.cn

================================================================================
来源：http://fx.huanxung.cn

J. 日期与时间
来源：http://ot.asd995.cn

================================================================================
来源：http://fz.haigaiapp.cn

[J01] 获取当前时间
来源：http://qc.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vl.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dp.hahajie.cn

JS:   new Date();  Date.now()
来源：http://kb.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ux.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://de.bookmarksfly.cn

Go:   time.Now()
来源：http://xn.colortex.cn

Ruby: Time.now
来源：http://py.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pz.huanxung.cn

[J02] 格式化输出
来源：http://vh.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wn.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dh.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fq.hahajie.cn

TS:   d.toISOString()
来源：http://ef.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xa.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ro.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nc.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lg.szxytkj.cn

[J03] 字符串解析为日期
来源：http://ad.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fb.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rb.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://fu.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://gp.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yy.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://st.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://bv.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qx.newstarts.cn

[J04] 时间戳与日期互转
来源：http://vy.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fy.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fq.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rz.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mo.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ww.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://es.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ah.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://el.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://ie.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://iu.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eb.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ir.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xy.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://mj.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nf.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://fj.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bb.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://nz.521024.cn

Py:   (end - start).total_seconds()
来源：http://wa.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://gc.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ca.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xz.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rz.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://dp.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://hj.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://xp.bjjhwx.cn


<!-- 参考信息 -->