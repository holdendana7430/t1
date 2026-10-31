代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jg.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jm.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yc.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ac.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://is.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zr.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pd.newstarts.cn

[H02] finally / ensure 收尾
来源：http://ef.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sr.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://be.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ej.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cz.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ch.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rt.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://em.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://am.9csxet.cn

[H03] 主动抛出异常
来源：http://cn.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://go.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ua.colortex.cn

JS:   throw new Error("错误信息");
来源：http://tc.asd995.cn

TS:   throw new Error("错误信息");
来源：http://hh.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hd.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yr.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yd.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zc.huanxung.cn

[H04] 自定义异常类型
来源：http://ac.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://tl.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bh.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://uz.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://wp.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://fu.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xq.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://xu.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://oc.colortex.cn

[H05] 捕获特定类型
来源：http://jf.gzmigu.cn

Py:   except ValueError as e:
来源：http://hy.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gv.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://sf.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://tk.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://om.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ip.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://pu.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xk.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://ku.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://bn.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rt.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lr.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://et.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xw.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nj.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://fd.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://sy.huixiangedu.cn

[H07] 断言
来源：http://sp.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://wd.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://lh.nicolike.cn

JS:   console.assert(x > 0);
来源：http://pd.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://cx.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://lc.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wl.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hm.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://pk.521024.cn

[H08] 获取错误信息与堆栈
来源：http://zd.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://sn.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pu.521024.cn

JS:   e.message;  e.stack
来源：http://sd.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ak.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mn.wgjwhj.cn

Go:   err.Error()
来源：http://ag.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://lk.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://sn.521024.cn

[H09] 带错误码的异常
来源：http://hq.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tb.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xv.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kk.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mg.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zu.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nh.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wt.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uq.nszjky.cn

[H10] 资源自动释放
来源：http://iy.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qz.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zk.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dj.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ni.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kc.hnjuh.cn

Go:   defer f.Close()
来源：http://rd.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kt.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gm.muxihuayi.cn

================================================================================
来源：http://gu.szxytkj.cn

I. 正则表达式
来源：http://zp.huixinmuqiang.cn

================================================================================
来源：http://qe.shxzukj.cn

[I01] 判断是否匹配
来源：http://mv.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ox.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vb.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://af.szsharing.cn

TS:   /\d+/.test(s)
来源：http://sm.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ww.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ua.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://jy.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://on.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://sx.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://kt.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wq.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ft.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://yj.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ms.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dg.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://il.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gn.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://vl.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tq.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ok.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://el.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kn.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://if.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zs.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kh.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ix.521024.cn

[I04] 正则替换
来源：http://xu.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xn.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wf.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cw.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rn.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://co.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ar.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tq.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ho.szsharing.cn

[I05] 按正则拆分
来源：http://oy.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tn.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qx.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://hc.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://iz.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://wo.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://si.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ee.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rf.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pb.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cu.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fk.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ky.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jz.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nu.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nl.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vv.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ya.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://et.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bw.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hs.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bh.shxzskj.cn

TS:   /error/gim
来源：http://tg.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qr.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://on.asd995.cn

Ruby: s.scan(/error/i)
来源：http://cf.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kl.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://xf.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vl.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mn.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://so.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kp.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qk.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://er.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hf.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wq.hnjuh.cn

================================================================================
来源：http://pg.gzmigu.cn

J. 日期与时间
来源：http://ag.bjjhwx.cn

================================================================================
来源：http://iw.haigaiapp.cn

[J01] 获取当前时间
来源：http://tu.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vh.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://md.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://qz.nicolike.cn

TS:   new Date();  Date.now()
来源：http://ij.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yt.nszjky.cn

Go:   time.Now()
来源：http://zo.jianghongdianzi.cn

Ruby: Time.now
来源：http://aj.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://st.shxzukj.cn

[J02] 格式化输出
来源：http://bd.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ju.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cx.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ud.huanxung.cn

TS:   d.toISOString()
来源：http://pz.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zr.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://br.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sy.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cg.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://nw.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zk.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qf.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ho.asd995.cn

TS:   new Date("2024-01-02")
来源：http://jy.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kk.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jk.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://sx.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oe.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://wj.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dy.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bc.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rd.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bk.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vw.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mw.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ly.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bj.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://ua.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://xm.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zw.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gv.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ll.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://fb.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vr.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://ub.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jq.9csxet.cn

[J06] 计算两时间之差
来源：http://lc.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://hs.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://cz.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dm.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pj.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bv.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://hd.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://ob.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ql.shxzukj.cn

[J07] 比较两个日期
来源：http://os.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://xr.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yi.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wv.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vq.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bv.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cu.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gw.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://uu.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://ng.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ra.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pa.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fd.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://db.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hf.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://av.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qv.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gj.yuntaijiaju.cn

[J09] 时区处理
来源：http://qv.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kj.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://md.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://am.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cr.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hj.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cv.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cu.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bz.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://nj.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xm.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pk.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yb.9csxet.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://py.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qd.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dr.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fh.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xr.bookmarksfly.cn

================================================================================
来源：http://op.huixiangedu.cn

K. JSON 与序列化
来源：http://tl.hnjuh.cn

================================================================================
来源：http://ch.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://hm.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hw.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://su.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://no.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://lj.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gy.9csxet.cn

Go:   json.Marshal(obj)
来源：http://ai.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cx.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://se.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://yc.muxihuayi.cn

Py:   json.loads(s)
来源：http://xt.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fo.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://dx.bookmarksfly.cn

TS:   JSON.parse(s)
来源：http://se.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ct.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://rx.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://sq.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ew.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://fa.newstarts.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aj.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://it.521024.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ii.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gt.szsharing.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zu.newstarts.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vw.jianghongdianzi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xl.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ft.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://nr.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lt.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ul.colortex.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ql.asd995.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nq.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://na.hnjuh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wb.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ln.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gq.jianghongdianzi.cn

[K05] 深拷贝对象
来源：http://dp.haigaiapp.cn

Py:   copy.deepcopy(obj)
来源：http://du.muxihuayi.cn

PHP:  unserialize(serialize($obj));
来源：http://in.nicolike.cn

JS:   structuredClone(obj)
来源：http://nv.panjiajie.cn

TS:   structuredClone(obj)
来源：http://wj.muxihuayi.cn


<!-- 参考信息 -->