代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://do.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://xk.521024.cn

TS:   toString(): string { return this.name; }
来源：http://zb.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://ff.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wl.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://sr.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://ud.huanxung.cn

[G13] 判断对象类型
来源：http://sb.szxytkj.cn

Py:   isinstance(u, User)
来源：http://lm.yuexingan06.cn

PHP:  $u instanceof User
来源：http://au.bookmarksfly.cn

JS:   u instanceof User
来源：http://tc.nicolike.cn

TS:   u instanceof User
来源：http://in.huixinmuqiang.cn

Java: u instanceof User
来源：http://rw.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zw.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://iw.521024.cn

C#:   u is User
来源：http://bl.shtwfgs.cn

[G14] 数据类 / record
来源：http://of.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tp.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://iz.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bo.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://nb.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://od.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://kr.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rv.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://xw.szxytkj.cn

[G15] 枚举
来源：http://tc.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gw.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mt.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rj.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vp.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://so.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dj.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://sa.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rz.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://rf.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pp.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://qc.9csxet.cn

JS:   Object.entries(obj)
来源：http://fn.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://yl.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qf.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yt.shxzukj.cn

Ruby: obj.instance_variables
来源：http://to.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://mq.chemitech.net.cn

================================================================================
来源：http://ck.lnxyls.cn

H. 异常与错误处理
来源：http://mv.nicolike.cn

================================================================================
来源：http://yj.bjjhwx.cn

[H01] try / catch 基础
来源：http://qs.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ec.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tb.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cu.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bq.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://px.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zy.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hm.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xa.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://vx.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wk.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sb.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wj.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jd.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://op.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rk.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ta.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dl.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://wq.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://qs.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://li.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://ks.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://ci.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sr.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ce.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ch.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qn.wgjwhj.cn

[H04] 自定义异常类型
来源：http://kk.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://ui.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jx.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://ip.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ep.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://tm.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://td.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://ay.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://qf.yuexingan06.cn

[H05] 捕获特定类型
来源：http://tx.521024.cn

Py:   except ValueError as e:
来源：http://ep.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rz.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://to.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://ik.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://om.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mb.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://hn.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://td.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://pj.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://li.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mm.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zo.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ae.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yq.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wu.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://ji.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://xw.nicolike.cn

[H07] 断言
来源：http://ae.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://qu.nszjky.cn

PHP:  assert($x > 0);
来源：http://bt.asd995.cn

JS:   console.assert(x > 0);
来源：http://np.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://ww.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://ba.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uy.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pa.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ox.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://na.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://oh.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lz.hnjuh.cn

JS:   e.message;  e.stack
来源：http://wm.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mh.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kw.nszjky.cn

Go:   err.Error()
来源：http://wc.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://rm.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://tb.shtwfgs.cn

[H09] 带错误码的异常
来源：http://tp.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ah.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ad.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eh.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pk.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ah.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zu.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oe.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xa.521024.cn

[H10] 资源自动释放
来源：http://tr.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xy.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ex.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mh.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cj.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wx.shxzskj.cn

Go:   defer f.Close()
来源：http://et.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fd.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ca.yuntaijiaju.cn

================================================================================
来源：http://yc.colortex.cn

I. 正则表达式
来源：http://zo.hnjuh.cn

================================================================================
来源：http://wi.lnxyls.cn

[I01] 判断是否匹配
来源：http://ip.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ld.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gu.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://ol.521024.cn

TS:   /\d+/.test(s)
来源：http://xe.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zg.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kj.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://fp.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yh.nszjky.cn

[I02] 提取所有匹配
来源：http://vl.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://jw.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qi.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ij.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://qs.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ki.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bp.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://mq.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lr.9csxet.cn

[I03] 提取捕获分组
来源：http://zs.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ml.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ps.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fc.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://go.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lc.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hi.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ym.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://db.521024.cn

[I04] 正则替换
来源：http://eo.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nu.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ug.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oy.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kp.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sz.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fo.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://py.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ls.wgjwhj.cn

[I05] 按正则拆分
来源：http://vf.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mf.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qf.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://ij.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ca.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://rq.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rj.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cl.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://su.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ri.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zx.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bz.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zq.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oi.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yj.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mi.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uc.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://rr.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jr.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tw.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zb.szxytkj.cn

TS:   /error/gim
来源：http://yv.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uq.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ue.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://pt.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cj.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://vt.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://in.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sq.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gg.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://en.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dd.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ma.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rc.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fs.wgjwhj.cn

================================================================================
来源：http://ib.chemitech.net.cn

J. 日期与时间
来源：http://vj.bookmarksfly.cn

================================================================================
来源：http://dr.bjjhwx.cn

[J01] 获取当前时间
来源：http://qf.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://it.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dn.nszjky.cn

JS:   new Date();  Date.now()
来源：http://ab.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://zx.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ue.newstarts.cn

Go:   time.Now()
来源：http://hh.jctech888.com.cn

Ruby: Time.now
来源：http://tw.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bg.haigaiapp.cn

[J02] 格式化输出
来源：http://ng.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pl.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ka.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gw.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://nv.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hg.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vj.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://la.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://do.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://wp.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iz.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vu.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://zl.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://za.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hn.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qe.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://qj.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wu.newstarts.cn

[J04] 时间戳与日期互转
来源：http://hk.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vk.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rj.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://do.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fq.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tt.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bf.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pm.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hy.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://am.asd995.cn

Py:   now + timedelta(days=7)
来源：http://fg.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://as.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://in.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eo.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://mq.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lo.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://gy.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kh.wgjwhj.cn

[J06] 计算两时间之差
来源：http://ae.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://wx.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://jy.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aa.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fl.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fa.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://xn.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://qn.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://zp.muxihuayi.cn

[J07] 比较两个日期
来源：http://re.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://hc.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qp.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xg.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qg.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zb.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sp.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cw.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://tj.9csxet.cn

[J08] 提取年月日与星期
来源：http://ab.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rw.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tp.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xk.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kh.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sf.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gf.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vr.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sa.9csxet.cn

[J09] 时区处理
来源：http://tw.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tu.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://es.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://po.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://me.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dj.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ap.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gs.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ur.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vz.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ez.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dr.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ux.newstarts.cn


<!-- 参考信息 -->