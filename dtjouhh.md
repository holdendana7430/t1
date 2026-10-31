代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ab.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kv.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mh.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vf.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://le.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://av.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://la.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://pj.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gu.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uu.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mn.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gi.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tp.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yo.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gw.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hk.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://kk.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://le.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eg.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://hw.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://bg.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pn.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yg.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vo.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vy.nicolike.cn

[H04] 自定义异常类型
来源：http://vk.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://km.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iy.521024.cn

JS:   class MyError extends Error {}
来源：http://og.huanxung.cn

TS:   class MyError extends Error {}
来源：http://mh.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://zq.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mq.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://ml.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://zi.521024.cn

[H05] 捕获特定类型
来源：http://ut.nicolike.cn

Py:   except ValueError as e:
来源：http://xq.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://te.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://gx.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ok.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://dg.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lk.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://ac.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xw.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://yn.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://in.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tl.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ne.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://es.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bo.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cx.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://xh.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://ue.lnxyls.cn

[H07] 断言
来源：http://wn.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://zs.nszjky.cn

PHP:  assert($x > 0);
来源：http://bf.hahajie.cn

JS:   console.assert(x > 0);
来源：http://kr.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ii.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://bt.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://am.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cr.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://gi.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ft.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://rl.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jx.huanxung.cn

JS:   e.message;  e.stack
来源：http://ry.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hr.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ly.asd995.cn

Go:   err.Error()
来源：http://ef.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ln.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://kd.asd995.cn

[H09] 带错误码的异常
来源：http://px.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yn.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xl.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wp.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://er.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vy.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ge.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pe.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qw.szsharing.cn

[H10] 资源自动释放
来源：http://wz.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pr.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xe.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ru.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jo.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rm.colortex.cn

Go:   defer f.Close()
来源：http://gt.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gi.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tz.muxihuayi.cn

================================================================================
来源：http://bc.jctech888.com.cn

I. 正则表达式
来源：http://mu.chemitech.net.cn

================================================================================
来源：http://vp.huanxung.cn

[I01] 判断是否匹配
来源：http://vz.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://st.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vf.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://ox.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://cm.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://il.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kl.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://fx.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dd.jctech888.com.cn

[I02] 提取所有匹配
来源：http://et.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://tm.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://je.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ki.asd995.cn

TS:   s.match(/\d+/g)
来源：http://pe.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rc.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hx.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://ct.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sj.huixiangedu.cn

[I03] 提取捕获分组
来源：http://mm.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vf.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ne.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vf.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iy.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nn.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://am.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jt.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ol.521024.cn

[I04] 正则替换
来源：http://xf.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dc.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eq.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ca.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ii.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vl.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ex.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://in.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fp.hnjuh.cn

[I05] 按正则拆分
来源：http://bd.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dw.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uc.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://to.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://uh.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://qs.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dh.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nt.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rm.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zi.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tu.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://je.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://je.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zn.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jk.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ce.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bf.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rh.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://yv.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wp.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zr.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sg.panjiajie.cn

TS:   /error/gim
来源：http://wh.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pl.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nd.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://er.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ez.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://vq.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xe.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uz.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ap.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://of.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dk.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://of.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yk.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://il.shxzukj.cn

================================================================================
来源：http://ge.asd995.cn

J. 日期与时间
来源：http://gq.panjiajie.cn

================================================================================
来源：http://yy.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://zr.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://py.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ic.9csxet.cn

JS:   new Date();  Date.now()
来源：http://tb.colortex.cn

TS:   new Date();  Date.now()
来源：http://zf.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tn.szxytkj.cn

Go:   time.Now()
来源：http://cq.hahajie.cn

Ruby: Time.now
来源：http://qv.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dq.bjjhwx.cn

[J02] 格式化输出
来源：http://gg.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tv.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gi.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fi.gzmigu.cn

TS:   d.toISOString()
来源：http://zj.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://se.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qv.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ru.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://va.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://ix.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ha.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ij.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://va.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://tl.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ch.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hm.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://nh.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nx.colortex.cn

[J04] 时间戳与日期互转
来源：http://cw.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nq.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qu.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mh.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fy.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ax.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sk.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lq.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qf.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://jw.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://fb.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aa.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qn.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lr.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://rs.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://if.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://jv.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ys.shxzskj.cn

[J06] 计算两时间之差
来源：http://vj.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://oe.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://lq.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bg.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://be.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jy.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://et.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://xl.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://qw.hnjuh.cn

[J07] 比较两个日期
来源：http://zp.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://ck.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vf.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tv.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lt.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ng.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ch.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ig.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://kq.nicolike.cn

[J08] 提取年月日与星期
来源：http://om.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bq.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wt.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yq.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rp.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ef.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ov.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pj.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hv.lnxyls.cn

[J09] 时区处理
来源：http://et.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qs.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ow.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vt.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zx.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aj.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vc.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qm.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ko.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://qd.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yy.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rn.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pt.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ak.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lw.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yc.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sf.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sp.jctech888.com.cn

================================================================================
来源：http://ig.jianghongdianzi.cn

K. JSON 与序列化
来源：http://be.hnjuh.cn

================================================================================
来源：http://vk.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://wd.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fj.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vq.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://yo.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://wt.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://im.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://nd.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ny.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oc.panjiajie.cn

[K02] JSON 字符串转对象
来源：http://ni.hahajie.cn

Py:   json.loads(s)
来源：http://tf.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yl.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://fg.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://za.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ec.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://rs.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://ut.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jl.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://ew.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://py.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lc.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yo.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kb.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yu.huixinmuqiang.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vg.colortex.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sf.panjiajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tn.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://jf.gzmigu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rs.gzmigu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bv.bookmarksfly.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lo.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vm.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pf.huanxung.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jd.huanxung.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qs.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ww.panjiajie.cn

[K05] 深拷贝对象
来源：http://wq.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://yl.huixiangedu.cn

PHP:  unserialize(serialize($obj));
来源：http://ly.9csxet.cn

JS:   structuredClone(obj)
来源：http://lc.nicolike.cn

TS:   structuredClone(obj)
来源：http://wv.yuntaijiaju.cn


<!-- 参考信息 -->