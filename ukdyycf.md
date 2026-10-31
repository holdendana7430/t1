代发 wailian999

PHP:  get_object_vars($obj);
来源：http://rc.shxzukj.cn

JS:   Object.entries(obj)
来源：http://df.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://sc.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jw.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oj.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://me.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://dk.huixinmuqiang.cn

================================================================================
来源：http://de.lnxyls.cn

H. 异常与错误处理
来源：http://cg.nicolike.cn

================================================================================
来源：http://mf.huixiangedu.cn

[H01] try / catch 基础
来源：http://lp.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cg.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wb.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://py.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://it.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dl.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yv.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kz.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ni.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://nj.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://if.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iv.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sj.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bk.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qr.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pi.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qh.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gc.huanxung.cn

[H03] 主动抛出异常
来源：http://ge.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://pt.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cn.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://vn.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://qq.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sy.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fa.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tn.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iu.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://gi.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://ye.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xy.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://jt.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://vh.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://dv.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ck.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://ch.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://kz.szsharing.cn

[H05] 捕获特定类型
来源：http://an.shxzukj.cn

Py:   except ValueError as e:
来源：http://lo.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ip.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://zt.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://op.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://km.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zv.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://qw.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ad.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://am.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://zn.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vn.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://co.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kt.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cc.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uc.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://mk.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://pd.9csxet.cn

[H07] 断言
来源：http://lo.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://ie.shxzukj.cn

PHP:  assert($x > 0);
来源：http://ut.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://ml.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://af.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://dz.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xl.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xn.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://as.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://vs.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://ev.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kf.panjiajie.cn

JS:   e.message;  e.stack
来源：http://gx.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wv.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tw.shtwfgs.cn

Go:   err.Error()
来源：http://pb.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://dl.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://dh.hahajie.cn

[H09] 带错误码的异常
来源：http://kd.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://de.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ex.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vb.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pu.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://td.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zt.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bg.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ig.muxihuayi.cn

[H10] 资源自动释放
来源：http://qx.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bg.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lr.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sm.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://un.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kh.huanxung.cn

Go:   defer f.Close()
来源：http://qu.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ra.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ue.shxzukj.cn

================================================================================
来源：http://rt.muxihuayi.cn

I. 正则表达式
来源：http://ql.gzmigu.cn

================================================================================
来源：http://wd.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://fp.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fp.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wt.huanxung.cn

JS:   /\d+/.test(s)
来源：http://ti.huanxung.cn

TS:   /\d+/.test(s)
来源：http://sx.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qu.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ko.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://fs.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lt.nicolike.cn

[I02] 提取所有匹配
来源：http://tr.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://mv.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hr.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ql.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://iy.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gs.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jt.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://tw.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ji.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://ru.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aq.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qc.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jq.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rl.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eg.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jp.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rk.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://du.huixinmuqiang.cn

[I04] 正则替换
来源：http://sk.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xj.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jx.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bf.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hb.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mj.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bx.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://km.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lt.nicolike.cn

[I05] 按正则拆分
来源：http://he.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://au.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nw.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://by.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://wg.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://ju.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://no.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zw.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ww.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dr.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bf.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hq.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ch.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zw.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pz.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hh.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cj.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hp.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://sr.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gw.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zh.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qv.wgjwhj.cn

TS:   /error/gim
来源：http://nz.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xe.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nm.asd995.cn

Ruby: s.scan(/error/i)
来源：http://sq.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://az.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://oe.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://da.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lk.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lu.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kz.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pf.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qz.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sn.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nu.wgjwhj.cn

================================================================================
来源：http://gt.shtwfgs.cn

J. 日期与时间
来源：http://bd.yuntaijiaju.cn

================================================================================
来源：http://zg.hahajie.cn

[J01] 获取当前时间
来源：http://ef.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ak.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xs.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://sv.521024.cn

TS:   new Date();  Date.now()
来源：http://ge.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rb.bjjhwx.cn

Go:   time.Now()
来源：http://lb.panjiajie.cn

Ruby: Time.now
来源：http://su.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zq.gzmigu.cn

[J02] 格式化输出
来源：http://kt.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dx.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zi.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wi.shtwfgs.cn

TS:   d.toISOString()
来源：http://yt.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eq.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xp.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dk.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://av.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://uy.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vt.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qy.asd995.cn

JS:   new Date("2024-01-02")
来源：http://re.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://hg.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gn.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ex.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://tc.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ys.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://vr.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pm.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qv.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zj.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xa.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ne.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xp.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ar.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qo.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://wt.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://di.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qn.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dy.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yg.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://uk.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qm.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://zf.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yz.shtwfgs.cn

[J06] 计算两时间之差
来源：http://fi.asd995.cn

Py:   (end - start).total_seconds()
来源：http://jk.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://ba.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eh.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://et.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kv.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://ur.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://pl.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://qi.muxihuayi.cn

[J07] 比较两个日期
来源：http://ka.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ct.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xn.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mc.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qv.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vk.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://av.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hh.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://pl.panjiajie.cn

[J08] 提取年月日与星期
来源：http://gq.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jo.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cj.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jd.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cl.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uy.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pg.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hh.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uw.shxzskj.cn

[J09] 时区处理
来源：http://ym.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nb.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tw.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vp.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ff.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gl.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sl.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nf.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ew.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://ja.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pt.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zw.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hc.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hx.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://je.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://di.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ee.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gf.nszjky.cn

================================================================================
来源：http://kk.lnxyls.cn

K. JSON 与序列化
来源：http://yz.muxihuayi.cn

================================================================================
来源：http://gd.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://xl.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://or.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mj.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://uj.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://yu.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ou.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://hl.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kb.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xu.colortex.cn

[K02] JSON 字符串转对象
来源：http://in.shxzukj.cn

Py:   json.loads(s)
来源：http://tu.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dn.9csxet.cn

JS:   JSON.parse(s)
来源：http://io.panjiajie.cn

TS:   JSON.parse(s)
来源：http://el.lnxyls.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fz.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://yi.szxytkj.cn

Ruby: JSON.parse(s)
来源：http://db.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fu.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://pa.panjiajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://so.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jj.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rc.nicolike.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gz.panjiajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pp.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ks.szxytkj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oa.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fq.nicolike.cn

[K04] 读取 JSON 文件
来源：http://ww.shtwfgs.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fz.nszjky.cn


<!-- 参考信息 -->