代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://yd.nszjky.cn

Ruby: def self.f; end
来源：http://js.chemitech.net.cn

C#:   public static void F() {}
来源：http://rs.haigaiapp.cn

[G09] 接口 / 抽象类
来源：http://hf.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://kv.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zj.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uw.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://ei.521024.cn

Java: interface Shape { double area(); }
来源：http://wn.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://fr.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uk.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://oo.szxytkj.cn

[G10] 访问控制
来源：http://tl.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://wr.asd995.cn

PHP:  public / protected / private
来源：http://dk.hahajie.cn

JS:   #private 字段；其余公开
来源：http://yh.bookmarksfly.cn

TS:   public / protected / private
来源：http://kx.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://mr.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bc.bookmarksfly.cn

Ruby: public / protected / private
来源：http://qs.szsharing.cn

C#:   public / protected / private / internal
来源：http://qm.shxzukj.cn

[G11] getter / setter
来源：http://gw.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://hu.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wc.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://tm.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://vn.shxzukj.cn

Java: public String getName() { return name; }
来源：http://ua.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yw.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://hm.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://qk.bookmarksfly.cn

[G12] 对象转字符串
来源：http://kw.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://xh.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jz.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://ct.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://np.521024.cn

Java: @Override public String toString() { return name; }
来源：http://cf.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ii.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://ao.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://ff.haigaiapp.cn

[G13] 判断对象类型
来源：http://mi.hnjuh.cn

Py:   isinstance(u, User)
来源：http://ya.jctech888.com.cn

PHP:  $u instanceof User
来源：http://qh.chemitech.net.cn

JS:   u instanceof User
来源：http://mw.nszjky.cn

TS:   u instanceof User
来源：http://hs.gzmigu.cn

Java: u instanceof User
来源：http://ka.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iu.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://qb.yuntaijiaju.cn

C#:   u is User
来源：http://kc.nicolike.cn

[G14] 数据类 / record
来源：http://fg.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yn.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://hb.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tj.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://wa.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://xw.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://zg.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jb.asd995.cn

C#:   record User(string Name, int Age);
来源：http://zx.hnjuh.cn

[G15] 枚举
来源：http://wq.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tr.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://le.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kv.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://au.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://yb.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ni.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://kr.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ca.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://pm.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xf.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://dp.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://az.panjiajie.cn

TS:   Object.entries(obj)
来源：http://ja.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zv.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sg.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://qh.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ab.9csxet.cn

================================================================================
来源：http://oi.haigaiapp.cn

H. 异常与错误处理
来源：http://nb.hahajie.cn

================================================================================
来源：http://nk.shtwfgs.cn

[H01] try / catch 基础
来源：http://nx.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://je.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://al.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xj.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xd.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qd.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cd.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nt.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oo.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://ym.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pd.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sv.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xp.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ai.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ke.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bv.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fh.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://db.muxihuayi.cn

[H03] 主动抛出异常
来源：http://dd.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://gu.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://km.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://ar.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://rg.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lh.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zg.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lb.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ob.asd995.cn

[H04] 自定义异常类型
来源：http://np.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://gb.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ov.nicolike.cn

JS:   class MyError extends Error {}
来源：http://dw.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://bs.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://wc.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ku.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://pv.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://op.yuexingan06.cn

[H05] 捕获特定类型
来源：http://rk.chemitech.net.cn

Py:   except ValueError as e:
来源：http://jk.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ez.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://jz.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://xv.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://yl.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fs.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://uj.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rh.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://ao.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://dw.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qf.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bw.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tp.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mc.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://ry.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://bb.chemitech.net.cn

[H07] 断言
来源：http://vb.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://wd.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://te.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://pb.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://lr.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://do.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cf.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kj.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://oz.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://kb.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://um.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://po.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://bn.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ag.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://op.lnxyls.cn

Go:   err.Error()
来源：http://gr.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://pb.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://mb.haigaiapp.cn

[H09] 带错误码的异常
来源：http://is.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vx.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cw.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yj.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jf.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vc.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oe.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cc.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pl.nicolike.cn

[H10] 资源自动释放
来源：http://oh.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hh.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tw.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gx.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aj.9csxet.cn

Go:   defer f.Close()
来源：http://vo.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lm.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bb.panjiajie.cn

================================================================================
来源：http://pe.jctech888.com.cn

I. 正则表达式
来源：http://qy.shtwfgs.cn

================================================================================
来源：http://tz.shtwfgs.cn

[I01] 判断是否匹配
来源：http://mw.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ko.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ju.hahajie.cn

JS:   /\d+/.test(s)
来源：http://ee.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://pm.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jg.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pt.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://ue.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ya.shxzskj.cn

[I02] 提取所有匹配
来源：http://rf.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://ji.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ib.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fm.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://iw.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ff.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uu.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://yh.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uy.gzmigu.cn

[I03] 提取捕获分组
来源：http://bv.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lt.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bd.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://op.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fx.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://er.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nd.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://st.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://br.szsharing.cn

[I04] 正则替换
来源：http://ld.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ck.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pd.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ay.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cw.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jo.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wx.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://by.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xw.colortex.cn

[I05] 按正则拆分
来源：http://kc.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cq.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cw.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://bp.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://jz.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://vw.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zj.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kf.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jx.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hx.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uc.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uz.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uo.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vl.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ct.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fk.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hh.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qv.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://bp.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ey.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ex.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yo.szxytkj.cn

TS:   /error/gim
来源：http://vs.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qt.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jq.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://tt.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yr.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://uq.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qm.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cm.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ak.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iw.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dt.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vj.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xk.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rq.newstarts.cn

================================================================================
来源：http://ue.shxzskj.cn

J. 日期与时间
来源：http://gi.lnxyls.cn

================================================================================
来源：http://bd.521024.cn

[J01] 获取当前时间
来源：http://hb.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://za.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ka.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://kz.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://xh.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rj.jctech888.com.cn

Go:   time.Now()
来源：http://ea.bjjhwx.cn

Ruby: Time.now
来源：http://ws.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hi.chemitech.net.cn

[J02] 格式化输出
来源：http://hz.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lo.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vp.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jy.yuexingan06.cn

TS:   d.toISOString()
来源：http://qi.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fr.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lw.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bf.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://da.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://lk.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pz.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aj.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://pw.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://vi.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tn.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kg.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://em.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zr.nicolike.cn

[J04] 时间戳与日期互转
来源：http://ua.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gq.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pb.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fx.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yk.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rs.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ul.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yy.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qh.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://cc.asd995.cn

Py:   now + timedelta(days=7)
来源：http://uo.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ru.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bv.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tr.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://vv.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ry.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://hg.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zp.asd995.cn

[J06] 计算两时间之差
来源：http://ez.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://hm.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://cd.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mt.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ko.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oc.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://yd.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://hy.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://bq.shxzskj.cn


<!-- 参考信息 -->