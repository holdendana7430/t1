代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://ok.521024.cn

Ruby: obj.instance_variables
来源：http://zd.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://fw.huixiangedu.cn

================================================================================
来源：http://pm.haigaiapp.cn

H. 异常与错误处理
来源：http://xg.yuntaijiaju.cn

================================================================================
来源：http://ab.panjiajie.cn

[H01] try / catch 基础
来源：http://wx.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wd.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eh.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sa.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sl.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://um.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vv.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nr.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oo.nicolike.cn

[H02] finally / ensure 收尾
来源：http://vu.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://je.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yn.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ik.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ho.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tu.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://au.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wq.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sz.szsharing.cn

[H03] 主动抛出异常
来源：http://rz.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://oz.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jk.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://lc.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://zv.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iy.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pl.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sp.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ug.colortex.cn

[H04] 自定义异常类型
来源：http://ki.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://rn.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yf.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://sh.szsharing.cn

TS:   class MyError extends Error {}
来源：http://gb.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://ym.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wv.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://qz.huanxung.cn

C#:   class MyException : Exception {}
来源：http://av.9csxet.cn

[H05] 捕获特定类型
来源：http://yl.521024.cn

Py:   except ValueError as e:
来源：http://kt.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ym.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://pg.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://bv.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://la.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zd.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://cn.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wi.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://lw.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://kr.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lv.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wm.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yg.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jg.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://al.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://fs.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://qo.gzmigu.cn

[H07] 断言
来源：http://nf.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://mf.szsharing.cn

PHP:  assert($x > 0);
来源：http://ey.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://rf.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://sg.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://nh.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://py.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yt.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://og.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://zp.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://pc.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gp.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://na.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sr.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fq.lnxyls.cn

Go:   err.Error()
来源：http://qo.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://dg.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://ul.huanxung.cn

[H09] 带错误码的异常
来源：http://rt.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://at.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vm.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kc.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yx.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lz.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qd.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vc.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gi.szxytkj.cn

[H10] 资源自动释放
来源：http://px.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kt.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mj.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hf.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vi.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ta.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://vo.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nb.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hg.chemitech.net.cn

================================================================================
来源：http://ee.szxytkj.cn

I. 正则表达式
来源：http://yq.bjjhwx.cn

================================================================================
来源：http://ki.asd995.cn

[I01] 判断是否匹配
来源：http://hc.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wm.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sb.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://hc.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://ce.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hm.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yg.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://qt.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yw.newstarts.cn

[I02] 提取所有匹配
来源：http://fl.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://oi.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qg.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vv.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://ar.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iv.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://db.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://op.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uh.colortex.cn

[I03] 提取捕获分组
来源：http://zm.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zy.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kt.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mu.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ij.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://or.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aj.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wx.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lj.9csxet.cn

[I04] 正则替换
来源：http://iv.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bp.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gq.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qv.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tp.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ux.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jr.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mx.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pb.bookmarksfly.cn

[I05] 按正则拆分
来源：http://qp.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ug.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pi.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://mv.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rw.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://yy.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dq.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sl.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tn.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gr.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zh.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nz.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lx.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xp.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gw.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ji.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pp.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ww.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://fv.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mi.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ej.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dt.chemitech.net.cn

TS:   /error/gim
来源：http://ae.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tf.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hc.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://oq.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tx.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://tv.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fk.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ww.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xf.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rs.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dl.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qw.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ay.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hj.jctech888.com.cn

================================================================================
来源：http://ev.521024.cn

J. 日期与时间
来源：http://zo.shtwfgs.cn

================================================================================
来源：http://wy.lnxyls.cn

[J01] 获取当前时间
来源：http://yj.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://am.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nh.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://ln.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://io.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qb.szxytkj.cn

Go:   time.Now()
来源：http://qe.wgjwhj.cn

Ruby: Time.now
来源：http://am.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jm.jianghongdianzi.cn

[J02] 格式化输出
来源：http://mh.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ge.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hg.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uf.nicolike.cn

TS:   d.toISOString()
来源：http://ao.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fo.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ly.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://to.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mw.colortex.cn

[J03] 字符串解析为日期
来源：http://re.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wk.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://va.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://qm.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://tj.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cc.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mh.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://xb.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xj.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://sd.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cb.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oy.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ze.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lv.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vy.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fh.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uz.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dd.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://jm.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://jh.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jr.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pf.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://td.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://uo.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yx.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://xt.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tz.szxytkj.cn

[J06] 计算两时间之差
来源：http://qf.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://vk.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://aa.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gc.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ae.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ju.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://hf.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://uu.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://lk.yuexingan06.cn

[J07] 比较两个日期
来源：http://fk.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://uy.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xs.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zt.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pm.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jo.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nf.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ot.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://tq.colortex.cn

[J08] 提取年月日与星期
来源：http://ax.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hf.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oe.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pt.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ub.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ut.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cd.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rq.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sb.hnjuh.cn

[J09] 时区处理
来源：http://gc.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qz.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yn.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iq.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ej.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jx.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ka.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://me.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ga.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://zk.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dt.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://om.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yw.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vy.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rz.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ul.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uz.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bw.huixiangedu.cn

================================================================================
来源：http://vc.huanxung.cn

K. JSON 与序列化
来源：http://uz.521024.cn

================================================================================
来源：http://br.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://vk.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vx.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oq.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://yg.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://ps.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ko.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://sx.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cj.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ge.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://fc.huanxung.cn

Py:   json.loads(s)
来源：http://tu.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vd.shxzukj.cn

JS:   JSON.parse(s)
来源：http://ra.jctech888.com.cn

TS:   JSON.parse(s)
来源：http://es.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vl.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://xs.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://eg.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ad.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://pr.muxihuayi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vs.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vn.huixinmuqiang.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mg.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://se.jctech888.com.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jx.shxzukj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xm.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xd.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oq.lnxyls.cn

[K04] 读取 JSON 文件
来源：http://bc.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oh.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tb.haigaiapp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aq.bookmarksfly.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uo.bookmarksfly.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://er.bjjhwx.cn


<!-- 参考信息 -->