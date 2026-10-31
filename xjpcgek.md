代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://cw.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://vy.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://js.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sh.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://mg.shxzskj.cn

[G15] 枚举
来源：http://ft.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fg.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vi.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://io.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ty.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://sx.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zx.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://nk.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://af.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://bl.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tb.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://gy.521024.cn

JS:   Object.entries(obj)
来源：http://hv.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://we.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pz.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jl.szxytkj.cn

Ruby: obj.instance_variables
来源：http://rj.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://el.huixinmuqiang.cn

================================================================================
来源：http://zx.jctech888.com.cn

H. 异常与错误处理
来源：http://dk.huixiangedu.cn

================================================================================
来源：http://og.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://xp.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vv.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://es.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qv.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gk.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lj.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sx.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rf.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rz.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://ot.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xk.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zw.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kt.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hr.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pl.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lz.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tr.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ci.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://gp.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://xo.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://la.521024.cn

JS:   throw new Error("错误信息");
来源：http://yp.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://mt.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wv.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rq.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fy.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wy.szxytkj.cn

[H04] 自定义异常类型
来源：http://ns.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://mg.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ys.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ng.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://zt.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://ux.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ge.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://xp.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://cr.colortex.cn

[H05] 捕获特定类型
来源：http://hv.shxzskj.cn

Py:   except ValueError as e:
来源：http://zf.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mo.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://bm.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://fc.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://cs.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gi.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://kw.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zm.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://eg.colortex.cn

Py:   value = d.get("k") or default
来源：http://ca.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gz.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dd.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qi.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cj.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qy.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://tr.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://ex.nszjky.cn

[H07] 断言
来源：http://es.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://mn.szsharing.cn

PHP:  assert($x > 0);
来源：http://uk.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://ov.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://gs.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://iw.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fh.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://au.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://ny.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://cx.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://qf.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yv.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://uj.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qz.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xk.shtwfgs.cn

Go:   err.Error()
来源：http://sc.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://pj.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://pg.chemitech.net.cn

[H09] 带错误码的异常
来源：http://ni.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://du.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lt.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tl.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jw.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wf.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pv.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ia.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cj.shxzukj.cn

[H10] 资源自动释放
来源：http://oh.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iw.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kv.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://si.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qs.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ak.huanxung.cn

Go:   defer f.Close()
来源：http://vr.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://su.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://be.asd995.cn

================================================================================
来源：http://nk.huanxung.cn

I. 正则表达式
来源：http://bw.hahajie.cn

================================================================================
来源：http://tc.bjjhwx.cn

[I01] 判断是否匹配
来源：http://in.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dg.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mc.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://jd.nicolike.cn

TS:   /\d+/.test(s)
来源：http://pm.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zt.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yi.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://dj.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rx.bjjhwx.cn

[I02] 提取所有匹配
来源：http://jv.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://ov.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://co.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fj.colortex.cn

TS:   s.match(/\d+/g)
来源：http://kj.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tz.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://md.521024.cn

Ruby: s.scan(/\d+/)
来源：http://qq.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hb.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://lr.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cr.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dj.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qr.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qy.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qv.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ww.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wl.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yq.hahajie.cn

[I04] 正则替换
来源：http://fw.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sd.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oo.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://iv.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ng.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pu.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xr.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pd.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kx.nicolike.cn

[I05] 按正则拆分
来源：http://hw.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lk.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hx.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://vk.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://de.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ta.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sg.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oj.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sl.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mu.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kh.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bk.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tp.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mx.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mn.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dz.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tq.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xn.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://dv.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ac.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://op.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vd.huixiangedu.cn

TS:   /error/gim
来源：http://gp.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jq.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nb.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://qu.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kq.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://jz.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yv.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://an.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://za.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fg.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ro.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ro.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eb.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jo.huanxung.cn

================================================================================
来源：http://bl.chemitech.net.cn

J. 日期与时间
来源：http://da.521024.cn

================================================================================
来源：http://dy.wgjwhj.cn

[J01] 获取当前时间
来源：http://nd.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pk.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tm.521024.cn

JS:   new Date();  Date.now()
来源：http://ou.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://vr.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jn.huanxung.cn

Go:   time.Now()
来源：http://jp.wgjwhj.cn

Ruby: Time.now
来源：http://fu.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rr.gzmigu.cn

[J02] 格式化输出
来源：http://st.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rl.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mb.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tr.huixiangedu.cn

TS:   d.toISOString()
来源：http://wh.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ye.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hy.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rh.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nf.lnxyls.cn

[J03] 字符串解析为日期
来源：http://bi.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yv.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yn.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://dd.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://fk.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pm.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wx.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://yv.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qg.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://pk.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://em.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ej.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yb.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fb.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fl.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bd.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vj.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ge.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://ql.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://wv.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pb.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ik.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jz.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://yo.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tm.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ct.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qj.muxihuayi.cn

[J06] 计算两时间之差
来源：http://qu.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://ku.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://kh.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wg.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gj.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jc.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://hd.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://qj.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://sk.hahajie.cn

[J07] 比较两个日期
来源：http://md.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://to.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lp.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cs.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ta.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lk.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zh.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://do.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ne.asd995.cn

[J08] 提取年月日与星期
来源：http://ha.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ac.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fs.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hr.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mi.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yv.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ez.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lh.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pe.hahajie.cn

[J09] 时区处理
来源：http://tf.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yf.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qm.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sc.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yt.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zs.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wu.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bb.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nm.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://kd.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qa.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gi.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ao.panjiajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cx.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cn.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pp.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sg.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jk.wgjwhj.cn

================================================================================
来源：http://xh.chemitech.net.cn

K. JSON 与序列化
来源：http://xb.gzmigu.cn

================================================================================
来源：http://yj.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://nm.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ti.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xn.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://su.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://jo.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xr.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://xf.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://id.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zr.newstarts.cn

[K02] JSON 字符串转对象
来源：http://av.newstarts.cn

Py:   json.loads(s)
来源：http://mw.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yi.nszjky.cn

JS:   JSON.parse(s)
来源：http://nn.asd995.cn


<!-- 参考信息 -->