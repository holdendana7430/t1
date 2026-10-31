代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://np.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sa.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vs.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vy.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ex.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pk.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://km.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://ke.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://us.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ri.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vi.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vs.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dp.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fl.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oz.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rq.szsharing.cn

[H03] 主动抛出异常
来源：http://hv.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://rm.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xa.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://xv.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://zy.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fn.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tw.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ma.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vn.colortex.cn

[H04] 自定义异常类型
来源：http://zo.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://kk.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aw.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://ry.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://hp.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://wl.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sn.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://ew.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://iw.colortex.cn

[H05] 捕获特定类型
来源：http://ry.muxihuayi.cn

Py:   except ValueError as e:
来源：http://bb.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jx.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://pv.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://ij.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://xh.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aq.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://bj.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tl.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://eg.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://yt.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rj.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ag.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yz.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rs.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oy.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://wy.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://bh.newstarts.cn

[H07] 断言
来源：http://ut.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://xc.panjiajie.cn

PHP:  assert($x > 0);
来源：http://td.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://ke.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://ql.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://xg.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qe.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hy.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://de.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://rj.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://px.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qw.huanxung.cn

JS:   e.message;  e.stack
来源：http://bs.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hc.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wo.asd995.cn

Go:   err.Error()
来源：http://cm.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://dc.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://cb.muxihuayi.cn

[H09] 带错误码的异常
来源：http://lh.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uh.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://le.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://af.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eh.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fw.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ej.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yj.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fw.lnxyls.cn

[H10] 资源自动释放
来源：http://yq.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zd.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://in.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://np.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zk.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fj.muxihuayi.cn

Go:   defer f.Close()
来源：http://qm.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cs.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zj.shtwfgs.cn

================================================================================
来源：http://qi.chemitech.net.cn

I. 正则表达式
来源：http://mj.hnjuh.cn

================================================================================
来源：http://oh.bjjhwx.cn

[I01] 判断是否匹配
来源：http://tv.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ty.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://li.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://dn.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://jo.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tj.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hd.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://jd.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rk.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://js.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://mp.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xc.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tg.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://tn.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vt.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vn.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://rp.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ax.hahajie.cn

[I03] 提取捕获分组
来源：http://rc.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rc.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://za.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gg.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gr.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mq.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zj.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ry.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xv.panjiajie.cn

[I04] 正则替换
来源：http://jb.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rv.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ad.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jb.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gn.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lt.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aj.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cj.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gc.jctech888.com.cn

[I05] 按正则拆分
来源：http://px.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cf.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ie.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://cn.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://as.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://iv.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wz.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wz.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rm.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wr.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xs.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bb.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gk.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tz.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tx.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ks.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fj.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pp.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ci.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nz.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cy.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kn.hahajie.cn

TS:   /error/gim
来源：http://np.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pz.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kk.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://gy.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hq.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://td.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lo.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qv.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ug.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dy.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qv.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cb.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tp.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xg.wgjwhj.cn

================================================================================
来源：http://kj.huixinmuqiang.cn

J. 日期与时间
来源：http://zc.nszjky.cn

================================================================================
来源：http://oe.newstarts.cn

[J01] 获取当前时间
来源：http://mx.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zg.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xg.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://rf.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://cj.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jj.nszjky.cn

Go:   time.Now()
来源：http://tk.yuexingan06.cn

Ruby: Time.now
来源：http://ss.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rc.hnjuh.cn

[J02] 格式化输出
来源：http://eg.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ld.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xa.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bk.wgjwhj.cn

TS:   d.toISOString()
来源：http://fd.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zi.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ds.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nn.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pj.521024.cn

[J03] 字符串解析为日期
来源：http://th.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yg.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ah.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://jw.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://uq.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xj.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mf.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://oe.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vl.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://oi.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kr.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sc.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ye.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hq.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eq.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zw.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xp.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kt.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://gs.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://yw.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mo.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hm.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wb.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://cr.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lz.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://np.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yl.gzmigu.cn

[J06] 计算两时间之差
来源：http://yj.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://qg.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://lx.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://te.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qw.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bq.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://nm.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://ft.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://ew.wgjwhj.cn

[J07] 比较两个日期
来源：http://ck.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://tt.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dy.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tb.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hx.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mh.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://da.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://br.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://uz.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://iy.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bn.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tc.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nv.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qd.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ri.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ud.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rx.haigaiapp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://at.wgjwhj.cn

[J09] 时区处理
来源：http://ck.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jt.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cq.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ta.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ci.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xk.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sz.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ae.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://of.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://dm.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ow.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wf.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ts.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kn.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qn.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pe.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bx.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yr.shxzukj.cn

================================================================================
来源：http://uo.jianghongdianzi.cn

K. JSON 与序列化
来源：http://dk.muxihuayi.cn

================================================================================
来源：http://jg.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://rj.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tl.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hp.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://ag.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://nr.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ik.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://hl.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xu.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vg.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://rz.panjiajie.cn

Py:   json.loads(s)
来源：http://uq.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jc.szsharing.cn

JS:   JSON.parse(s)
来源：http://iy.shxzukj.cn

TS:   JSON.parse(s)
来源：http://kb.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xz.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://ur.asd995.cn

Ruby: JSON.parse(s)
来源：http://zj.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ib.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://pp.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uq.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qg.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pd.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cn.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wi.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mh.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lv.hnjuh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ly.yuexingan06.cn

[K04] 读取 JSON 文件
来源：http://nh.bjjhwx.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ay.lnxyls.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ch.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ju.lnxyls.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://np.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oq.shxzskj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jr.panjiajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jh.asd995.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hd.shtwfgs.cn

[K05] 深拷贝对象
来源：http://fv.shxzskj.cn

Py:   copy.deepcopy(obj)
来源：http://ic.szsharing.cn

PHP:  unserialize(serialize($obj));
来源：http://er.asd995.cn

JS:   structuredClone(obj)
来源：http://ri.haigaiapp.cn

TS:   structuredClone(obj)
来源：http://de.lnxyls.cn


<!-- 参考信息 -->