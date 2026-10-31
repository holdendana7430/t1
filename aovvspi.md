代发 wailian999

PHP:  get_object_vars($obj);
来源：http://qs.szxytkj.cn

JS:   Object.entries(obj)
来源：http://vv.szsharing.cn

TS:   Object.entries(obj)
来源：http://xa.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hl.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uk.colortex.cn

Ruby: obj.instance_variables
来源：http://df.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://um.9csxet.cn

================================================================================
来源：http://ab.yuntaijiaju.cn

H. 异常与错误处理
来源：http://sb.jianghongdianzi.cn

================================================================================
来源：http://sk.9csxet.cn

[H01] try / catch 基础
来源：http://oa.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ki.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://te.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tj.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pc.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://as.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uu.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qw.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dp.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://ck.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ix.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://de.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hn.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dn.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://am.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://us.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ne.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pi.colortex.cn

[H03] 主动抛出异常
来源：http://ka.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://ns.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fj.colortex.cn

JS:   throw new Error("错误信息");
来源：http://ae.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://tj.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://al.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gt.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hg.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ip.chemitech.net.cn

[H04] 自定义异常类型
来源：http://js.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://cl.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wg.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://re.hahajie.cn

TS:   class MyError extends Error {}
来源：http://wz.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://ae.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uu.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://cd.huanxung.cn

C#:   class MyException : Exception {}
来源：http://yb.panjiajie.cn

[H05] 捕获特定类型
来源：http://ki.shtwfgs.cn

Py:   except ValueError as e:
来源：http://tz.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hf.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://dc.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://vx.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://fo.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ec.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://po.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://an.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://su.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://po.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rs.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kp.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ya.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://su.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ag.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://dn.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://iu.hahajie.cn

[H07] 断言
来源：http://vo.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ca.nszjky.cn

PHP:  assert($x > 0);
来源：http://hr.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://bp.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://yd.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://tn.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ee.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dl.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://tg.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://hh.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://lb.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ru.hahajie.cn

JS:   e.message;  e.stack
来源：http://wv.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dq.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qd.shxzskj.cn

Go:   err.Error()
来源：http://ul.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://tl.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://kh.huanxung.cn

[H09] 带错误码的异常
来源：http://th.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ez.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wv.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hb.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://na.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kt.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fq.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sl.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://om.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://bc.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://al.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hq.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ba.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jr.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://la.wgjwhj.cn

Go:   defer f.Close()
来源：http://zv.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ia.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nw.gzmigu.cn

================================================================================
来源：http://fc.yuntaijiaju.cn

I. 正则表达式
来源：http://ka.shxzskj.cn

================================================================================
来源：http://ks.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://an.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ka.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lu.szsharing.cn

JS:   /\d+/.test(s)
来源：http://lm.asd995.cn

TS:   /\d+/.test(s)
来源：http://xn.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fb.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jf.521024.cn

Ruby: s.match?(/\d+/)
来源：http://jb.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vj.panjiajie.cn

[I02] 提取所有匹配
来源：http://sb.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://cb.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bt.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qw.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://gz.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ip.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zc.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://ap.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://na.szsharing.cn

[I03] 提取捕获分组
来源：http://nd.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gb.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ny.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oa.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ly.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sn.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rk.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ls.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bq.bookmarksfly.cn

[I04] 正则替换
来源：http://cf.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gz.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mp.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jm.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ig.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ey.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pw.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://db.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wg.nszjky.cn

[I05] 按正则拆分
来源：http://fl.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kt.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hm.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://by.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://cp.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://qm.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ss.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lj.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wz.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dd.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nd.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zh.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zs.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kh.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mw.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jt.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dr.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fi.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://tm.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mg.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qg.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cn.yuexingan06.cn

TS:   /error/gim
来源：http://gj.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://po.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bi.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://yw.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dw.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://uf.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nt.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nr.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ml.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lu.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xl.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ji.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://or.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uy.lnxyls.cn

================================================================================
来源：http://fc.gzmigu.cn

J. 日期与时间
来源：http://gk.nszjky.cn

================================================================================
来源：http://ue.muxihuayi.cn

[J01] 获取当前时间
来源：http://wf.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dg.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pr.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://oh.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://oa.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iz.gzmigu.cn

Go:   time.Now()
来源：http://ss.gzmigu.cn

Ruby: Time.now
来源：http://uj.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zd.lnxyls.cn

[J02] 格式化输出
来源：http://pg.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sn.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zz.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ai.hahajie.cn

TS:   d.toISOString()
来源：http://sr.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ym.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wf.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ko.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dr.nicolike.cn

[J03] 字符串解析为日期
来源：http://il.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ll.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ye.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://ab.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://oz.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ju.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ew.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://ml.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jg.hahajie.cn

[J04] 时间戳与日期互转
来源：http://lm.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://se.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://in.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rm.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://so.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bu.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ds.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zm.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fq.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://vt.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://jc.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qu.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://un.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hb.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://bi.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ub.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://rz.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://da.muxihuayi.cn

[J06] 计算两时间之差
来源：http://wz.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://aj.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://jd.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ma.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ip.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bt.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://sa.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://zp.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://pw.shtwfgs.cn

[J07] 比较两个日期
来源：http://fc.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://qy.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nb.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dk.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mp.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nt.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fc.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sc.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://cr.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://ey.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://an.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bm.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xq.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dt.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rv.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kz.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lh.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ai.szsharing.cn

[J09] 时区处理
来源：http://ve.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qt.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kq.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://go.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fs.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rq.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dg.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bd.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://rq.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hj.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qx.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bg.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pg.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vz.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ee.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://so.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ug.bjjhwx.cn

================================================================================
来源：http://rd.muxihuayi.cn

K. JSON 与序列化
来源：http://kn.lnxyls.cn

================================================================================
来源：http://kx.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://lp.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xd.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mz.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://wa.hnjuh.cn

TS:   JSON.stringify(obj)
来源：http://hf.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fg.newstarts.cn

Go:   json.Marshal(obj)
来源：http://lv.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fa.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iz.newstarts.cn

[K02] JSON 字符串转对象
来源：http://iq.bjjhwx.cn

Py:   json.loads(s)
来源：http://ck.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pc.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://wo.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://is.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oa.hahajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://tu.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://ux.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tc.bookmarksfly.cn

[K03] JSON 美化输出（带缩进）
来源：http://ak.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pa.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sy.hahajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bq.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vq.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dg.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tw.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qs.asd995.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sr.nicolike.cn

[K04] 读取 JSON 文件
来源：http://fj.yuntaijiaju.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://im.nszjky.cn


<!-- 参考信息 -->