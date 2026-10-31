代发 wailian999

PHP:  get_object_vars($obj);
来源：http://pq.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://wo.shxzukj.cn

TS:   Object.entries(obj)
来源：http://xt.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qz.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lj.hahajie.cn

Ruby: obj.instance_variables
来源：http://cx.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://pa.9csxet.cn

================================================================================
来源：http://we.asd995.cn

H. 异常与错误处理
来源：http://bw.muxihuayi.cn

================================================================================
来源：http://qo.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://sx.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://at.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pw.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ym.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://un.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wz.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rx.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xh.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yj.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://pm.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oc.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cn.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mb.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oo.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bn.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jv.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oh.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ul.lnxyls.cn

[H03] 主动抛出异常
来源：http://ng.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://vs.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://we.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://hu.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://hv.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jg.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zu.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ro.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pl.haigaiapp.cn

[H04] 自定义异常类型
来源：http://wk.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://iy.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ce.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://bh.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://nu.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://gn.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gy.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://qg.521024.cn

C#:   class MyException : Exception {}
来源：http://dr.bjjhwx.cn

[H05] 捕获特定类型
来源：http://wy.nszjky.cn

Py:   except ValueError as e:
来源：http://kp.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://du.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://pp.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://mm.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://jb.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ce.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://ye.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jt.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://rr.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://ra.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mu.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dr.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://og.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ha.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gn.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://sf.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://lb.shxzskj.cn

[H07] 断言
来源：http://fr.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://qx.asd995.cn

PHP:  assert($x > 0);
来源：http://nh.colortex.cn

JS:   console.assert(x > 0);
来源：http://hw.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://dw.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://qz.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ig.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yg.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://tz.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://ia.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://aw.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nh.panjiajie.cn

JS:   e.message;  e.stack
来源：http://ew.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://es.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ho.hahajie.cn

Go:   err.Error()
来源：http://rs.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://xn.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://fr.bjjhwx.cn

[H09] 带错误码的异常
来源：http://il.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aq.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://es.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lt.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dq.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pf.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wz.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qb.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qq.jctech888.com.cn

[H10] 资源自动释放
来源：http://of.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yk.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ce.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jz.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ks.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ed.nszjky.cn

Go:   defer f.Close()
来源：http://nx.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://om.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sq.chemitech.net.cn

================================================================================
来源：http://we.huixiangedu.cn

I. 正则表达式
来源：http://np.asd995.cn

================================================================================
来源：http://rv.9csxet.cn

[I01] 判断是否匹配
来源：http://uo.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yf.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tw.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://xo.nszjky.cn

TS:   /\d+/.test(s)
来源：http://ze.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nc.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://go.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://cr.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mn.haigaiapp.cn

[I02] 提取所有匹配
来源：http://da.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://wj.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qm.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mk.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://au.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sd.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://me.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://hn.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zw.lnxyls.cn

[I03] 提取捕获分组
来源：http://ul.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rz.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fi.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qg.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uq.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pc.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xq.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vv.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://px.shxzskj.cn

[I04] 正则替换
来源：http://uv.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qt.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ms.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://au.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lo.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wq.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xo.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bp.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sp.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://qs.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rm.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ec.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://ff.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ds.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://ws.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fr.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nw.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nv.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vg.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://na.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gj.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tm.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zb.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://de.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://he.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://in.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hj.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://ut.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jh.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fr.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://we.huixinmuqiang.cn

TS:   /error/gim
来源：http://aj.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nu.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dq.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://qv.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pj.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://mg.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xm.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hp.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ye.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pt.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ei.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ev.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ej.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ww.lnxyls.cn

================================================================================
来源：http://zd.hnjuh.cn

J. 日期与时间
来源：http://wb.huixinmuqiang.cn

================================================================================
来源：http://oo.chemitech.net.cn

[J01] 获取当前时间
来源：http://ex.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kq.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oi.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://lp.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://qh.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dj.yuntaijiaju.cn

Go:   time.Now()
来源：http://us.gzmigu.cn

Ruby: Time.now
来源：http://fm.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hn.bjjhwx.cn

[J02] 格式化输出
来源：http://nt.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rb.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lu.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lr.szxytkj.cn

TS:   d.toISOString()
来源：http://dd.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ow.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://al.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rc.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ax.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://wg.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dc.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jw.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://rd.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://jl.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fh.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://do.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://zb.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kq.colortex.cn

[J04] 时间戳与日期互转
来源：http://ic.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hk.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lv.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mq.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ez.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ad.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://md.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dq.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eq.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://lc.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://dl.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zs.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://em.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ez.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://lr.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uo.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://iz.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ty.shxzskj.cn

[J06] 计算两时间之差
来源：http://kd.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://sc.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://bz.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ta.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fo.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nn.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://bd.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://dn.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://mf.521024.cn

[J07] 比较两个日期
来源：http://xn.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://fr.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://an.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lf.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lu.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dm.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://if.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cv.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://sw.huanxung.cn

[J08] 提取年月日与星期
来源：http://ns.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qd.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cn.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sb.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ta.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vf.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pb.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cz.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hi.yuntaijiaju.cn

[J09] 时区处理
来源：http://bx.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vn.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sr.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dt.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xr.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kg.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rz.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rn.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xg.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://zs.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aq.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://js.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zi.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xe.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xi.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xh.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tb.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cz.shtwfgs.cn

================================================================================
来源：http://bt.bjjhwx.cn

K. JSON 与序列化
来源：http://zw.nicolike.cn

================================================================================
来源：http://kr.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://rp.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lz.nszjky.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mv.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://aw.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://zh.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ex.yuexingan06.cn

Go:   json.Marshal(obj)
来源：http://oi.521024.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sd.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jr.colortex.cn

[K02] JSON 字符串转对象
来源：http://yx.asd995.cn

Py:   json.loads(s)
来源：http://ia.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://du.yuexingan06.cn

JS:   JSON.parse(s)
来源：http://zi.lnxyls.cn

TS:   JSON.parse(s)
来源：http://sn.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qr.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://re.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://fm.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lo.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://ht.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ww.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mb.jianghongdianzi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oe.bookmarksfly.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mm.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ro.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sh.bjjhwx.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uz.gzmigu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fz.9csxet.cn

[K04] 读取 JSON 文件
来源：http://bf.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jj.bookmarksfly.cn


<!-- 参考信息 -->