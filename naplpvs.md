代发 wailian999

PHP:  get_object_vars($obj);
来源：http://ic.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://ot.szsharing.cn

TS:   Object.entries(obj)
来源：http://ef.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wt.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://no.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://rf.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://hf.nszjky.cn

================================================================================
来源：http://ze.521024.cn

H. 异常与错误处理
来源：http://jx.shxzukj.cn

================================================================================
来源：http://ca.hahajie.cn

[H01] try / catch 基础
来源：http://db.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yx.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sh.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sv.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ve.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yk.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ub.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ua.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lk.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://bo.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pp.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://np.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://na.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lv.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tu.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lg.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pu.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jw.shxzskj.cn

[H03] 主动抛出异常
来源：http://ex.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://ej.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ts.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://ux.521024.cn

TS:   throw new Error("错误信息");
来源：http://qt.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sg.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://um.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://py.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mc.521024.cn

[H04] 自定义异常类型
来源：http://ow.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://fd.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sa.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://ui.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://kx.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://it.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rz.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://ye.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://pv.nicolike.cn

[H05] 捕获特定类型
来源：http://il.panjiajie.cn

Py:   except ValueError as e:
来源：http://tq.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://so.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ep.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://sw.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://vq.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vs.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://iq.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ka.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://qe.nszjky.cn

Py:   value = d.get("k") or default
来源：http://zu.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uw.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ju.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://az.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ll.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cp.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://ba.521024.cn

C#:   obj?.A?.B ?? default
来源：http://xy.nszjky.cn

[H07] 断言
来源：http://bb.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://dr.hahajie.cn

PHP:  assert($x > 0);
来源：http://id.9csxet.cn

JS:   console.assert(x > 0);
来源：http://qq.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://cr.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://of.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bg.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xr.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://ci.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://nz.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://su.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jg.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://jz.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wx.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yz.shxzukj.cn

Go:   err.Error()
来源：http://wh.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://bd.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://yz.newstarts.cn

[H09] 带错误码的异常
来源：http://lr.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ft.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gz.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://er.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hc.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dh.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rx.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yx.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oe.huixiangedu.cn

[H10] 资源自动释放
来源：http://ol.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ll.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rx.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mq.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://on.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mw.yuexingan06.cn

Go:   defer f.Close()
来源：http://ia.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kw.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ww.newstarts.cn

================================================================================
来源：http://sr.bookmarksfly.cn

I. 正则表达式
来源：http://tv.chemitech.net.cn

================================================================================
来源：http://qh.colortex.cn

[I01] 判断是否匹配
来源：http://nd.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rh.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xp.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://qi.newstarts.cn

TS:   /\d+/.test(s)
来源：http://sg.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://or.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ug.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://vx.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://il.shtwfgs.cn

[I02] 提取所有匹配
来源：http://hy.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://wl.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qo.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://li.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://as.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sr.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yz.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://th.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ly.shxzukj.cn

[I03] 提取捕获分组
来源：http://am.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kz.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cf.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cz.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jz.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iu.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ud.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rk.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mm.yuntaijiaju.cn

[I04] 正则替换
来源：http://xn.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ns.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gm.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ed.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ov.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qg.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ij.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mg.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vs.newstarts.cn

[I05] 按正则拆分
来源：http://um.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sa.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mk.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://os.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://yt.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://mr.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jv.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uq.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nr.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dc.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ez.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cl.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wy.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eb.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://di.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://de.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jb.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ra.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://pp.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xm.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uc.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ay.521024.cn

TS:   /error/gim
来源：http://av.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wm.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sf.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://od.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://io.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://rl.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ow.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yv.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gx.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tk.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tp.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ss.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xf.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vg.panjiajie.cn

================================================================================
来源：http://ov.wgjwhj.cn

J. 日期与时间
来源：http://ca.nszjky.cn

================================================================================
来源：http://hk.bookmarksfly.cn

[J01] 获取当前时间
来源：http://pm.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lw.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://um.nicolike.cn

JS:   new Date();  Date.now()
来源：http://vp.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ov.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xm.yuntaijiaju.cn

Go:   time.Now()
来源：http://zd.nicolike.cn

Ruby: Time.now
来源：http://xs.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bz.newstarts.cn

[J02] 格式化输出
来源：http://ju.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ul.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iw.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uz.chemitech.net.cn

TS:   d.toISOString()
来源：http://kv.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qk.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ah.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ju.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pi.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://wo.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://th.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mb.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://le.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://lq.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cr.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nt.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://yl.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jl.nicolike.cn

[J04] 时间戳与日期互转
来源：http://yd.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ch.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uv.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kl.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ps.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jh.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ub.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://df.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wu.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://co.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://oi.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zw.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vc.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tn.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://bh.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fi.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://qk.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rq.huixiangedu.cn

[J06] 计算两时间之差
来源：http://jy.521024.cn

Py:   (end - start).total_seconds()
来源：http://xx.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://fo.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tf.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nb.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vj.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://wj.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://ff.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://ui.9csxet.cn

[J07] 比较两个日期
来源：http://kh.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://xm.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tu.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bu.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xn.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xv.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mr.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yl.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://im.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://xt.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kl.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dx.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uz.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cq.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ak.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cd.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gj.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jj.yuntaijiaju.cn

[J09] 时区处理
来源：http://fa.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vw.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ro.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sr.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dg.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wl.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zp.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yf.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pk.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://ex.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aq.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cl.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jc.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wb.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ty.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mv.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hc.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oc.yuexingan06.cn

================================================================================
来源：http://xj.szxytkj.cn

K. JSON 与序列化
来源：http://vv.huixiangedu.cn

================================================================================
来源：http://ew.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://hw.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fy.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pe.521024.cn

JS:   JSON.stringify(obj)
来源：http://au.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://aj.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oe.szsharing.cn

Go:   json.Marshal(obj)
来源：http://ie.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yv.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tp.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://mk.szsharing.cn

Py:   json.loads(s)
来源：http://xf.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ae.szxytkj.cn

JS:   JSON.parse(s)
来源：http://mj.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://av.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yp.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://ml.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://qh.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dr.nszjky.cn

[K03] JSON 美化输出（带缩进）
来源：http://aj.szsharing.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dz.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bb.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aw.jianghongdianzi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oo.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ct.jianghongdianzi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wr.panjiajie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pc.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jz.szxytkj.cn

[K04] 读取 JSON 文件
来源：http://uh.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yp.panjiajie.cn


<!-- 参考信息 -->