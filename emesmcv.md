代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://po.shxzukj.cn

Ruby: obj.instance_variables
来源：http://md.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://pl.asd995.cn

================================================================================
来源：http://pg.yuntaijiaju.cn

H. 异常与错误处理
来源：http://uf.szsharing.cn

================================================================================
来源：http://ov.szsharing.cn

[H01] try / catch 基础
来源：http://xk.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bs.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ni.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xg.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xd.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vd.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ig.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://je.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tp.colortex.cn

[H02] finally / ensure 收尾
来源：http://ki.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gx.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xk.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pp.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nu.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ub.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oj.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xa.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aq.huanxung.cn

[H03] 主动抛出异常
来源：http://tf.521024.cn

Py:   raise ValueError("错误信息")
来源：http://qb.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jl.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://mn.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://li.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wp.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gk.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tr.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ei.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://br.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://oq.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jg.asd995.cn

JS:   class MyError extends Error {}
来源：http://vm.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://ly.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://wr.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pg.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://hw.szsharing.cn

C#:   class MyException : Exception {}
来源：http://pc.nszjky.cn

[H05] 捕获特定类型
来源：http://gt.muxihuayi.cn

Py:   except ValueError as e:
来源：http://rj.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gf.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://gc.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://or.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://ik.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rb.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://oy.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ya.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://sf.hahajie.cn

Py:   value = d.get("k") or default
来源：http://up.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ma.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wd.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://js.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mu.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ot.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ve.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://ti.9csxet.cn

[H07] 断言
来源：http://hf.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://hm.shxzskj.cn

PHP:  assert($x > 0);
来源：http://vg.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://zw.hahajie.cn

TS:   console.assert(x > 0);
来源：http://zp.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://ni.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cz.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ug.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://vf.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://ts.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://ul.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ds.shxzskj.cn

JS:   e.message;  e.stack
来源：http://ne.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xl.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yg.szsharing.cn

Go:   err.Error()
来源：http://er.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://kd.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://bs.hnjuh.cn

[H09] 带错误码的异常
来源：http://wg.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gw.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oc.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nt.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nz.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://df.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ih.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ok.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ct.bjjhwx.cn

[H10] 资源自动释放
来源：http://wg.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ps.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aq.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ky.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ch.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jo.gzmigu.cn

Go:   defer f.Close()
来源：http://cq.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hy.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kp.nicolike.cn

================================================================================
来源：http://vk.gzmigu.cn

I. 正则表达式
来源：http://ut.asd995.cn

================================================================================
来源：http://hm.szxytkj.cn

[I01] 判断是否匹配
来源：http://dm.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ud.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yy.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://gg.newstarts.cn

TS:   /\d+/.test(s)
来源：http://gc.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://db.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vq.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://to.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ho.szsharing.cn

[I02] 提取所有匹配
来源：http://qp.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://eq.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kk.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ib.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://du.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ei.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vd.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://dw.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vj.hahajie.cn

[I03] 提取捕获分组
来源：http://cn.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sd.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ap.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bu.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cd.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://us.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ap.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cm.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wm.panjiajie.cn

[I04] 正则替换
来源：http://ca.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://we.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jb.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wp.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fe.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sy.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tr.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zj.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mz.jctech888.com.cn

[I05] 按正则拆分
来源：http://jo.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eg.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lh.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://gy.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://mq.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://rc.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iu.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nj.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cm.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ze.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iz.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mr.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ds.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nk.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gd.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ir.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ry.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hg.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://vm.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sb.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fx.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bb.wgjwhj.cn

TS:   /error/gim
来源：http://tp.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ww.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pa.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://ij.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zc.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://gb.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ka.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zf.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ig.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ue.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nq.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nc.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wt.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ao.asd995.cn

================================================================================
来源：http://dr.bjjhwx.cn

J. 日期与时间
来源：http://df.nszjky.cn

================================================================================
来源：http://sj.muxihuayi.cn

[J01] 获取当前时间
来源：http://rq.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lu.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vi.huanxung.cn

JS:   new Date();  Date.now()
来源：http://di.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://na.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xd.jianghongdianzi.cn

Go:   time.Now()
来源：http://pw.shxzukj.cn

Ruby: Time.now
来源：http://wf.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://db.gzmigu.cn

[J02] 格式化输出
来源：http://bw.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rr.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gi.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qa.chemitech.net.cn

TS:   d.toISOString()
来源：http://sq.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jn.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xv.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dv.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://so.nicolike.cn

[J03] 字符串解析为日期
来源：http://yj.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eg.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vw.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://fb.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://ml.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sp.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ya.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://zs.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xw.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://ww.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ya.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rf.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://js.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gu.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pv.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pc.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://md.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sm.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://nx.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://mb.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vw.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pr.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ey.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://ld.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jw.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://dy.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lq.muxihuayi.cn

[J06] 计算两时间之差
来源：http://vs.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://zt.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://fp.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ia.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gq.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ji.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://jg.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://vp.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://ml.shxzskj.cn

[J07] 比较两个日期
来源：http://fm.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://uh.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dp.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rw.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pf.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xf.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xf.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://om.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://zs.szxytkj.cn

[J08] 提取年月日与星期
来源：http://og.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ev.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://im.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pj.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pa.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ak.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mf.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rd.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wz.newstarts.cn

[J09] 时区处理
来源：http://so.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ie.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://du.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jd.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ed.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pd.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vi.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ew.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kt.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://gf.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ug.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oj.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ez.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ri.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zw.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ay.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nx.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ll.chemitech.net.cn

================================================================================
来源：http://se.bjjhwx.cn

K. JSON 与序列化
来源：http://pf.lnxyls.cn

================================================================================
来源：http://fr.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://ph.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rb.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hi.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://sr.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://hq.asd995.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bm.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://mz.jianghongdianzi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tc.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qn.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://rp.shxzskj.cn

Py:   json.loads(s)
来源：http://xl.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sp.szxytkj.cn

JS:   JSON.parse(s)
来源：http://uo.colortex.cn

TS:   JSON.parse(s)
来源：http://ac.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pd.muxihuayi.cn

Go:   json.Unmarshal(data, &v)
来源：http://km.shxzukj.cn

Ruby: JSON.parse(s)
来源：http://eu.gzmigu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ug.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://pj.wgjwhj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sw.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yp.asd995.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tq.huanxung.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pk.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sa.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rf.jctech888.com.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lz.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uz.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://cb.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lz.shxzskj.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dk.nicolike.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://br.szsharing.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xk.nicolike.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vc.chemitech.net.cn


<!-- 参考信息 -->