代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zl.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cp.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://gh.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bk.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://nr.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vr.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://mg.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uh.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://ko.asd995.cn

JS:   Object.entries(obj)
来源：http://ph.shxzukj.cn

TS:   Object.entries(obj)
来源：http://xj.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iq.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xf.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://dj.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://nl.newstarts.cn

================================================================================
来源：http://xq.521024.cn

H. 异常与错误处理
来源：http://zt.bjjhwx.cn

================================================================================
来源：http://dr.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://qn.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ay.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ps.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gk.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ly.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hw.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zg.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rq.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cl.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://lp.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cv.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cn.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oy.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yr.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pr.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://to.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cy.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nr.shxzukj.cn

[H03] 主动抛出异常
来源：http://ej.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://uh.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nm.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://cv.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://kg.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pg.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://by.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ii.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jj.gzmigu.cn

[H04] 自定义异常类型
来源：http://ko.asd995.cn

Py:   class MyError(Exception): pass
来源：http://hw.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qr.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://lh.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://ns.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://ei.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kb.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://ow.colortex.cn

C#:   class MyException : Exception {}
来源：http://hq.chemitech.net.cn

[H05] 捕获特定类型
来源：http://qd.shxzskj.cn

Py:   except ValueError as e:
来源：http://eo.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ya.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://os.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://gp.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://eo.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gv.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://ud.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wg.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://zp.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://xk.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nl.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gw.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xm.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ao.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kg.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ev.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://wa.panjiajie.cn

[H07] 断言
来源：http://ou.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://rp.szsharing.cn

PHP:  assert($x > 0);
来源：http://wd.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://gs.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://ri.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://ri.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fx.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://br.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://dh.521024.cn

[H08] 获取错误信息与堆栈
来源：http://as.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://go.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dq.9csxet.cn

JS:   e.message;  e.stack
来源：http://zm.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wc.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nt.hnjuh.cn

Go:   err.Error()
来源：http://gi.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://dp.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://uh.shxzukj.cn

[H09] 带错误码的异常
来源：http://al.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://av.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hc.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pb.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vl.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ah.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yc.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xs.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gy.shxzukj.cn

[H10] 资源自动释放
来源：http://uj.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cd.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zu.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gt.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yb.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hn.lnxyls.cn

Go:   defer f.Close()
来源：http://ws.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vi.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ut.521024.cn

================================================================================
来源：http://vx.szsharing.cn

I. 正则表达式
来源：http://st.yuntaijiaju.cn

================================================================================
来源：http://zc.chemitech.net.cn

[I01] 判断是否匹配
来源：http://gw.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fo.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jx.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://oy.asd995.cn

TS:   /\d+/.test(s)
来源：http://ti.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jh.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mo.521024.cn

Ruby: s.match?(/\d+/)
来源：http://bu.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fu.huanxung.cn

[I02] 提取所有匹配
来源：http://je.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://cp.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xy.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qe.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://xp.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tg.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://po.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://rs.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ac.bjjhwx.cn

[I03] 提取捕获分组
来源：http://ix.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ez.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pc.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gy.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nr.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ne.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://up.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bh.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rr.bjjhwx.cn

[I04] 正则替换
来源：http://ne.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qw.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vw.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dy.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kh.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dv.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ob.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wz.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vp.bookmarksfly.cn

[I05] 按正则拆分
来源：http://ed.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iv.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://un.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://af.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://cl.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://hn.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xt.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ym.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lt.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ao.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zs.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nk.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dn.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ip.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zr.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nb.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tm.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dn.521024.cn

[I07] 忽略大小写与多行模式
来源：http://ar.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mn.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nv.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uq.lnxyls.cn

TS:   /error/gim
来源：http://om.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pb.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fd.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://en.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vw.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ff.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pk.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hp.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cr.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sg.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fn.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nm.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yy.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gc.nicolike.cn

================================================================================
来源：http://im.jianghongdianzi.cn

J. 日期与时间
来源：http://xa.hnjuh.cn

================================================================================
来源：http://ea.newstarts.cn

[J01] 获取当前时间
来源：http://dv.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ej.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cm.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://rl.huanxung.cn

TS:   new Date();  Date.now()
来源：http://av.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sg.hahajie.cn

Go:   time.Now()
来源：http://au.chemitech.net.cn

Ruby: Time.now
来源：http://wu.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cx.szsharing.cn

[J02] 格式化输出
来源：http://eb.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vf.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cl.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ij.hahajie.cn

TS:   d.toISOString()
来源：http://je.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://os.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zo.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cq.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jb.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://tm.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ee.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nf.521024.cn

JS:   new Date("2024-01-02")
来源：http://bq.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://nr.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vq.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yu.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://xx.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zt.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://yq.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pl.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://id.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bn.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yt.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uo.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jg.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ek.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ku.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ns.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://az.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xv.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xz.asd995.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://av.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://mo.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://os.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://mw.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cm.muxihuayi.cn

[J06] 计算两时间之差
来源：http://wh.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://lj.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://uj.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ly.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ry.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lc.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://ao.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ah.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://ba.hnjuh.cn

[J07] 比较两个日期
来源：http://ot.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://kc.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://at.hahajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lv.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dg.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ec.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zo.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://we.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://wm.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://ru.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kp.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eg.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gb.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ta.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qf.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wb.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://us.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wr.lnxyls.cn

[J09] 时区处理
来源：http://mc.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ol.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hs.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xc.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://la.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mp.colortex.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://td.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://to.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yp.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://cj.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rr.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xm.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zn.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bu.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qt.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://af.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iy.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://je.huixinmuqiang.cn

================================================================================
来源：http://au.szxytkj.cn

K. JSON 与序列化
来源：http://pq.521024.cn

================================================================================
来源：http://st.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://dy.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hu.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://np.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://zv.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://yc.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bc.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://cc.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zf.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xi.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://si.huixiangedu.cn

Py:   json.loads(s)
来源：http://nu.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://li.hahajie.cn

JS:   JSON.parse(s)
来源：http://ja.szsharing.cn

TS:   JSON.parse(s)
来源：http://ke.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yh.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://ua.9csxet.cn

Ruby: JSON.parse(s)
来源：http://yp.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lr.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://tw.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sj.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ms.shxzukj.cn


<!-- 参考信息 -->