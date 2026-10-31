代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gh.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lz.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dv.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tt.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pj.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mz.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pz.nszjky.cn

[H02] finally / ensure 收尾
来源：http://zb.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sq.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yo.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tn.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pp.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iu.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jo.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ua.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zk.newstarts.cn

[H03] 主动抛出异常
来源：http://ue.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://xc.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://po.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://dx.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://yl.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://if.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lc.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cc.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mq.panjiajie.cn

[H04] 自定义异常类型
来源：http://sr.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://ti.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ig.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://bq.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://fh.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://aq.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tk.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://cu.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://af.nszjky.cn

[H05] 捕获特定类型
来源：http://fs.wgjwhj.cn

Py:   except ValueError as e:
来源：http://tg.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yk.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://sx.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://pv.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://qf.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vw.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://pu.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dy.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://pv.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://my.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kx.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hw.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hl.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ky.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wt.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://zk.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://ix.bookmarksfly.cn

[H07] 断言
来源：http://ut.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://qj.hahajie.cn

PHP:  assert($x > 0);
来源：http://cc.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://dj.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://ko.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://sc.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://em.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fr.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://ky.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://cy.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://am.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qd.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://in.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dh.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ta.hahajie.cn

Go:   err.Error()
来源：http://gy.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://jn.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://te.shtwfgs.cn

[H09] 带错误码的异常
来源：http://iv.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://al.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wn.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eq.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mk.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yu.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wd.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://at.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cc.haigaiapp.cn

[H10] 资源自动释放
来源：http://as.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lq.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dx.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yh.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fi.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bg.nicolike.cn

Go:   defer f.Close()
来源：http://il.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xk.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hi.shxzskj.cn

================================================================================
来源：http://un.chemitech.net.cn

I. 正则表达式
来源：http://lg.521024.cn

================================================================================
来源：http://wo.szxytkj.cn

[I01] 判断是否匹配
来源：http://pu.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zb.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://re.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://ub.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://ka.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cg.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hs.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://sw.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uh.panjiajie.cn

[I02] 提取所有匹配
来源：http://zy.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://fd.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vj.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dr.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://dl.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eo.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qu.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://dk.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://np.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://xj.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ao.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ki.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vz.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vf.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bs.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gc.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bp.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xb.haigaiapp.cn

[I04] 正则替换
来源：http://ly.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://le.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eg.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xt.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ug.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jh.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dn.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://as.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fb.jctech888.com.cn

[I05] 按正则拆分
来源：http://xq.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qh.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sp.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://vd.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://pt.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://ji.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hw.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dp.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ju.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://li.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ah.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yh.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ti.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qz.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mn.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iq.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ia.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hh.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://wy.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yo.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kz.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ih.nicolike.cn

TS:   /error/gim
来源：http://pk.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wm.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ij.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://lr.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zr.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://tr.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pc.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fj.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gn.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rd.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ln.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ag.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ro.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://os.jctech888.com.cn

================================================================================
来源：http://ax.hahajie.cn

J. 日期与时间
来源：http://fy.shxzukj.cn

================================================================================
来源：http://rw.muxihuayi.cn

[J01] 获取当前时间
来源：http://cd.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xj.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ph.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://mm.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ac.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bt.huixiangedu.cn

Go:   time.Now()
来源：http://vo.asd995.cn

Ruby: Time.now
来源：http://fj.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dv.shxzukj.cn

[J02] 格式化输出
来源：http://og.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://me.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fo.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pj.nicolike.cn

TS:   d.toISOString()
来源：http://dq.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ji.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bc.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wq.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mg.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://cb.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bv.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gq.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://xl.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://jv.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dh.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qn.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://cg.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://me.colortex.cn

[J04] 时间戳与日期互转
来源：http://rw.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kf.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sp.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tc.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uw.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rm.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kg.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xz.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://og.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://ii.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://sm.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://np.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://op.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jy.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://kc.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://av.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://gn.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vg.wgjwhj.cn

[J06] 计算两时间之差
来源：http://gm.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://ok.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://de.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qm.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tl.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://td.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://yl.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://ew.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://zr.panjiajie.cn

[J07] 比较两个日期
来源：http://ah.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://dh.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cb.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://li.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cg.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ms.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://na.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pc.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://nf.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://mt.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uc.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pc.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nj.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ff.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jg.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lg.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lr.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ys.hahajie.cn

[J09] 时区处理
来源：http://fb.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qj.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zu.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ni.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kp.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hq.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hq.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qg.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nw.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://uv.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tl.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rk.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vn.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://di.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cf.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tt.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://im.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nk.haigaiapp.cn

================================================================================
来源：http://ed.9csxet.cn

K. JSON 与序列化
来源：http://wv.lnxyls.cn

================================================================================
来源：http://uo.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://uu.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wf.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vh.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://fp.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://hh.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://up.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://bu.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mr.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iq.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://ad.gzmigu.cn

Py:   json.loads(s)
来源：http://wn.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ds.hahajie.cn

JS:   JSON.parse(s)
来源：http://ce.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://kp.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fe.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://jx.521024.cn

Ruby: JSON.parse(s)
来源：http://gy.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gi.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://pb.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eo.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://it.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ll.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hx.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tx.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jh.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://js.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ca.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://wl.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tl.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oi.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ba.panjiajie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fc.nszjky.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pg.newstarts.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nm.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xo.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ni.gzmigu.cn

[K05] 深拷贝对象
来源：http://ce.hnjuh.cn

Py:   copy.deepcopy(obj)
来源：http://cs.shxzukj.cn

PHP:  unserialize(serialize($obj));
来源：http://ek.huixiangedu.cn

JS:   structuredClone(obj)
来源：http://ct.521024.cn

TS:   structuredClone(obj)
来源：http://am.9csxet.cn


<!-- 参考信息 -->