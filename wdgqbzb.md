代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://ke.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://dr.colortex.cn

C#:   public override string ToString() => Name;
来源：http://ni.yuexingan06.cn

[G13] 判断对象类型
来源：http://ke.newstarts.cn

Py:   isinstance(u, User)
来源：http://wh.haigaiapp.cn

PHP:  $u instanceof User
来源：http://fe.shxzukj.cn

JS:   u instanceof User
来源：http://um.521024.cn

TS:   u instanceof User
来源：http://rt.nicolike.cn

Java: u instanceof User
来源：http://cq.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bm.colortex.cn

Ruby: u.is_a?(User)
来源：http://na.shxzskj.cn

C#:   u is User
来源：http://nc.wgjwhj.cn

[G14] 数据类 / record
来源：http://py.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ff.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://az.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yn.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://vi.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://uv.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://yf.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wm.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://qt.yuexingan06.cn

[G15] 枚举
来源：http://ym.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://se.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xe.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zi.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://em.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://cj.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://to.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://fb.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://la.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://zx.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zj.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://qa.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://ky.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://sd.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xo.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mr.hnjuh.cn

Ruby: obj.instance_variables
来源：http://zr.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://zh.shtwfgs.cn

================================================================================
来源：http://av.shxzskj.cn

H. 异常与错误处理
来源：http://yr.hnjuh.cn

================================================================================
来源：http://bx.szsharing.cn

[H01] try / catch 基础
来源：http://ed.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sl.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ul.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ua.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ij.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dg.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lg.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yo.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kk.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://tl.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qy.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gl.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yb.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://so.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yl.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ke.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oz.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gq.shxzukj.cn

[H03] 主动抛出异常
来源：http://rq.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://yx.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bs.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://el.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://it.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fy.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xa.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uc.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kg.nicolike.cn

[H04] 自定义异常类型
来源：http://dw.521024.cn

Py:   class MyError(Exception): pass
来源：http://wa.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ho.nszjky.cn

JS:   class MyError extends Error {}
来源：http://ep.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://of.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://qy.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lv.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://zq.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://fo.haigaiapp.cn

[H05] 捕获特定类型
来源：http://pu.jctech888.com.cn

Py:   except ValueError as e:
来源：http://lj.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://js.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ec.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://zn.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://rp.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tn.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://dx.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://st.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://lf.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://jb.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xp.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ej.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://po.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://se.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fh.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://dw.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://nu.colortex.cn

[H07] 断言
来源：http://ns.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://cb.panjiajie.cn

PHP:  assert($x > 0);
来源：http://rs.szsharing.cn

JS:   console.assert(x > 0);
来源：http://yf.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://cm.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://fc.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rm.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zp.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://in.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://rx.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://py.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xr.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://jw.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qx.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tq.bjjhwx.cn

Go:   err.Error()
来源：http://de.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://aw.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://bv.nicolike.cn

[H09] 带错误码的异常
来源：http://bd.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dq.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zz.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tl.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ih.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dp.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://td.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eh.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zl.colortex.cn

[H10] 资源自动释放
来源：http://ll.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vb.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kn.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cx.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qr.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bf.panjiajie.cn

Go:   defer f.Close()
来源：http://fg.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vy.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rp.jianghongdianzi.cn

================================================================================
来源：http://mt.yuntaijiaju.cn

I. 正则表达式
来源：http://hv.jctech888.com.cn

================================================================================
来源：http://at.szsharing.cn

[I01] 判断是否匹配
来源：http://ao.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://or.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pq.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://sa.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://fa.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wc.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dm.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://wu.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vg.szsharing.cn

[I02] 提取所有匹配
来源：http://gd.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://ta.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eu.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cb.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://jb.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vw.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zh.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://ng.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fl.shtwfgs.cn

[I03] 提取捕获分组
来源：http://ys.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qi.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iv.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ec.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bv.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://li.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dl.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gx.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://za.lnxyls.cn

[I04] 正则替换
来源：http://id.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lv.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yu.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ba.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://at.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xd.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://iv.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rp.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kx.newstarts.cn

[I05] 按正则拆分
来源：http://jb.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hf.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yr.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://xd.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ey.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://pi.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mt.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bt.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kz.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pq.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qa.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qb.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aq.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yq.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hn.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aw.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uj.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nh.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://sv.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ix.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ow.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ci.chemitech.net.cn

TS:   /error/gim
来源：http://nv.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xo.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ys.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://tj.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mg.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://zq.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://du.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bc.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bm.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pb.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kg.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uj.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oq.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zg.shtwfgs.cn

================================================================================
来源：http://wu.bjjhwx.cn

J. 日期与时间
来源：http://ln.yuexingan06.cn

================================================================================
来源：http://sm.wgjwhj.cn

[J01] 获取当前时间
来源：http://kc.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iv.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://td.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://cv.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://gt.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ji.hnjuh.cn

Go:   time.Now()
来源：http://ap.asd995.cn

Ruby: Time.now
来源：http://bq.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kl.yuntaijiaju.cn

[J02] 格式化输出
来源：http://bw.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pa.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nt.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qh.huanxung.cn

TS:   d.toISOString()
来源：http://ht.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://st.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dw.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ih.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cu.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://si.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cu.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gb.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://dh.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://eh.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mq.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ah.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://xd.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wo.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ng.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gg.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://he.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gl.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uy.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hu.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qn.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lg.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sd.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://gf.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://su.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bj.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hq.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oe.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://zs.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xx.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ij.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ew.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://fe.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://xu.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://cn.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xj.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://by.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qj.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://rf.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://rj.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://dc.colortex.cn

[J07] 比较两个日期
来源：http://jn.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://el.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sg.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://do.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rr.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fe.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qs.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xw.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ww.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://ss.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ue.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cg.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fo.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jh.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wb.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kx.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zf.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dm.shtwfgs.cn

[J09] 时区处理
来源：http://ir.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nz.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vu.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ry.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rn.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rc.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fz.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ju.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wz.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://xs.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ty.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pr.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ot.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ob.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vz.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vt.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ee.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rg.yuntaijiaju.cn


<!-- 参考信息 -->