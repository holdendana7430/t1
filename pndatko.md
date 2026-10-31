代发 wailian999

C#:   record User(string Name, int Age);
来源：http://uz.nicolike.cn

[G15] 枚举
来源：http://qo.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zv.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ti.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bq.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cx.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://ze.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hv.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://fa.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ix.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://mu.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rv.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://br.nszjky.cn

JS:   Object.entries(obj)
来源：http://bo.gzmigu.cn

TS:   Object.entries(obj)
来源：http://yr.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ju.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hs.shxzskj.cn

Ruby: obj.instance_variables
来源：http://xa.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://yq.szxytkj.cn

================================================================================
来源：http://hx.panjiajie.cn

H. 异常与错误处理
来源：http://xt.newstarts.cn

================================================================================
来源：http://uq.haigaiapp.cn

[H01] try / catch 基础
来源：http://qq.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ua.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://em.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://al.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://so.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ri.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lp.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pk.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ax.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ex.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xz.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lb.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gu.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iw.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yy.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hn.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rn.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mt.chemitech.net.cn

[H03] 主动抛出异常
来源：http://lp.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://mp.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lr.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://wm.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://wz.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mp.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://se.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mu.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://px.szsharing.cn

[H04] 自定义异常类型
来源：http://gg.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://zv.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mq.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://ni.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://xu.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://ou.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ye.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://bd.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://hg.gzmigu.cn

[H05] 捕获特定类型
来源：http://ia.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://di.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ps.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://jm.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://gs.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://mt.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ut.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://ry.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zf.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://kb.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://qe.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vr.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ip.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nr.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cv.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cj.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://ne.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://ls.shxzukj.cn

[H07] 断言
来源：http://eb.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://us.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://ii.nicolike.cn

JS:   console.assert(x > 0);
来源：http://ej.asd995.cn

TS:   console.assert(x > 0);
来源：http://rk.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://kh.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tb.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oj.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://wc.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ow.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ds.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rs.panjiajie.cn

JS:   e.message;  e.stack
来源：http://le.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gw.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nd.newstarts.cn

Go:   err.Error()
来源：http://ea.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://go.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://fc.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://ic.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xc.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ey.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qd.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sh.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bg.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cz.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qx.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ro.huanxung.cn

[H10] 资源自动释放
来源：http://pg.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yo.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ez.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sj.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kt.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ew.shtwfgs.cn

Go:   defer f.Close()
来源：http://ka.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wi.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ff.wgjwhj.cn

================================================================================
来源：http://lx.bjjhwx.cn

I. 正则表达式
来源：http://dq.asd995.cn

================================================================================
来源：http://mz.lnxyls.cn

[I01] 判断是否匹配
来源：http://fg.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cc.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gz.9csxet.cn

JS:   /\d+/.test(s)
来源：http://mo.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://wd.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pj.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wk.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://kr.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://su.gzmigu.cn

[I02] 提取所有匹配
来源：http://ax.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://jc.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uu.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ro.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://lk.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yp.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hf.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://zd.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tl.szxytkj.cn

[I03] 提取捕获分组
来源：http://mv.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sb.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dl.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xc.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ab.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ww.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hm.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ix.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gr.bookmarksfly.cn

[I04] 正则替换
来源：http://tb.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mz.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xp.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fy.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://th.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gb.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hs.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zd.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rt.haigaiapp.cn

[I05] 按正则拆分
来源：http://kl.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fi.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zj.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://qo.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://sy.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://hh.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ag.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ye.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ce.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eo.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kn.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gc.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ez.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ou.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cp.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ze.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fl.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sw.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://rt.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mu.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cq.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://id.szsharing.cn

TS:   /error/gim
来源：http://nw.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://te.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ih.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://ik.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pb.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://rj.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zv.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cs.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ln.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bt.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yb.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hr.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gg.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ay.chemitech.net.cn

================================================================================
来源：http://ty.yuexingan06.cn

J. 日期与时间
来源：http://gn.newstarts.cn

================================================================================
来源：http://yg.shxzskj.cn

[J01] 获取当前时间
来源：http://qf.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vj.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mv.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://wr.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://rv.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ub.haigaiapp.cn

Go:   time.Now()
来源：http://ek.shxzskj.cn

Ruby: Time.now
来源：http://kw.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pz.bookmarksfly.cn

[J02] 格式化输出
来源：http://dv.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gs.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bn.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lv.lnxyls.cn

TS:   d.toISOString()
来源：http://wy.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wy.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gq.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wx.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vw.521024.cn

[J03] 字符串解析为日期
来源：http://eg.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://um.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lq.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ui.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://yi.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xo.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ob.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://iy.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dz.huanxung.cn

[J04] 时间戳与日期互转
来源：http://bu.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zl.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ay.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kj.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vd.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hh.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://il.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hd.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jw.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://av.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://tl.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ej.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rf.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://df.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://as.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iq.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://ty.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gl.521024.cn

[J06] 计算两时间之差
来源：http://bq.asd995.cn

Py:   (end - start).total_seconds()
来源：http://qe.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://mt.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://et.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://og.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://br.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://xt.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://cw.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://em.shtwfgs.cn

[J07] 比较两个日期
来源：http://vp.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://jk.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gr.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vy.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fd.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zu.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hl.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wc.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://oo.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://op.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bj.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eq.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rb.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gg.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qe.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yt.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ag.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zz.9csxet.cn

[J09] 时区处理
来源：http://qp.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bj.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oe.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sl.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wr.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vc.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jv.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sa.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bt.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://vj.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bf.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sk.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ss.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ig.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zc.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zz.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ev.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fo.szsharing.cn

================================================================================
来源：http://ni.chemitech.net.cn

K. JSON 与序列化
来源：http://rt.bjjhwx.cn

================================================================================
来源：http://mm.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ms.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mr.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ew.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://jg.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ol.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ok.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://nh.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uz.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://di.huanxung.cn

[K02] JSON 字符串转对象
来源：http://xt.hnjuh.cn

Py:   json.loads(s)
来源：http://ty.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zf.wgjwhj.cn

JS:   JSON.parse(s)
来源：http://ue.panjiajie.cn

TS:   JSON.parse(s)
来源：http://kg.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fj.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://ca.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://wi.chemitech.net.cn


<!-- 参考信息 -->