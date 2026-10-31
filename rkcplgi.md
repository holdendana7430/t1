代发 wailian999

H. 异常与错误处理
来源：http://to.yuntaijiaju.cn

================================================================================
来源：http://xj.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://vm.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ay.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iz.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tt.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wc.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dy.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://es.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tr.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vq.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://ch.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mm.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yy.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pw.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lr.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tc.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cu.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ql.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dw.nszjky.cn

[H03] 主动抛出异常
来源：http://jj.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://tj.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ip.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://ym.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://qb.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://da.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ls.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://iq.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vg.bjjhwx.cn

[H04] 自定义异常类型
来源：http://iv.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://wo.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cz.asd995.cn

JS:   class MyError extends Error {}
来源：http://lb.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://zy.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://xf.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qz.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://ng.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://iq.huanxung.cn

[H05] 捕获特定类型
来源：http://cd.hahajie.cn

Py:   except ValueError as e:
来源：http://hb.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://if.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://zj.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://rp.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://uu.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://th.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://no.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://js.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://mx.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://ps.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ay.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xo.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nc.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qd.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pj.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://jr.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://ts.newstarts.cn

[H07] 断言
来源：http://dz.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ah.hnjuh.cn

PHP:  assert($x > 0);
来源：http://fy.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://th.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://sn.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://xb.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mc.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ga.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://mq.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://rg.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://rj.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ic.szsharing.cn

JS:   e.message;  e.stack
来源：http://at.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ja.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ei.521024.cn

Go:   err.Error()
来源：http://mf.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://ga.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://lq.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ks.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sn.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gg.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bu.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wd.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sb.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://al.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cb.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rs.panjiajie.cn

[H10] 资源自动释放
来源：http://en.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wq.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ls.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ag.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jy.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rf.szsharing.cn

Go:   defer f.Close()
来源：http://rr.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vz.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iy.lnxyls.cn

================================================================================
来源：http://fg.chemitech.net.cn

I. 正则表达式
来源：http://lu.huixiangedu.cn

================================================================================
来源：http://xc.nicolike.cn

[I01] 判断是否匹配
来源：http://gn.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uk.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://at.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://yi.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://om.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rw.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wr.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://ij.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fc.hahajie.cn

[I02] 提取所有匹配
来源：http://qe.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://sl.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://la.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uq.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://ty.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zq.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tj.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://lt.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://af.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://sa.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ga.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://et.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zl.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://im.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gt.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zl.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fo.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ov.shxzukj.cn

[I04] 正则替换
来源：http://ae.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qs.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oi.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ij.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fo.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yq.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://my.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fm.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nz.gzmigu.cn

[I05] 按正则拆分
来源：http://mu.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bc.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ck.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://sc.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://wn.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://oo.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cz.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tv.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iv.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nh.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dy.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sc.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xp.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oy.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ss.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rp.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hn.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cm.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://mi.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ze.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://by.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ry.muxihuayi.cn

TS:   /error/gim
来源：http://rx.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mu.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mi.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://cm.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gm.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://bv.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gh.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qw.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tl.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dv.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://da.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xe.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://si.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dk.jctech888.com.cn

================================================================================
来源：http://hp.shtwfgs.cn

J. 日期与时间
来源：http://rz.bookmarksfly.cn

================================================================================
来源：http://dd.gzmigu.cn

[J01] 获取当前时间
来源：http://bv.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xq.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xj.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://av.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://qq.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://km.bjjhwx.cn

Go:   time.Now()
来源：http://au.lnxyls.cn

Ruby: Time.now
来源：http://si.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://od.nszjky.cn

[J02] 格式化输出
来源：http://kg.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wn.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fe.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ir.szsharing.cn

TS:   d.toISOString()
来源：http://zj.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://od.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ax.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jo.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ei.szsharing.cn

[J03] 字符串解析为日期
来源：http://bo.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ki.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fe.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://gx.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://vn.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://st.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tv.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://dl.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bq.521024.cn

[J04] 时间戳与日期互转
来源：http://eb.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dj.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://my.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wu.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wu.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bh.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kg.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nc.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ny.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://re.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://lz.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://us.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yl.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qp.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://xh.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://be.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://wl.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ae.asd995.cn

[J06] 计算两时间之差
来源：http://en.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://pb.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://en.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mo.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cd.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sh.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://qm.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://yz.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://fj.lnxyls.cn

[J07] 比较两个日期
来源：http://kf.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://ya.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fq.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mu.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qh.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bc.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zt.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fk.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://iq.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://uv.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dv.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nw.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xa.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ir.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://im.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rl.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rc.hahajie.cn

[J09] 时区处理
来源：http://ku.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ou.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ld.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://au.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://js.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hu.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ih.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jj.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://si.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://fz.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fh.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://si.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kw.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yq.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tb.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ft.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jz.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dg.gzmigu.cn

================================================================================
来源：http://ms.shxzskj.cn

K. JSON 与序列化
来源：http://hi.huixinmuqiang.cn

================================================================================
来源：http://nc.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://oy.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fq.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ev.colortex.cn

JS:   JSON.stringify(obj)
来源：http://vd.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://bb.colortex.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ir.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://zn.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dm.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://in.colortex.cn

[K02] JSON 字符串转对象
来源：http://ah.newstarts.cn

Py:   json.loads(s)
来源：http://he.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ub.newstarts.cn

JS:   JSON.parse(s)
来源：http://kf.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://kj.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cd.wgjwhj.cn

Go:   json.Unmarshal(data, &v)
来源：http://bo.hahajie.cn

Ruby: JSON.parse(s)
来源：http://dm.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gg.hnjuh.cn

[K03] JSON 美化输出（带缩进）
来源：http://uh.9csxet.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wf.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tz.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://af.asd995.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yn.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mf.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cm.newstarts.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ku.nicolike.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aj.hahajie.cn

[K04] 读取 JSON 文件
来源：http://zb.asd995.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tw.huanxung.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ra.9csxet.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dc.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pb.huanxung.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pw.shxzukj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xg.bookmarksfly.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://if.huixiangedu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wz.szsharing.cn

[K05] 深拷贝对象
来源：http://hj.panjiajie.cn


<!-- 参考信息 -->