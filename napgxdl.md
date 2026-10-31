代发 wailian999

H. 异常与错误处理
来源：http://jv.huixiangedu.cn

================================================================================
来源：http://yo.haigaiapp.cn

[H01] try / catch 基础
来源：http://eh.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qj.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dw.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ve.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://um.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qo.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xp.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wv.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eq.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://wn.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ii.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ry.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://go.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://so.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yq.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fy.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://my.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ur.9csxet.cn

[H03] 主动抛出异常
来源：http://jc.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://gs.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fw.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://yq.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://cr.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ss.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qs.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xe.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ke.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://yr.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://yx.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nb.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://ci.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://ue.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://nk.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sb.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://kq.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://it.yuexingan06.cn

[H05] 捕获特定类型
来源：http://yp.jctech888.com.cn

Py:   except ValueError as e:
来源：http://lx.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ks.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://xn.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://xu.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://tn.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://no.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://xz.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bh.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://zv.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://go.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qo.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qq.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ox.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dw.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qq.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://ab.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://pi.jctech888.com.cn

[H07] 断言
来源：http://ga.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://gb.colortex.cn

PHP:  assert($x > 0);
来源：http://zn.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://vr.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://ev.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://xd.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ir.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ce.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://yo.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://cd.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://km.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gh.shxzukj.cn

JS:   e.message;  e.stack
来源：http://ux.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eq.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pz.muxihuayi.cn

Go:   err.Error()
来源：http://ho.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://et.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://ms.hahajie.cn

[H09] 带错误码的异常
来源：http://yw.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jd.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kx.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ab.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://us.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vc.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yo.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wh.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://df.lnxyls.cn

[H10] 资源自动释放
来源：http://ko.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tq.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ty.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lu.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tl.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://um.wgjwhj.cn

Go:   defer f.Close()
来源：http://lx.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nx.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lm.bjjhwx.cn

================================================================================
来源：http://nz.shxzukj.cn

I. 正则表达式
来源：http://bi.huixinmuqiang.cn

================================================================================
来源：http://sm.szsharing.cn

[I01] 判断是否匹配
来源：http://vp.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://go.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kk.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://pg.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://up.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://za.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xg.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://rv.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://aj.9csxet.cn

[I02] 提取所有匹配
来源：http://dp.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://ih.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ux.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kg.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://cj.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tt.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ju.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://aj.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bp.9csxet.cn

[I03] 提取捕获分组
来源：http://if.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vq.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jo.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fw.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wl.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pc.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bm.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gq.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zy.newstarts.cn

[I04] 正则替换
来源：http://ew.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qk.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fb.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cu.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bt.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zm.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zl.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kl.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ch.szsharing.cn

[I05] 按正则拆分
来源：http://en.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ci.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fi.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://hd.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://us.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://lv.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jf.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nb.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://id.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bt.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zc.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wh.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mo.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ef.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pd.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jj.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gv.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://be.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://mk.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uw.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hm.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rc.gzmigu.cn

TS:   /error/gim
来源：http://vt.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wd.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qf.asd995.cn

Ruby: s.scan(/error/i)
来源：http://dw.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ta.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://vq.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ir.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vv.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xb.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oh.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xd.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qy.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rm.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tl.shtwfgs.cn

================================================================================
来源：http://bz.huixiangedu.cn

J. 日期与时间
来源：http://uz.shtwfgs.cn

================================================================================
来源：http://gu.bookmarksfly.cn

[J01] 获取当前时间
来源：http://ck.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xs.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lu.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://td.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://uc.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oo.chemitech.net.cn

Go:   time.Now()
来源：http://dw.hahajie.cn

Ruby: Time.now
来源：http://uc.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eb.huixinmuqiang.cn

[J02] 格式化输出
来源：http://vo.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fu.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ph.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lc.hnjuh.cn

TS:   d.toISOString()
来源：http://qc.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bu.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lx.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zc.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hl.szxytkj.cn

[J03] 字符串解析为日期
来源：http://fx.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xm.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yq.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://zc.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://qm.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yx.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gb.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://cq.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gg.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://zr.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ym.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dn.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lw.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jf.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xe.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bh.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zb.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ou.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://wz.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://gq.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lz.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://po.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nw.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://np.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ei.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://jq.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ba.asd995.cn

[J06] 计算两时间之差
来源：http://mi.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://ai.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://dv.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://my.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ek.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aw.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://jv.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://ce.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://yq.szsharing.cn

[J07] 比较两个日期
来源：http://hz.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://ve.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tu.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://np.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xw.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://by.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://re.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ly.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://eu.shxzukj.cn

[J08] 提取年月日与星期
来源：http://uz.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ua.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ru.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://td.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cs.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vn.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pb.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jm.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://au.chemitech.net.cn

[J09] 时区处理
来源：http://mt.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zu.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://du.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cz.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nr.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://em.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://be.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hs.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yu.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://yo.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xk.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zp.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hw.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wv.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bw.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nb.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nx.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yt.huanxung.cn

================================================================================
来源：http://pf.bookmarksfly.cn

K. JSON 与序列化
来源：http://dh.wgjwhj.cn

================================================================================
来源：http://sg.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://na.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oq.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uu.colortex.cn

JS:   JSON.stringify(obj)
来源：http://vk.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://oh.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fr.wgjwhj.cn

Go:   json.Marshal(obj)
来源：http://uk.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yu.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wx.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://yg.panjiajie.cn

Py:   json.loads(s)
来源：http://io.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ik.szsharing.cn

JS:   JSON.parse(s)
来源：http://ki.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://is.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pa.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://ow.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://ji.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qb.panjiajie.cn

[K03] JSON 美化输出（带缩进）
来源：http://vi.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ak.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ni.hnjuh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://se.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rn.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rc.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zr.shtwfgs.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ao.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ru.nszjky.cn

[K04] 读取 JSON 文件
来源：http://qb.wgjwhj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sn.jianghongdianzi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dy.huanxung.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iw.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rx.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dx.huixiangedu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sb.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://un.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://br.9csxet.cn


<!-- 参考信息 -->