代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://pc.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://uu.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://rv.chemitech.net.cn

================================================================================
来源：http://sa.nicolike.cn

H. 异常与错误处理
来源：http://jk.shtwfgs.cn

================================================================================
来源：http://po.haigaiapp.cn

[H01] try / catch 基础
来源：http://yv.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sf.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ws.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rq.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wu.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://th.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gw.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://op.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oy.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://va.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rp.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://av.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ts.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bm.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rc.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ml.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ez.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sz.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://ym.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://ib.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nj.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://ef.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://be.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ld.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ti.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xr.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mc.hnjuh.cn

[H04] 自定义异常类型
来源：http://nb.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://vv.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rh.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://yu.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://bs.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://ku.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ra.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://cf.newstarts.cn

C#:   class MyException : Exception {}
来源：http://gi.szsharing.cn

[H05] 捕获特定类型
来源：http://bl.wgjwhj.cn

Py:   except ValueError as e:
来源：http://ay.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ha.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://lw.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://oq.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://pn.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tg.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://fh.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pb.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://ac.nszjky.cn

Py:   value = d.get("k") or default
来源：http://ob.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uk.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://si.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ao.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xi.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nx.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://sd.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://pb.shxzukj.cn

[H07] 断言
来源：http://oh.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://xl.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://sz.szsharing.cn

JS:   console.assert(x > 0);
来源：http://kp.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://et.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://pc.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ue.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ln.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ns.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://jv.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://mt.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oo.gzmigu.cn

JS:   e.message;  e.stack
来源：http://nq.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qd.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://es.gzmigu.cn

Go:   err.Error()
来源：http://yr.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://sj.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ks.nicolike.cn

[H09] 带错误码的异常
来源：http://rd.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sj.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lm.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ll.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://do.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ie.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ue.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hb.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gw.panjiajie.cn

[H10] 资源自动释放
来源：http://zq.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fz.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://um.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bo.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pu.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iw.huanxung.cn

Go:   defer f.Close()
来源：http://fq.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lj.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wd.panjiajie.cn

================================================================================
来源：http://sp.colortex.cn

I. 正则表达式
来源：http://gy.szxytkj.cn

================================================================================
来源：http://ee.szsharing.cn

[I01] 判断是否匹配
来源：http://ch.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hc.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wf.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://ny.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://di.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vk.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pk.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://mq.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dh.shxzskj.cn

[I02] 提取所有匹配
来源：http://gy.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://vi.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qz.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fx.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://ww.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vf.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ra.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://oc.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ag.bjjhwx.cn

[I03] 提取捕获分组
来源：http://il.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gu.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xz.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yl.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vd.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hi.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mq.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dr.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nq.szsharing.cn

[I04] 正则替换
来源：http://wa.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vx.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mc.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ep.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ng.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ta.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rf.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://op.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lq.jctech888.com.cn

[I05] 按正则拆分
来源：http://ms.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ku.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gw.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://wr.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://af.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://oi.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cz.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pe.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ro.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ea.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sz.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qt.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hh.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jd.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ug.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jv.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kn.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eo.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://fg.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nn.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bw.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ue.hahajie.cn

TS:   /error/gim
来源：http://ar.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lz.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rv.asd995.cn

Ruby: s.scan(/error/i)
来源：http://vw.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vj.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://ho.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xu.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ux.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fl.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ds.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://or.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ap.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fp.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ny.bjjhwx.cn

================================================================================
来源：http://fd.shxzskj.cn

J. 日期与时间
来源：http://tz.yuntaijiaju.cn

================================================================================
来源：http://ex.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://tr.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pn.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gd.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ai.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://ty.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bd.szsharing.cn

Go:   time.Now()
来源：http://an.wgjwhj.cn

Ruby: Time.now
来源：http://eb.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ct.lnxyls.cn

[J02] 格式化输出
来源：http://pz.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ij.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://li.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tk.yuexingan06.cn

TS:   d.toISOString()
来源：http://fd.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bb.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wz.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gx.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://co.shxzukj.cn

[J03] 字符串解析为日期
来源：http://kb.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pe.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pr.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://pr.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://ao.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fz.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://md.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://zr.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gb.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://zj.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ng.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zv.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rn.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zd.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://an.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kt.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dm.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fv.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://ln.colortex.cn

Py:   now + timedelta(days=7)
来源：http://le.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://us.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ny.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pt.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ib.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://im.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://ht.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lj.nicolike.cn

[J06] 计算两时间之差
来源：http://bc.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://vv.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://or.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jf.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sj.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gc.521024.cn

Go:   end.Sub(start).Hours()
来源：http://zi.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://bb.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://az.szsharing.cn

[J07] 比较两个日期
来源：http://mb.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://pd.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hn.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tk.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xp.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bo.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://os.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lc.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://gl.szxytkj.cn

[J08] 提取年月日与星期
来源：http://jy.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vj.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ge.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bs.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ws.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cu.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hv.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hq.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dm.newstarts.cn

[J09] 时区处理
来源：http://tv.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yr.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qg.colortex.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://po.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nd.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vm.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://de.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xl.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dd.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://ez.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ju.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rc.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jm.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fp.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qz.jianghongdianzi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iz.jianghongdianzi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://td.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ch.hnjuh.cn

================================================================================
来源：http://nu.hnjuh.cn

K. JSON 与序列化
来源：http://th.bookmarksfly.cn

================================================================================
来源：http://ny.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://od.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gk.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ju.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://ad.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://mb.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ad.hahajie.cn

Go:   json.Marshal(obj)
来源：http://so.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mb.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jz.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://ap.colortex.cn

Py:   json.loads(s)
来源：http://uz.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dp.nszjky.cn

JS:   JSON.parse(s)
来源：http://nr.asd995.cn

TS:   JSON.parse(s)
来源：http://ba.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ot.huanxung.cn

Go:   json.Unmarshal(data, &v)
来源：http://hr.huixiangedu.cn

Ruby: JSON.parse(s)
来源：http://wt.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cf.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://bl.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hr.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eu.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nj.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yh.lnxyls.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vc.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vp.bookmarksfly.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mk.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jj.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://xh.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pg.yuntaijiaju.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xi.hahajie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kz.yuexingan06.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kr.yuntaijiaju.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://su.jctech888.com.cn


<!-- 参考信息 -->