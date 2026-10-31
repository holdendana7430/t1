代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hc.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://cr.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ug.colortex.cn

================================================================================
来源：http://pd.jianghongdianzi.cn

H. 异常与错误处理
来源：http://dj.jctech888.com.cn

================================================================================
来源：http://qf.hahajie.cn

[H01] try / catch 基础
来源：http://yg.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qt.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oa.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fv.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ms.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zc.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ky.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dx.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ve.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://qw.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sf.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kw.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oh.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vx.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qm.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jx.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nu.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uw.newstarts.cn

[H03] 主动抛出异常
来源：http://av.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://yu.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://av.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://ej.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://bc.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://np.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yx.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fm.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://va.colortex.cn

[H04] 自定义异常类型
来源：http://sj.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://qr.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wp.huanxung.cn

JS:   class MyError extends Error {}
来源：http://vb.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://tv.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://yd.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ls.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://bw.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://we.panjiajie.cn

[H05] 捕获特定类型
来源：http://xr.asd995.cn

Py:   except ValueError as e:
来源：http://ty.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nh.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://ys.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://bp.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://xc.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pg.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://tt.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iy.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://uu.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://tj.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vz.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zf.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fw.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xa.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pr.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ly.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://ch.shxzukj.cn

[H07] 断言
来源：http://ws.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://of.nicolike.cn

PHP:  assert($x > 0);
来源：http://yl.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://rs.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://sv.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://pd.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ko.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vl.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://yv.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://xb.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://fp.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xn.szsharing.cn

JS:   e.message;  e.stack
来源：http://ii.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nf.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ri.wgjwhj.cn

Go:   err.Error()
来源：http://hf.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://nk.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ew.wgjwhj.cn

[H09] 带错误码的异常
来源：http://sw.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://st.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://br.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bd.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mg.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pf.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rn.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rd.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://et.gzmigu.cn

[H10] 资源自动释放
来源：http://li.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gk.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gy.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sz.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yj.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://il.lnxyls.cn

Go:   defer f.Close()
来源：http://eh.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lw.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ww.chemitech.net.cn

================================================================================
来源：http://jq.521024.cn

I. 正则表达式
来源：http://op.nszjky.cn

================================================================================
来源：http://rx.521024.cn

[I01] 判断是否匹配
来源：http://zk.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lb.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qd.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://ql.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://qn.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xc.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hm.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://ec.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://za.asd995.cn

[I02] 提取所有匹配
来源：http://zf.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://gt.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kw.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ax.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://gl.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gf.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zu.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://wo.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gm.chemitech.net.cn

[I03] 提取捕获分组
来源：http://xn.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://di.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nh.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nt.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://og.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tx.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uj.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bq.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qf.wgjwhj.cn

[I04] 正则替换
来源：http://lo.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mh.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ru.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ld.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yo.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eg.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yp.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zz.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cy.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://wq.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zg.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ht.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://ut.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://ku.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://uy.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jo.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ts.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vg.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dy.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fu.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eq.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ls.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dk.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cv.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lv.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://se.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ij.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://ip.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qi.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tq.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sg.nszjky.cn

TS:   /error/gim
来源：http://kg.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vd.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sr.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://cl.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lg.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://bf.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nt.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yu.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dt.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xd.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ym.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mx.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://my.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gg.lnxyls.cn

================================================================================
来源：http://th.huixiangedu.cn

J. 日期与时间
来源：http://ux.panjiajie.cn

================================================================================
来源：http://nj.wgjwhj.cn

[J01] 获取当前时间
来源：http://wc.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ft.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://un.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://oc.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://qh.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xu.chemitech.net.cn

Go:   time.Now()
来源：http://zj.yuntaijiaju.cn

Ruby: Time.now
来源：http://sr.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gy.newstarts.cn

[J02] 格式化输出
来源：http://gc.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sq.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gc.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ib.521024.cn

TS:   d.toISOString()
来源：http://we.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xj.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://py.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gc.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ov.panjiajie.cn

[J03] 字符串解析为日期
来源：http://yw.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fb.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eq.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://cm.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://hz.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bb.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rd.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://wr.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wp.nicolike.cn

[J04] 时间戳与日期互转
来源：http://xy.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://za.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hk.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://da.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jk.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ed.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ju.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hm.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bp.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://mq.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://tt.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pz.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tk.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yd.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://zc.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://br.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://vn.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wn.haigaiapp.cn

[J06] 计算两时间之差
来源：http://fi.colortex.cn

Py:   (end - start).total_seconds()
来源：http://af.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://md.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dq.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://km.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ah.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://vx.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://zm.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://vp.asd995.cn

[J07] 比较两个日期
来源：http://vy.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ci.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kl.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gy.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hy.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nf.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qd.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cf.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://mp.nszjky.cn

[J08] 提取年月日与星期
来源：http://vc.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rb.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dm.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yh.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://to.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wc.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pz.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://td.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://as.gzmigu.cn

[J09] 时区处理
来源：http://oo.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rd.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vw.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://az.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oa.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hk.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pw.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cl.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pp.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://fd.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kj.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ly.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fc.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://at.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iy.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sq.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tp.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yh.yuntaijiaju.cn

================================================================================
来源：http://zr.wgjwhj.cn

K. JSON 与序列化
来源：http://qt.yuexingan06.cn

================================================================================
来源：http://gt.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://mq.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gy.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fz.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://qg.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://fz.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fe.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://qm.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aw.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wp.nszjky.cn

[K02] JSON 字符串转对象
来源：http://xn.yuexingan06.cn

Py:   json.loads(s)
来源：http://wd.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ei.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://pg.panjiajie.cn

TS:   JSON.parse(s)
来源：http://hz.panjiajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://of.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://bc.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://yl.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dc.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://sa.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hj.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wh.shtwfgs.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mx.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vo.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lr.asd995.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vg.yuexingan06.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fn.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mb.chemitech.net.cn

[K04] 读取 JSON 文件
来源：http://lv.huixinmuqiang.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lk.nszjky.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ro.yuntaijiaju.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kn.shxzukj.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dp.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hp.muxihuayi.cn


<!-- 参考信息 -->