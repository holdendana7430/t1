代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://ll.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://rd.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://yn.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://ak.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nz.hahajie.cn

Ruby: def to_s; @name; end
来源：http://qt.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://gx.jctech888.com.cn

[G13] 判断对象类型
来源：http://ht.szsharing.cn

Py:   isinstance(u, User)
来源：http://jx.muxihuayi.cn

PHP:  $u instanceof User
来源：http://rr.szsharing.cn

JS:   u instanceof User
来源：http://yk.nszjky.cn

TS:   u instanceof User
来源：http://mi.yuntaijiaju.cn

Java: u instanceof User
来源：http://fr.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ty.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://sa.szsharing.cn

C#:   u is User
来源：http://rw.yuexingan06.cn

[G14] 数据类 / record
来源：http://hh.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rw.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://oa.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oe.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://rg.nszjky.cn

Java: record User(String name, int age) {}
来源：http://wr.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://ex.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sd.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://tr.hahajie.cn

[G15] 枚举
来源：http://go.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gx.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ud.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nl.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rm.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://pe.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oc.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://om.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nt.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://vg.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dp.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://ev.panjiajie.cn

JS:   Object.entries(obj)
来源：http://mo.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://xr.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://en.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dg.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://im.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://qq.huixiangedu.cn

================================================================================
来源：http://ma.panjiajie.cn

H. 异常与错误处理
来源：http://yw.nszjky.cn

================================================================================
来源：http://ks.nszjky.cn

[H01] try / catch 基础
来源：http://xs.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nh.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ta.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://by.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hg.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bo.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sl.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sz.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zt.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://pz.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jq.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ct.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ct.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qd.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tg.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cr.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ug.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hi.jctech888.com.cn

[H03] 主动抛出异常
来源：http://qi.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://tl.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oi.colortex.cn

JS:   throw new Error("错误信息");
来源：http://af.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://fg.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xz.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jh.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xr.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xa.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://fx.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://qk.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vm.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://lw.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://bl.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://ly.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://td.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://si.colortex.cn

C#:   class MyException : Exception {}
来源：http://ly.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://rv.panjiajie.cn

Py:   except ValueError as e:
来源：http://io.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uf.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://zc.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://kf.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://ts.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rr.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://gt.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pv.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://ql.huanxung.cn

Py:   value = d.get("k") or default
来源：http://fx.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ea.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hq.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://na.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qw.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xe.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://uj.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://dj.shxzskj.cn

[H07] 断言
来源：http://ye.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://bb.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://nc.nszjky.cn

JS:   console.assert(x > 0);
来源：http://ah.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://kg.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://mb.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hv.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mt.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://re.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://to.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://kd.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rz.gzmigu.cn

JS:   e.message;  e.stack
来源：http://ts.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yf.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yf.lnxyls.cn

Go:   err.Error()
来源：http://jc.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://dm.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://yz.wgjwhj.cn

[H09] 带错误码的异常
来源：http://oe.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hu.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gx.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wi.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ge.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kw.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xb.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gs.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pc.muxihuayi.cn

[H10] 资源自动释放
来源：http://bh.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vt.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gj.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://is.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lm.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vl.huanxung.cn

Go:   defer f.Close()
来源：http://eh.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vr.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://au.bjjhwx.cn

================================================================================
来源：http://hs.jctech888.com.cn

I. 正则表达式
来源：http://xo.haigaiapp.cn

================================================================================
来源：http://de.nszjky.cn

[I01] 判断是否匹配
来源：http://ru.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ir.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uw.colortex.cn

JS:   /\d+/.test(s)
来源：http://lr.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://xv.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pz.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tq.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://gl.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zw.shxzukj.cn

[I02] 提取所有匹配
来源：http://hv.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://lp.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://km.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nn.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://vr.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xt.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zq.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://rd.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pf.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://rg.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dn.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qu.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yq.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ym.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://to.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yq.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fx.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zq.panjiajie.cn

[I04] 正则替换
来源：http://wp.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dy.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pq.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xj.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rt.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sh.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mv.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ju.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sw.szsharing.cn

[I05] 按正则拆分
来源：http://ld.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://we.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mm.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://pa.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://qr.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://or.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pc.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tm.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gz.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xo.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pc.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yb.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mj.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yb.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jy.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nh.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pu.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ht.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://gs.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yw.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xo.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bt.yuntaijiaju.cn

TS:   /error/gim
来源：http://dx.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ve.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xi.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://rn.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ys.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://oo.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jg.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ay.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sj.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pt.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qb.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fx.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ar.newstarts.cn

================================================================================
来源：http://mj.jctech888.com.cn

J. 日期与时间
来源：http://ix.szxytkj.cn

================================================================================
来源：http://yv.panjiajie.cn

[J01] 获取当前时间
来源：http://zh.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ft.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ts.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://ce.nicolike.cn

TS:   new Date();  Date.now()
来源：http://wi.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gv.nszjky.cn

Go:   time.Now()
来源：http://kz.jianghongdianzi.cn

Ruby: Time.now
来源：http://fj.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nb.huixiangedu.cn

[J02] 格式化输出
来源：http://ua.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qk.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://la.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bn.chemitech.net.cn

TS:   d.toISOString()
来源：http://fc.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://os.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wx.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tv.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rn.newstarts.cn

[J03] 字符串解析为日期
来源：http://km.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lr.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ku.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://em.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://ny.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tm.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jd.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://kf.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sp.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://hw.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xt.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nn.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bm.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://po.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ru.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pu.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://el.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tu.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://ar.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://jq.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jd.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ug.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oy.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://kg.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ef.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://nx.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fo.yuexingan06.cn

[J06] 计算两时间之差
来源：http://ne.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://ih.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://kl.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ah.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oa.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iz.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://ga.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://dy.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://nn.colortex.cn

[J07] 比较两个日期
来源：http://eb.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://du.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zg.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lf.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mm.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gs.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mh.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rp.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://dm.panjiajie.cn

[J08] 提取年月日与星期
来源：http://co.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ur.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vo.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qp.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zg.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xn.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://in.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ff.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gv.huanxung.cn

[J09] 时区处理
来源：http://wl.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://em.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iz.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fh.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qg.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gt.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gp.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jg.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wa.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://sc.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://af.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tk.chemitech.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ov.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sf.lnxyls.cn


<!-- 参考信息 -->