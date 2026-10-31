代发 wailian999

H. 异常与错误处理
来源：http://ca.bookmarksfly.cn

================================================================================
来源：http://ij.lnxyls.cn

[H01] try / catch 基础
来源：http://bd.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://no.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kl.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ml.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ek.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qy.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ur.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qp.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xy.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://jp.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rf.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bm.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ww.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zv.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oh.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xt.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wr.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hm.panjiajie.cn

[H03] 主动抛出异常
来源：http://vw.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://oo.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://og.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://fs.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://rx.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://em.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ax.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://my.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ql.shxzukj.cn

[H04] 自定义异常类型
来源：http://nt.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://ru.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hn.hahajie.cn

JS:   class MyError extends Error {}
来源：http://jx.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://uu.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://aa.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wq.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ge.huanxung.cn

C#:   class MyException : Exception {}
来源：http://nx.asd995.cn

[H05] 捕获特定类型
来源：http://ji.521024.cn

Py:   except ValueError as e:
来源：http://sf.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://on.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://yc.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://wx.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://gt.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bv.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://qd.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://me.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://pq.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://dp.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pl.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mz.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fp.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sl.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://et.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://yg.521024.cn

C#:   obj?.A?.B ?? default
来源：http://cu.hnjuh.cn

[H07] 断言
来源：http://hd.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://gp.szsharing.cn

PHP:  assert($x > 0);
来源：http://it.szsharing.cn

JS:   console.assert(x > 0);
来源：http://va.521024.cn

TS:   console.assert(x > 0);
来源：http://us.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://xl.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hp.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://md.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://ec.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://fp.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://xj.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nh.shxzukj.cn

JS:   e.message;  e.stack
来源：http://yn.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dw.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oa.asd995.cn

Go:   err.Error()
来源：http://tt.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://rw.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://qj.gzmigu.cn

[H09] 带错误码的异常
来源：http://tn.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ix.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ie.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rh.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rn.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ov.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cd.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bn.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ct.panjiajie.cn

[H10] 资源自动释放
来源：http://xp.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qe.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ep.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jo.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wi.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wc.huanxung.cn

Go:   defer f.Close()
来源：http://vq.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cs.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ou.asd995.cn

================================================================================
来源：http://ov.nicolike.cn

I. 正则表达式
来源：http://ng.hnjuh.cn

================================================================================
来源：http://mq.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://tn.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zh.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://au.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://wj.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://bx.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://to.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mf.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://ej.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rs.asd995.cn

[I02] 提取所有匹配
来源：http://ut.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://na.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rs.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ie.521024.cn

TS:   s.match(/\d+/g)
来源：http://qk.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jm.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tr.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://hd.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eh.newstarts.cn

[I03] 提取捕获分组
来源：http://ap.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xj.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fq.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ha.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gz.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nj.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mj.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://il.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qi.hnjuh.cn

[I04] 正则替换
来源：http://cy.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pt.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tf.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lh.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sz.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ci.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://de.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fq.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vq.gzmigu.cn

[I05] 按正则拆分
来源：http://iq.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oe.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kd.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://ch.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://qy.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://li.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jk.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vh.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pr.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sr.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jc.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://or.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gp.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lb.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ek.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qk.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lq.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://dk.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ub.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sy.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://im.jctech888.com.cn

TS:   /error/gim
来源：http://pa.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xi.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nd.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://zk.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zs.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://ue.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dq.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ct.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://us.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lr.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gn.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://we.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ao.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ix.bookmarksfly.cn

================================================================================
来源：http://gc.nicolike.cn

J. 日期与时间
来源：http://ly.huixinmuqiang.cn

================================================================================
来源：http://ak.bookmarksfly.cn

[J01] 获取当前时间
来源：http://do.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yy.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kh.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://pi.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://xg.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://by.bjjhwx.cn

Go:   time.Now()
来源：http://ux.9csxet.cn

Ruby: Time.now
来源：http://vq.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sx.yuntaijiaju.cn

[J02] 格式化输出
来源：http://ol.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bm.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wy.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mw.chemitech.net.cn

TS:   d.toISOString()
来源：http://xk.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vt.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hs.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kk.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pc.gzmigu.cn

[J03] 字符串解析为日期
来源：http://ep.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qy.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kv.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://po.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ps.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tr.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mu.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://qo.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lh.nicolike.cn

[J04] 时间戳与日期互转
来源：http://db.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ad.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vl.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xc.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://as.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uw.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kq.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uk.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://er.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://nh.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://gi.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qi.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zj.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pm.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://hq.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fm.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ox.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ov.huanxung.cn

[J06] 计算两时间之差
来源：http://zi.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://ut.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://lj.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://km.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ya.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rt.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://hc.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://vf.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://tm.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://ag.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://jf.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://st.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xe.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hq.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gk.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hb.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wb.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://vr.hahajie.cn

[J08] 提取年月日与星期
来源：http://gl.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ov.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ep.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hi.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yf.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jy.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lg.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pi.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://um.colortex.cn

[J09] 时区处理
来源：http://yv.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jp.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mi.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qm.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jn.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tu.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vs.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qy.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eu.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://yp.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qw.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ud.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ap.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ah.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fp.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ky.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://up.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jh.huixiangedu.cn

================================================================================
来源：http://xh.nszjky.cn

K. JSON 与序列化
来源：http://sw.lnxyls.cn

================================================================================
来源：http://aq.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://vk.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nf.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vk.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://xn.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://vg.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jw.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://sx.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ml.hahajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jp.521024.cn

[K02] JSON 字符串转对象
来源：http://hw.huanxung.cn

Py:   json.loads(s)
来源：http://cp.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nk.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://ny.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://ts.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ar.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://un.lnxyls.cn

Ruby: JSON.parse(s)
来源：http://ps.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xq.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://ii.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vu.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oq.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gg.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fu.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rh.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hl.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ui.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://re.nszjky.cn

[K04] 读取 JSON 文件
来源：http://df.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fi.chemitech.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gv.newstarts.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ml.hahajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ez.panjiajie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://db.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qt.lnxyls.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uh.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://io.9csxet.cn

[K05] 深拷贝对象
来源：http://pw.yuexingan06.cn


<!-- 参考信息 -->