代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kv.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ol.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://du.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aa.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ie.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gf.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nd.szsharing.cn

[H02] finally / ensure 收尾
来源：http://qc.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ri.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://la.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qa.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zf.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tx.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qb.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lo.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rn.muxihuayi.cn

[H03] 主动抛出异常
来源：http://sv.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://tw.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ha.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://ad.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://wx.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nx.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ct.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://en.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nv.huanxung.cn

[H04] 自定义异常类型
来源：http://jl.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://jj.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aw.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://gv.521024.cn

TS:   class MyError extends Error {}
来源：http://pn.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://lb.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pj.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://vd.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://yo.huanxung.cn

[H05] 捕获特定类型
来源：http://lk.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://ff.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pu.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://ud.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://ud.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://bz.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fq.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://gq.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nh.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://qx.colortex.cn

Py:   value = d.get("k") or default
来源：http://af.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cc.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ag.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sx.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mg.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dr.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://ij.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://be.hahajie.cn

[H07] 断言
来源：http://ng.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://hh.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://wf.szsharing.cn

JS:   console.assert(x > 0);
来源：http://qz.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://al.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://bn.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zb.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ux.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://uz.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://pz.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://pj.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jd.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://ap.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ky.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ml.shtwfgs.cn

Go:   err.Error()
来源：http://ea.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://ws.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://vb.chemitech.net.cn

[H09] 带错误码的异常
来源：http://to.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://co.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uh.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gr.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nx.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xb.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lc.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cq.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vh.wgjwhj.cn

[H10] 资源自动释放
来源：http://rw.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ag.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pp.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sx.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xo.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://os.haigaiapp.cn

Go:   defer f.Close()
来源：http://ev.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yx.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uh.wgjwhj.cn

================================================================================
来源：http://pb.shxzskj.cn

I. 正则表达式
来源：http://uo.chemitech.net.cn

================================================================================
来源：http://li.jctech888.com.cn

[I01] 判断是否匹配
来源：http://st.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qn.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xv.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://vl.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://ym.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://la.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ie.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://hi.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bw.huanxung.cn

[I02] 提取所有匹配
来源：http://uv.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://of.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rt.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lr.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://os.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fz.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vc.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://hp.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ir.szxytkj.cn

[I03] 提取捕获分组
来源：http://ph.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gf.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://su.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fs.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bw.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://is.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hr.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kt.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jg.shtwfgs.cn

[I04] 正则替换
来源：http://ka.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://aq.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kd.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ji.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cj.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hp.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fl.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qr.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hx.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://dy.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yq.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qs.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://zp.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://yg.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://th.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://po.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dd.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sa.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zt.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ap.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pp.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://au.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kx.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yc.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jk.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yw.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lx.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://mt.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vt.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fh.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mm.hnjuh.cn

TS:   /error/gim
来源：http://wh.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xq.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dp.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://rp.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pb.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://pr.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jq.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tm.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qy.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://li.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ce.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wk.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://am.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ee.shtwfgs.cn

================================================================================
来源：http://ah.nicolike.cn

J. 日期与时间
来源：http://ic.muxihuayi.cn

================================================================================
来源：http://xy.muxihuayi.cn

[J01] 获取当前时间
来源：http://is.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://af.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qn.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://ev.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://lp.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fg.nicolike.cn

Go:   time.Now()
来源：http://sn.nicolike.cn

Ruby: Time.now
来源：http://kc.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pa.gzmigu.cn

[J02] 格式化输出
来源：http://tv.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vu.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wx.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://id.newstarts.cn

TS:   d.toISOString()
来源：http://hz.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lt.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ga.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tt.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bn.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://nu.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ev.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ub.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://cy.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://pq.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uk.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jm.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://bs.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://va.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://dl.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hf.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ly.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ay.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bn.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zc.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hs.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uv.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gr.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://qx.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://pa.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ns.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ol.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lx.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://qr.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ec.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://wz.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xy.chemitech.net.cn

[J06] 计算两时间之差
来源：http://fm.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://lv.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://te.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ov.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bo.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://js.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://kn.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://pn.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://ca.hahajie.cn

[J07] 比较两个日期
来源：http://nh.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://kj.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://by.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ah.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rw.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dp.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ne.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://le.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://yq.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://im.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ax.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oe.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xg.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dr.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pw.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gy.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dz.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yi.lnxyls.cn

[J09] 时区处理
来源：http://ll.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yh.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rr.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lr.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qp.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eo.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tp.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mo.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tw.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://yx.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ei.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hw.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sq.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wm.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xw.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hk.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sl.shxzukj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oe.newstarts.cn

================================================================================
来源：http://wj.huixinmuqiang.cn

K. JSON 与序列化
来源：http://ig.nicolike.cn

================================================================================
来源：http://uv.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://tt.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ay.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yb.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://cs.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://pa.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nm.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://vz.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xn.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ik.hahajie.cn

[K02] JSON 字符串转对象
来源：http://sh.szxytkj.cn

Py:   json.loads(s)
来源：http://ul.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gq.521024.cn

JS:   JSON.parse(s)
来源：http://rb.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://yz.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://um.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://pz.panjiajie.cn

Ruby: JSON.parse(s)
来源：http://xv.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ku.hahajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://gs.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pg.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ur.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zl.haigaiapp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://im.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://og.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lw.hahajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sb.shxzukj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cx.huanxung.cn

[K04] 读取 JSON 文件
来源：http://qh.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aa.colortex.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ne.wgjwhj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ve.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://on.lnxyls.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://do.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://et.gzmigu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lo.jctech888.com.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ow.nszjky.cn

[K05] 深拷贝对象
来源：http://xt.hahajie.cn

Py:   copy.deepcopy(obj)
来源：http://tq.shtwfgs.cn

PHP:  unserialize(serialize($obj));
来源：http://ou.jctech888.com.cn

JS:   structuredClone(obj)
来源：http://js.nicolike.cn

TS:   structuredClone(obj)
来源：http://to.chemitech.net.cn


<!-- 参考信息 -->