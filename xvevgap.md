代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://iu.shxzukj.cn

Ruby: obj.instance_variables
来源：http://jy.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://as.hahajie.cn

================================================================================
来源：http://am.bookmarksfly.cn

H. 异常与错误处理
来源：http://cv.chemitech.net.cn

================================================================================
来源：http://md.bookmarksfly.cn

[H01] try / catch 基础
来源：http://gw.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gi.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ls.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zy.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iz.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rr.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://or.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xj.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ze.colortex.cn

[H02] finally / ensure 收尾
来源：http://gc.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pk.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fu.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zv.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pv.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dp.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ql.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ta.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rr.bjjhwx.cn

[H03] 主动抛出异常
来源：http://if.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://fo.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://of.asd995.cn

JS:   throw new Error("错误信息");
来源：http://di.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://rm.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pd.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lo.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://em.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ot.muxihuayi.cn

[H04] 自定义异常类型
来源：http://ab.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://ky.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ot.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://ag.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://qe.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://nj.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pp.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://sa.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://ju.asd995.cn

[H05] 捕获特定类型
来源：http://xm.hahajie.cn

Py:   except ValueError as e:
来源：http://yw.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://av.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://if.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://cb.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://kr.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rv.521024.cn

Ruby: rescue ArgumentError => e
来源：http://wx.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kj.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://ew.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://om.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mm.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bs.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wk.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hb.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://aa.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ub.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://bb.chemitech.net.cn

[H07] 断言
来源：http://er.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://hf.szsharing.cn

PHP:  assert($x > 0);
来源：http://ye.colortex.cn

JS:   console.assert(x > 0);
来源：http://bf.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://gz.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://hb.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kz.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kg.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://ec.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://wn.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://wh.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://td.hahajie.cn

JS:   e.message;  e.stack
来源：http://br.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yu.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mp.muxihuayi.cn

Go:   err.Error()
来源：http://gn.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://ok.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://ys.521024.cn

[H09] 带错误码的异常
来源：http://hf.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vm.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ur.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gm.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xa.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ff.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nw.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://et.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dp.huixiangedu.cn

[H10] 资源自动释放
来源：http://rr.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oe.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rg.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xb.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://io.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ex.wgjwhj.cn

Go:   defer f.Close()
来源：http://za.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tm.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://my.521024.cn

================================================================================
来源：http://wp.hahajie.cn

I. 正则表达式
来源：http://rw.yuexingan06.cn

================================================================================
来源：http://ke.bjjhwx.cn

[I01] 判断是否匹配
来源：http://yz.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vi.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://es.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://jk.nicolike.cn

TS:   /\d+/.test(s)
来源：http://jb.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vv.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bp.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://ll.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://av.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://po.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://io.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rz.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://so.colortex.cn

TS:   s.match(/\d+/g)
来源：http://fx.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wl.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aw.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://nd.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rr.huanxung.cn

[I03] 提取捕获分组
来源：http://mq.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nz.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zb.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lr.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ae.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kv.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zc.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qr.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ao.asd995.cn

[I04] 正则替换
来源：http://jv.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rr.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xv.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lo.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fo.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hx.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://os.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lf.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jg.szsharing.cn

[I05] 按正则拆分
来源：http://ee.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://md.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ef.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://jl.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://zw.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://mg.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mp.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wo.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yy.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yh.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ru.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ng.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dj.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kp.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sy.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rw.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fb.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ni.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://jj.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hd.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uw.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://df.szsharing.cn

TS:   /error/gim
来源：http://on.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hj.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kp.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://qf.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nr.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://qo.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xt.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ld.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lb.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lq.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iz.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ob.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://le.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://um.lnxyls.cn

================================================================================
来源：http://wv.bjjhwx.cn

J. 日期与时间
来源：http://oj.gzmigu.cn

================================================================================
来源：http://su.shtwfgs.cn

[J01] 获取当前时间
来源：http://qd.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rw.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sm.nszjky.cn

JS:   new Date();  Date.now()
来源：http://ia.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://uv.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ac.jctech888.com.cn

Go:   time.Now()
来源：http://qo.hnjuh.cn

Ruby: Time.now
来源：http://pm.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dl.shtwfgs.cn

[J02] 格式化输出
来源：http://xd.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://df.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hs.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qf.asd995.cn

TS:   d.toISOString()
来源：http://az.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ct.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ms.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://am.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zz.nicolike.cn

[J03] 字符串解析为日期
来源：http://hp.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://za.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ne.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://ga.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://yv.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uj.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kp.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://xs.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hb.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://dm.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yx.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bp.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nb.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ul.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dy.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hr.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zf.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eh.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://fj.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://qw.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ad.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xr.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aq.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://vp.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://km.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://ka.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mh.jctech888.com.cn

[J06] 计算两时间之差
来源：http://li.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://xo.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://uv.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oi.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gf.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pr.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://zd.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://md.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://wp.wgjwhj.cn

[J07] 比较两个日期
来源：http://bv.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://yt.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sy.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wx.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ug.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wt.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tx.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ty.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ma.9csxet.cn

[J08] 提取年月日与星期
来源：http://ro.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ps.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pn.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nn.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ko.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lj.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://py.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lg.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rc.yuntaijiaju.cn

[J09] 时区处理
来源：http://fw.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zh.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oq.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kk.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gu.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ib.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://il.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qn.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ze.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://qy.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ub.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ku.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lf.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://og.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tt.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qo.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://is.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ev.shtwfgs.cn

================================================================================
来源：http://wt.shxzskj.cn

K. JSON 与序列化
来源：http://jh.chemitech.net.cn

================================================================================
来源：http://re.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://hi.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nl.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dt.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://ao.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://kl.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://la.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://hq.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bq.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rm.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://gu.jctech888.com.cn

Py:   json.loads(s)
来源：http://pn.chemitech.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pm.nicolike.cn

JS:   JSON.parse(s)
来源：http://sn.bjjhwx.cn

TS:   JSON.parse(s)
来源：http://wm.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kt.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://mt.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://xu.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fj.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://ut.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ff.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xa.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dt.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nw.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rf.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hw.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bu.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vt.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://hf.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fd.wgjwhj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://er.bjjhwx.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kb.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ex.shxzukj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nx.chemitech.net.cn


<!-- 参考信息 -->