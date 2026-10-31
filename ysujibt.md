代发 wailian999

JS:   get name() { return this._name; }
来源：http://rz.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://so.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://oc.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hh.szxytkj.cn

Ruby: attr_accessor :name
来源：http://pk.huanxung.cn

C#:   public string Name { get; set; }
来源：http://zv.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://qu.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://ey.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://di.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://ko.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://sb.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://br.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vz.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://dw.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://yk.szsharing.cn

[G13] 判断对象类型
来源：http://ws.lnxyls.cn

Py:   isinstance(u, User)
来源：http://yp.jctech888.com.cn

PHP:  $u instanceof User
来源：http://dh.shxzukj.cn

JS:   u instanceof User
来源：http://fi.bookmarksfly.cn

TS:   u instanceof User
来源：http://xr.shtwfgs.cn

Java: u instanceof User
来源：http://wr.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vr.huanxung.cn

Ruby: u.is_a?(User)
来源：http://bd.gzmigu.cn

C#:   u is User
来源：http://nz.wgjwhj.cn

[G14] 数据类 / record
来源：http://eb.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dt.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://nb.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ka.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://qt.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://ao.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://av.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zg.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://ko.szxytkj.cn

[G15] 枚举
来源：http://zx.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mz.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://av.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lv.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sg.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://aa.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mk.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://ty.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gy.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://kn.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fb.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://fr.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://qn.hnjuh.cn

TS:   Object.entries(obj)
来源：http://ks.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sq.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ri.szsharing.cn

Ruby: obj.instance_variables
来源：http://qm.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://dl.szsharing.cn

================================================================================
来源：http://ih.huanxung.cn

H. 异常与错误处理
来源：http://on.bookmarksfly.cn

================================================================================
来源：http://cg.shxzskj.cn

[H01] try / catch 基础
来源：http://wb.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zw.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pc.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rc.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wc.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xg.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jb.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://an.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tg.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://hz.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sh.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hb.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ee.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ba.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rc.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eu.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wo.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zf.shxzskj.cn

[H03] 主动抛出异常
来源：http://do.521024.cn

Py:   raise ValueError("错误信息")
来源：http://dk.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vv.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://nt.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://qx.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rs.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ul.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://am.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qj.haigaiapp.cn

[H04] 自定义异常类型
来源：http://zp.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://mx.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://za.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://he.newstarts.cn

TS:   class MyError extends Error {}
来源：http://pp.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://nt.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kn.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://zd.521024.cn

C#:   class MyException : Exception {}
来源：http://uq.yuexingan06.cn

[H05] 捕获特定类型
来源：http://nq.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://sk.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gl.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://fx.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://vu.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://qk.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xc.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://ka.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wh.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://gp.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://vv.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qp.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ix.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://de.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wq.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://at.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://ff.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://px.bjjhwx.cn

[H07] 断言
来源：http://oh.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://gp.szxytkj.cn

PHP:  assert($x > 0);
来源：http://ee.hahajie.cn

JS:   console.assert(x > 0);
来源：http://kf.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://bh.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://qv.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://af.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://el.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://jp.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://xh.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://pm.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xz.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://kp.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gs.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yf.asd995.cn

Go:   err.Error()
来源：http://ap.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://cn.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://bb.haigaiapp.cn

[H09] 带错误码的异常
来源：http://wx.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dx.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xx.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fl.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cm.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tl.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ca.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hs.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://af.bjjhwx.cn

[H10] 资源自动释放
来源：http://xe.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ux.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://es.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kk.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rs.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ak.huanxung.cn

Go:   defer f.Close()
来源：http://fa.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dj.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://of.haigaiapp.cn

================================================================================
来源：http://ib.lnxyls.cn

I. 正则表达式
来源：http://ob.yuexingan06.cn

================================================================================
来源：http://xg.huixiangedu.cn

[I01] 判断是否匹配
来源：http://nm.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bq.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://re.hahajie.cn

JS:   /\d+/.test(s)
来源：http://ri.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://wu.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://co.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tx.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://xi.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kb.hahajie.cn

[I02] 提取所有匹配
来源：http://ug.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://tf.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dh.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ii.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://bh.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://or.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ve.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://wv.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cn.yuexingan06.cn

[I03] 提取捕获分组
来源：http://cn.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iy.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nn.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kb.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ca.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xd.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pi.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yh.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wgjwhj.cn

[I04] 正则替换
来源：http://dk.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kt.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hs.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vy.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lx.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ie.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ot.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vo.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://be.hnjuh.cn

[I05] 按正则拆分
来源：http://ph.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xt.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xj.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://bs.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://pi.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://al.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lx.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qv.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fh.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bh.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://br.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xf.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vn.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zy.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qu.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://be.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://az.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zo.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ts.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fq.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://la.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qq.nicolike.cn

TS:   /error/gim
来源：http://ej.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ia.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hc.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://xj.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fa.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://pr.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xf.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ur.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nu.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hu.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rm.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ym.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yt.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wr.hnjuh.cn

================================================================================
来源：http://nq.huixiangedu.cn

J. 日期与时间
来源：http://vj.nicolike.cn

================================================================================
来源：http://xc.nszjky.cn

[J01] 获取当前时间
来源：http://vu.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ox.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oa.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://sw.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://lu.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jb.wgjwhj.cn

Go:   time.Now()
来源：http://ua.szsharing.cn

Ruby: Time.now
来源：http://te.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zv.huanxung.cn

[J02] 格式化输出
来源：http://sw.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ag.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yp.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tf.shxzukj.cn

TS:   d.toISOString()
来源：http://ot.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bq.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sy.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gz.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cp.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://mq.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vh.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uk.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://pa.521024.cn

TS:   new Date("2024-01-02")
来源：http://fm.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://en.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nk.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://mg.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ws.huanxung.cn

[J04] 时间戳与日期互转
来源：http://uv.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ne.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dm.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gq.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zy.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wj.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://do.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bc.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ef.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://gn.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://ha.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uw.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yn.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sd.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://em.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rg.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://hw.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xu.shxzskj.cn

[J06] 计算两时间之差
来源：http://em.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://lt.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://fd.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://je.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cj.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uy.521024.cn

Go:   end.Sub(start).Hours()
来源：http://jv.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://fh.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://dq.panjiajie.cn

[J07] 比较两个日期
来源：http://dw.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://mm.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lu.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vp.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kr.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ry.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lt.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yq.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://tb.shxzskj.cn

[J08] 提取年月日与星期
来源：http://bd.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tv.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tm.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qc.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yg.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xn.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hw.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fr.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ju.521024.cn

[J09] 时区处理
来源：http://pi.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bq.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eg.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pa.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qd.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vi.szxytkj.cn


<!-- 参考信息 -->