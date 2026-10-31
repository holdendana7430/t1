代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pt.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hu.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wx.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bg.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ls.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zy.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zs.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://tn.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hy.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hs.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vg.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lv.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nl.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tv.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kd.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://az.haigaiapp.cn

[H03] 主动抛出异常
来源：http://ip.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://er.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yo.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://js.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://zb.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pj.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fv.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jx.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gn.hahajie.cn

[H04] 自定义异常类型
来源：http://ub.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://fs.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xw.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://ac.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://yh.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://tg.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gq.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://fi.521024.cn

C#:   class MyException : Exception {}
来源：http://xj.nszjky.cn

[H05] 捕获特定类型
来源：http://lg.asd995.cn

Py:   except ValueError as e:
来源：http://wo.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ko.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://bs.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://eb.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://nm.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wo.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://gj.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bc.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://oe.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://lx.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ca.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sq.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://go.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lu.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://es.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://jf.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://ta.bjjhwx.cn

[H07] 断言
来源：http://kd.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://jp.szxytkj.cn

PHP:  assert($x > 0);
来源：http://hn.colortex.cn

JS:   console.assert(x > 0);
来源：http://mk.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://lq.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://li.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iu.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vk.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://vo.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://ze.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://yu.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://db.shxzukj.cn

JS:   e.message;  e.stack
来源：http://jb.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uq.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nv.nszjky.cn

Go:   err.Error()
来源：http://hl.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://gh.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://wt.yuexingan06.cn

[H09] 带错误码的异常
来源：http://oh.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jw.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wl.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://is.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cq.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://js.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zp.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fv.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kb.lnxyls.cn

[H10] 资源自动释放
来源：http://so.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wd.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gb.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eu.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mm.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ah.chemitech.net.cn

Go:   defer f.Close()
来源：http://ri.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tu.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kq.huixinmuqiang.cn

================================================================================
来源：http://sx.haigaiapp.cn

I. 正则表达式
来源：http://in.shtwfgs.cn

================================================================================
来源：http://pz.wgjwhj.cn

[I01] 判断是否匹配
来源：http://qo.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ng.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xv.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://zc.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://da.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kr.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wm.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://iy.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qa.nszjky.cn

[I02] 提取所有匹配
来源：http://mc.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://sz.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oi.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ut.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://ll.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tl.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mv.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://jk.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qj.szxytkj.cn

[I03] 提取捕获分组
来源：http://uf.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://id.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yj.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gq.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nr.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jh.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fg.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vt.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iv.9csxet.cn

[I04] 正则替换
来源：http://jv.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vg.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rn.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ot.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sv.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jt.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rk.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://si.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jh.colortex.cn

[I05] 按正则拆分
来源：http://lc.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sm.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://so.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ht.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://xj.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://ia.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zx.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bu.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ec.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ri.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sv.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uk.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lo.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mm.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fy.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yx.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ej.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ec.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://np.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nc.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pa.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ct.jctech888.com.cn

TS:   /error/gim
来源：http://pq.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cm.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wu.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://gg.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://da.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ng.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://op.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ah.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://do.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ef.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bb.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://su.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kb.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ol.yuexingan06.cn

================================================================================
来源：http://nf.yuexingan06.cn

J. 日期与时间
来源：http://zk.shxzukj.cn

================================================================================
来源：http://yi.szsharing.cn

[J01] 获取当前时间
来源：http://nw.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://be.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lt.521024.cn

JS:   new Date();  Date.now()
来源：http://cc.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://wf.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zk.newstarts.cn

Go:   time.Now()
来源：http://sx.nicolike.cn

Ruby: Time.now
来源：http://pg.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hm.hahajie.cn

[J02] 格式化输出
来源：http://qn.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qm.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fz.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lb.panjiajie.cn

TS:   d.toISOString()
来源：http://fg.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ys.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zq.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aw.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ny.szsharing.cn

[J03] 字符串解析为日期
来源：http://sd.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kd.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qz.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://dq.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://ha.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dn.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rs.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://wt.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://od.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://qo.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fn.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hm.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jc.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oz.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ox.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://an.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kw.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wi.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://tb.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://pw.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yh.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://my.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://te.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://rb.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kx.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://un.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xe.muxihuayi.cn

[J06] 计算两时间之差
来源：http://fg.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://fb.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://wn.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ig.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vw.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://iv.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://bn.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://dw.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://sh.huixiangedu.cn

[J07] 比较两个日期
来源：http://zz.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://ha.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ji.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sd.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vh.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fh.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nc.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wm.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://ma.hahajie.cn

[J08] 提取年月日与星期
来源：http://sc.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gi.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xo.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aq.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ef.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nf.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://if.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mb.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ec.nicolike.cn

[J09] 时区处理
来源：http://bc.szxytkj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ha.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dy.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kw.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sc.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yt.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fe.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://me.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bw.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://mr.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fb.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vl.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zl.szsharing.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qa.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gp.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kd.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rz.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jc.newstarts.cn

================================================================================
来源：http://wb.gzmigu.cn

K. JSON 与序列化
来源：http://ur.newstarts.cn

================================================================================
来源：http://st.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://qi.yuntaijiaju.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yt.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oe.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://dt.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://qp.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://th.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://yw.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zb.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qz.bookmarksfly.cn

[K02] JSON 字符串转对象
来源：http://mh.colortex.cn

Py:   json.loads(s)
来源：http://vq.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tw.newstarts.cn

JS:   JSON.parse(s)
来源：http://jt.gzmigu.cn

TS:   JSON.parse(s)
来源：http://jf.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ey.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://uj.yuexingan06.cn

Ruby: JSON.parse(s)
来源：http://ar.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://im.yuntaijiaju.cn

[K03] JSON 美化输出（带缩进）
来源：http://gh.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mr.521024.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://em.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xv.huixiangedu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gi.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pg.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nj.huixiangedu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ri.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cv.colortex.cn

[K04] 读取 JSON 文件
来源：http://ui.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vm.huixiangedu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://el.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qw.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fs.yuexingan06.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ea.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://np.yuexingan06.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ev.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hi.muxihuayi.cn

[K05] 深拷贝对象
来源：http://is.panjiajie.cn

Py:   copy.deepcopy(obj)
来源：http://fr.521024.cn

PHP:  unserialize(serialize($obj));
来源：http://xg.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://wk.lnxyls.cn

TS:   structuredClone(obj)
来源：http://oc.huanxung.cn


<!-- 参考信息 -->