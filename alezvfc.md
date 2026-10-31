代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://fl.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://so.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://op.gzmigu.cn

================================================================================
来源：http://hy.newstarts.cn

H. 异常与错误处理
来源：http://ru.jctech888.com.cn

================================================================================
来源：http://pj.gzmigu.cn

[H01] try / catch 基础
来源：http://of.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cc.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qb.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qm.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tf.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://er.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ir.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yc.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yx.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://tj.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wu.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ta.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jf.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ju.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zs.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vl.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vz.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://md.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://fa.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://ku.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zt.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://ye.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://ai.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jj.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tx.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bp.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uj.lnxyls.cn

[H04] 自定义异常类型
来源：http://at.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://sn.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://hd.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://st.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://wm.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tj.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://kf.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://yu.bjjhwx.cn

[H05] 捕获特定类型
来源：http://lo.haigaiapp.cn

Py:   except ValueError as e:
来源：http://dq.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ax.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://jq.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://bo.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://sm.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xs.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://sz.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kp.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://dr.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://xk.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hg.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sx.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dx.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://um.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ai.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://uw.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://ha.colortex.cn

[H07] 断言
来源：http://nd.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://th.nicolike.cn

PHP:  assert($x > 0);
来源：http://vk.asd995.cn

JS:   console.assert(x > 0);
来源：http://cd.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://xn.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://oy.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kl.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fz.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://pj.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://iq.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://zg.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jg.panjiajie.cn

JS:   e.message;  e.stack
来源：http://wp.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xd.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zr.lnxyls.cn

Go:   err.Error()
来源：http://wt.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ks.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ex.lnxyls.cn

[H09] 带错误码的异常
来源：http://lf.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wk.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://po.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wk.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bb.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://je.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ac.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ot.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ge.nicolike.cn

[H10] 资源自动释放
来源：http://er.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jh.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ps.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wp.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bn.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qz.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://ca.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cn.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pj.jctech888.com.cn

================================================================================
来源：http://qj.newstarts.cn

I. 正则表达式
来源：http://xi.jctech888.com.cn

================================================================================
来源：http://us.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://mm.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gw.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wx.asd995.cn

JS:   /\d+/.test(s)
来源：http://vn.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://hr.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mp.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hf.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://uj.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pp.nicolike.cn

[I02] 提取所有匹配
来源：http://nn.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://pe.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rh.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://my.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://hq.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wu.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xe.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://dl.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uh.szxytkj.cn

[I03] 提取捕获分组
来源：http://wf.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yx.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pq.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kh.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ij.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sh.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nc.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tl.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ie.yuexingan06.cn

[I04] 正则替换
来源：http://ys.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gd.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://px.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bn.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hz.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fm.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rb.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://co.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rm.shtwfgs.cn

[I05] 按正则拆分
来源：http://hg.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ai.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vq.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://sh.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://xp.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://vs.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mc.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ea.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ke.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bj.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sd.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nk.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rg.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ja.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zi.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yw.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pq.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lz.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://xr.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pr.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jy.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rj.chemitech.net.cn

TS:   /error/gim
来源：http://pt.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://du.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vh.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://cy.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ek.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ob.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zd.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mo.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bv.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xk.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fd.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bx.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qt.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fe.hnjuh.cn

================================================================================
来源：http://go.huixiangedu.cn

J. 日期与时间
来源：http://it.jianghongdianzi.cn

================================================================================
来源：http://at.shxzukj.cn

[J01] 获取当前时间
来源：http://ma.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vg.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zw.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://qm.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://sa.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://td.nszjky.cn

Go:   time.Now()
来源：http://te.wgjwhj.cn

Ruby: Time.now
来源：http://hs.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ao.chemitech.net.cn

[J02] 格式化输出
来源：http://uj.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zm.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lz.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ks.bookmarksfly.cn

TS:   d.toISOString()
来源：http://ye.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xu.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sc.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ds.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://at.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://ts.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pg.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wt.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://fa.asd995.cn

TS:   new Date("2024-01-02")
来源：http://zy.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vo.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pz.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://rg.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://py.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://my.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tn.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kn.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qi.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vj.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pe.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wm.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wl.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tm.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://ci.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://bg.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://du.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gm.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vz.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://us.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bc.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://ym.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hz.521024.cn

[J06] 计算两时间之差
来源：http://wk.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://cp.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://wn.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uo.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fk.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wf.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://mi.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://vl.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://fm.hnjuh.cn

[J07] 比较两个日期
来源：http://km.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://dz.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://de.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eh.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lf.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jw.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dl.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ic.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://ld.521024.cn

[J08] 提取年月日与星期
来源：http://rm.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fv.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sm.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ba.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ls.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dj.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jf.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rp.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tk.colortex.cn

[J09] 时区处理
来源：http://ze.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uf.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ya.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bm.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sj.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zz.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pr.bjjhwx.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cw.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uw.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://fn.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jd.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ct.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ly.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tg.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rd.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dg.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rs.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lo.shxzukj.cn

================================================================================
来源：http://pu.lnxyls.cn

K. JSON 与序列化
来源：http://ke.yuexingan06.cn

================================================================================
来源：http://mn.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://ht.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fb.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xq.asd995.cn

JS:   JSON.stringify(obj)
来源：http://hn.521024.cn

TS:   JSON.stringify(obj)
来源：http://cf.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fw.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://aa.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dh.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zx.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://xq.newstarts.cn

Py:   json.loads(s)
来源：http://bl.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bd.huanxung.cn

JS:   JSON.parse(s)
来源：http://hx.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ny.bjjhwx.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cn.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://uu.521024.cn

Ruby: JSON.parse(s)
来源：http://zu.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iw.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://za.jctech888.com.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ys.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cb.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uy.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ae.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pc.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xa.lnxyls.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vr.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pq.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://cx.huanxung.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jo.asd995.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://om.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://we.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ep.huixiangedu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xb.shxzukj.cn


<!-- 参考信息 -->