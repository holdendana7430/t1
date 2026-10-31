代发 wailian999

H. 异常与错误处理
来源：http://hj.nszjky.cn

================================================================================
来源：http://ig.nszjky.cn

[H01] try / catch 基础
来源：http://un.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lf.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://no.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ko.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fe.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ip.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://og.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gq.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xv.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://rb.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gl.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://my.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wr.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nk.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bv.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ge.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eq.muxihuayi.cn

[H03] 主动抛出异常
来源：http://bz.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://we.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fi.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://ty.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://fq.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ou.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://im.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://so.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ar.shxzukj.cn

[H04] 自定义异常类型
来源：http://aq.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://rq.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ud.colortex.cn

JS:   class MyError extends Error {}
来源：http://kz.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://si.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://ow.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yl.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://gw.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://vm.hahajie.cn

[H05] 捕获特定类型
来源：http://fa.wgjwhj.cn

Py:   except ValueError as e:
来源：http://kl.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pi.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://ld.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://ua.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://hb.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mq.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://st.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://np.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://qt.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://gi.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kc.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fr.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pa.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iu.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zx.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://io.521024.cn

C#:   obj?.A?.B ?? default
来源：http://vi.wgjwhj.cn

[H07] 断言
来源：http://lo.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://sv.shxzukj.cn

PHP:  assert($x > 0);
来源：http://sl.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://tc.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://mp.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://lk.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wc.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bk.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://fy.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://vg.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://rd.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zz.nszjky.cn

JS:   e.message;  e.stack
来源：http://ot.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xm.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hm.hahajie.cn

Go:   err.Error()
来源：http://rr.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://ei.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://qt.lnxyls.cn

[H09] 带错误码的异常
来源：http://pk.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vc.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jr.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tx.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yq.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cs.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ao.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://il.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cz.szsharing.cn

[H10] 资源自动释放
来源：http://ri.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gf.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jp.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ro.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mt.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eq.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://at.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pf.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ig.jctech888.com.cn

================================================================================
来源：http://de.bjjhwx.cn

I. 正则表达式
来源：http://th.shxzskj.cn

================================================================================
来源：http://lh.panjiajie.cn

[I01] 判断是否匹配
来源：http://ep.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mk.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gf.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://vt.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://kz.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gd.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rn.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://xn.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ul.haigaiapp.cn

[I02] 提取所有匹配
来源：http://ud.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://py.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vn.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ls.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://zv.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sl.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gc.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://bh.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zm.shtwfgs.cn

[I03] 提取捕获分组
来源：http://to.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ah.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lx.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wr.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yz.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wv.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gi.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iq.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ak.huixinmuqiang.cn

[I04] 正则替换
来源：http://qa.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jt.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wy.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dr.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ty.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rs.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://en.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zh.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mm.9csxet.cn

[I05] 按正则拆分
来源：http://vk.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sb.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ga.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://mp.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://yb.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://al.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://br.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hn.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hm.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rg.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wl.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zq.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hs.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ew.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jx.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tj.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wu.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zz.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://zz.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tu.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xy.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ub.colortex.cn

TS:   /error/gim
来源：http://bl.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pq.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yc.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://mf.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mq.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://xw.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pz.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rp.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ej.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pa.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fh.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uo.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vf.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hm.521024.cn

================================================================================
来源：http://fv.szsharing.cn

J. 日期与时间
来源：http://aq.bjjhwx.cn

================================================================================
来源：http://mt.newstarts.cn

[J01] 获取当前时间
来源：http://cd.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ar.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yf.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://xz.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://rs.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zw.nszjky.cn

Go:   time.Now()
来源：http://ej.yuntaijiaju.cn

Ruby: Time.now
来源：http://ow.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yl.gzmigu.cn

[J02] 格式化输出
来源：http://so.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qi.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tr.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tp.bookmarksfly.cn

TS:   d.toISOString()
来源：http://nl.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vo.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nc.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jb.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ah.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://lt.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gp.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fz.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://ks.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://jh.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ph.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ji.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ic.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rm.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://ed.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wi.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wv.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kk.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uh.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://po.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sx.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jm.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hg.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ys.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://su.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fm.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ri.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vj.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://jj.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yr.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://ad.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ff.521024.cn

[J06] 计算两时间之差
来源：http://ad.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://mm.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://hl.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nt.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lb.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oy.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://dz.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://ac.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://qe.yuexingan06.cn

[J07] 比较两个日期
来源：http://lf.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://wo.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ve.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aj.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sw.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://au.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gr.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zg.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://bl.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://nu.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://we.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sb.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rd.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://km.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://te.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mr.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xu.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hx.yuexingan06.cn

[J09] 时区处理
来源：http://tn.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ue.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pz.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dx.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wb.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://po.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ci.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://er.hahajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cb.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://yl.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sm.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bu.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kp.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iq.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ej.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ez.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hv.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wh.lnxyls.cn

================================================================================
来源：http://im.haigaiapp.cn

K. JSON 与序列化
来源：http://as.bookmarksfly.cn

================================================================================
来源：http://ma.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://bq.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qf.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xd.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://ew.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://sj.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://na.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://as.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sn.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ys.nszjky.cn

[K02] JSON 字符串转对象
来源：http://bh.huixiangedu.cn

Py:   json.loads(s)
来源：http://kn.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jn.shxzukj.cn

JS:   JSON.parse(s)
来源：http://ct.shxzukj.cn

TS:   JSON.parse(s)
来源：http://zr.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xn.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://lh.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://fr.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ca.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://ay.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://go.newstarts.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xb.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rp.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://me.jianghongdianzi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xt.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bv.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hi.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yb.nszjky.cn

[K04] 读取 JSON 文件
来源：http://at.9csxet.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tt.jctech888.com.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tk.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xn.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bn.chemitech.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rf.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kf.hahajie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fu.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mu.huanxung.cn

[K05] 深拷贝对象
来源：http://do.lnxyls.cn


<!-- 参考信息 -->