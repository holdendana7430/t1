代发 wailian999

PHP:  get_object_vars($obj);
来源：http://wf.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://iy.szsharing.cn

TS:   Object.entries(obj)
来源：http://vf.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yb.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rm.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://sg.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://wi.yuntaijiaju.cn

================================================================================
来源：http://xj.asd995.cn

H. 异常与错误处理
来源：http://zt.jctech888.com.cn

================================================================================
来源：http://ys.hahajie.cn

[H01] try / catch 基础
来源：http://pc.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pv.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://po.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jp.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ha.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://et.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zt.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vj.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rm.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://mf.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mf.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vd.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ju.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cd.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://av.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vj.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jr.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gl.asd995.cn

[H03] 主动抛出异常
来源：http://af.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://rz.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iw.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://qf.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://kf.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tv.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dt.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lo.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tm.panjiajie.cn

[H04] 自定义异常类型
来源：http://eu.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://kx.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xr.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://rb.9csxet.cn

TS:   class MyError extends Error {}
来源：http://gr.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://rz.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eo.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://au.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://ac.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://dv.huixiangedu.cn

Py:   except ValueError as e:
来源：http://is.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vc.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://nt.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://wc.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://il.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dc.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://gq.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bl.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://oi.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://bu.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tr.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ww.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eq.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://na.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://do.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://fq.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://ls.szxytkj.cn

[H07] 断言
来源：http://uc.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://px.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://cq.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://oh.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://kw.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://bp.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://or.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wb.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://nu.521024.cn

[H08] 获取错误信息与堆栈
来源：http://mo.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ex.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ug.hahajie.cn

JS:   e.message;  e.stack
来源：http://ss.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hp.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hn.chemitech.net.cn

Go:   err.Error()
来源：http://vr.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://bs.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://ac.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://xo.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gy.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dc.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eb.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zq.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bh.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nn.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jl.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tg.jctech888.com.cn

[H10] 资源自动释放
来源：http://bo.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yx.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ii.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rj.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vf.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://to.asd995.cn

Go:   defer f.Close()
来源：http://mw.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nk.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ia.bookmarksfly.cn

================================================================================
来源：http://zx.panjiajie.cn

I. 正则表达式
来源：http://ii.jianghongdianzi.cn

================================================================================
来源：http://df.shxzskj.cn

[I01] 判断是否匹配
来源：http://pn.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ug.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tg.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://mi.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://oi.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ln.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ds.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://rx.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zg.asd995.cn

[I02] 提取所有匹配
来源：http://lj.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://qf.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://be.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ml.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://eo.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cu.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nh.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://tt.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tf.hnjuh.cn

[I03] 提取捕获分组
来源：http://tu.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xz.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ay.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pq.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ke.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sp.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://em.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ck.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pl.hnjuh.cn

[I04] 正则替换
来源：http://vu.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lj.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eq.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wv.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zj.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://is.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://no.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lw.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://un.chemitech.net.cn

[I05] 按正则拆分
来源：http://wx.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://be.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hg.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://vu.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://of.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://ct.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ay.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pu.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://az.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nu.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jp.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xr.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pp.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cy.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mg.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ai.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ec.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qc.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://sd.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://do.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://is.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bv.jctech888.com.cn

TS:   /error/gim
来源：http://rk.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bs.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eg.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://ju.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://du.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://cx.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pj.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qr.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wo.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ma.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lm.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yt.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lk.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bx.huanxung.cn

================================================================================
来源：http://im.jianghongdianzi.cn

J. 日期与时间
来源：http://fu.huanxung.cn

================================================================================
来源：http://wt.panjiajie.cn

[J01] 获取当前时间
来源：http://jn.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ay.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://en.9csxet.cn

JS:   new Date();  Date.now()
来源：http://lr.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://op.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fg.hahajie.cn

Go:   time.Now()
来源：http://jc.huixiangedu.cn

Ruby: Time.now
来源：http://cj.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bv.panjiajie.cn

[J02] 格式化输出
来源：http://zk.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xk.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mw.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://is.hnjuh.cn

TS:   d.toISOString()
来源：http://rm.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xa.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lc.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fu.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yk.shxzukj.cn

[J03] 字符串解析为日期
来源：http://ys.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tf.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ow.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://cy.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://hq.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tl.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yk.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ss.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gw.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://qw.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uk.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rd.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://el.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jo.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ne.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yy.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sx.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ot.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://lb.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://jm.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eb.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vd.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lx.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://yr.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lc.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://xg.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kr.colortex.cn

[J06] 计算两时间之差
来源：http://yf.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://ti.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://vq.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rp.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wk.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sd.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://yr.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://fd.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://og.shtwfgs.cn

[J07] 比较两个日期
来源：http://ej.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://vs.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://am.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iy.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kl.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bi.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://la.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yq.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://xh.asd995.cn

[J08] 提取年月日与星期
来源：http://xl.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mv.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jc.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mb.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qk.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vj.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ky.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tl.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fa.gzmigu.cn

[J09] 时区处理
来源：http://zl.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kn.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ts.huixinmuqiang.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ah.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://re.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aq.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zo.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eg.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rc.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://xe.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ic.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cf.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fw.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xs.521024.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rx.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vb.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yx.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hj.jctech888.com.cn

================================================================================
来源：http://sk.gzmigu.cn

K. JSON 与序列化
来源：http://yz.shtwfgs.cn

================================================================================
来源：http://bi.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://xg.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://no.bookmarksfly.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://er.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://yz.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://kf.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://na.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://ur.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qc.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sn.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://wz.szxytkj.cn

Py:   json.loads(s)
来源：http://ye.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://al.asd995.cn

JS:   JSON.parse(s)
来源：http://yx.9csxet.cn

TS:   JSON.parse(s)
来源：http://dt.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pi.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://jw.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://fg.shxzukj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://al.huanxung.cn

[K03] JSON 美化输出（带缩进）
来源：http://fc.jianghongdianzi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lp.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jc.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xo.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://il.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ak.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://av.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yr.nszjky.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://is.huanxung.cn

[K04] 读取 JSON 文件
来源：http://dl.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://op.haigaiapp.cn


<!-- 参考信息 -->