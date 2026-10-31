代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://ta.hahajie.cn

Ruby: obj.instance_variables
来源：http://nt.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://ma.hnjuh.cn

================================================================================
来源：http://br.bjjhwx.cn

H. 异常与错误处理
来源：http://mh.9csxet.cn

================================================================================
来源：http://mv.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://rb.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kp.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qy.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zj.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://do.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yk.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gw.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sw.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lk.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://jr.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://do.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tr.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kh.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vu.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tp.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://va.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qe.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xt.muxihuayi.cn

[H03] 主动抛出异常
来源：http://xn.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://zk.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jw.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://cr.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://oi.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sh.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oy.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vo.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hk.lnxyls.cn

[H04] 自定义异常类型
来源：http://mb.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://td.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ub.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://fk.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://wr.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://cf.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bj.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://zk.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://mw.hahajie.cn

[H05] 捕获特定类型
来源：http://lf.asd995.cn

Py:   except ValueError as e:
来源：http://pe.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qx.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://ns.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://hn.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://uu.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ww.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://hi.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oz.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://ev.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://tv.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://du.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wp.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ku.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://om.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gv.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://rp.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://zr.bookmarksfly.cn

[H07] 断言
来源：http://wt.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://rl.asd995.cn

PHP:  assert($x > 0);
来源：http://sy.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://ig.521024.cn

TS:   console.assert(x > 0);
来源：http://os.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://tw.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dk.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xz.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://uc.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://bp.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://pc.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ub.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://aw.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://to.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://or.szsharing.cn

Go:   err.Error()
来源：http://rc.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://an.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://mk.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://mh.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jq.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lj.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ok.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tx.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rq.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://td.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fy.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ts.szsharing.cn

[H10] 资源自动释放
来源：http://le.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://os.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ew.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vm.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jt.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tc.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://je.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vw.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jy.asd995.cn

================================================================================
来源：http://gv.jctech888.com.cn

I. 正则表达式
来源：http://jg.szsharing.cn

================================================================================
来源：http://lu.huixiangedu.cn

[I01] 判断是否匹配
来源：http://yy.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ob.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ye.asd995.cn

JS:   /\d+/.test(s)
来源：http://ht.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://hg.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fx.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ov.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://ny.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nl.szsharing.cn

[I02] 提取所有匹配
来源：http://kw.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://qh.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sw.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://df.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://up.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vz.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oj.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://mv.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zz.huanxung.cn

[I03] 提取捕获分组
来源：http://in.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://in.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tl.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lm.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ld.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yy.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ws.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rj.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qa.nicolike.cn

[I04] 正则替换
来源：http://um.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ii.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bt.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://av.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sx.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zs.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qp.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rg.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kt.nszjky.cn

[I05] 按正则拆分
来源：http://eg.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ej.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nr.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://le.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://fq.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://yn.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yc.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ls.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vz.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mb.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zg.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lh.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lj.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hi.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tn.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://db.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nr.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rn.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://mb.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nl.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wy.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xx.muxihuayi.cn

TS:   /error/gim
来源：http://br.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wy.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bi.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://cg.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cz.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://if.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ld.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pl.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ix.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gk.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ha.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jt.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rn.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fa.hnjuh.cn

================================================================================
来源：http://ir.szsharing.cn

J. 日期与时间
来源：http://zi.szxytkj.cn

================================================================================
来源：http://xb.hahajie.cn

[J01] 获取当前时间
来源：http://mq.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iu.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jq.huanxung.cn

JS:   new Date();  Date.now()
来源：http://bn.huanxung.cn

TS:   new Date();  Date.now()
来源：http://sq.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cp.shtwfgs.cn

Go:   time.Now()
来源：http://vw.huanxung.cn

Ruby: Time.now
来源：http://wn.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xx.huixinmuqiang.cn

[J02] 格式化输出
来源：http://qq.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bd.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tx.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zp.521024.cn

TS:   d.toISOString()
来源：http://qc.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vu.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wl.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cg.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ue.szxytkj.cn

[J03] 字符串解析为日期
来源：http://md.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cl.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iz.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://wj.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://ju.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cb.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uk.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ma.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rm.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://sq.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gb.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ku.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tn.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ty.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ys.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xd.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ts.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zi.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://at.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://gp.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://an.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kc.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zc.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://nb.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fp.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://ik.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hj.huixiangedu.cn

[J06] 计算两时间之差
来源：http://ha.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://ep.521024.cn

PHP:  $end->diff($start)->days;
来源：http://ik.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eq.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zk.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ci.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://xr.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://td.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://aa.lnxyls.cn

[J07] 比较两个日期
来源：http://ou.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://qr.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wf.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ny.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yv.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bo.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ao.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ea.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://up.lnxyls.cn

[J08] 提取年月日与星期
来源：http://oq.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ch.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cw.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zt.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wg.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fa.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kb.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ii.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nk.hahajie.cn

[J09] 时区处理
来源：http://wr.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gv.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ha.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://on.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kw.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hs.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tw.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://md.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bl.521024.cn

[J10] 取今天 / 本月第一天
来源：http://uh.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fr.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pw.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://is.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aj.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ok.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ax.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jl.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uw.muxihuayi.cn

================================================================================
来源：http://ew.jctech888.com.cn

K. JSON 与序列化
来源：http://dm.yuexingan06.cn

================================================================================
来源：http://fo.hnjuh.cn

[K01] 对象转 JSON 字符串
来源：http://rz.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cq.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jm.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://ru.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://wq.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qi.9csxet.cn

Go:   json.Marshal(obj)
来源：http://se.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ts.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xn.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://fd.lnxyls.cn

Py:   json.loads(s)
来源：http://oj.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xv.nicolike.cn

JS:   JSON.parse(s)
来源：http://pz.lnxyls.cn

TS:   JSON.parse(s)
来源：http://zi.colortex.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fe.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://gi.colortex.cn

Ruby: JSON.parse(s)
来源：http://qp.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pj.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://lo.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ln.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qs.newstarts.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zf.9csxet.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lq.nszjky.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gv.shxzskj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lr.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sx.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://so.shxzskj.cn

[K04] 读取 JSON 文件
来源：http://km.huixiangedu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jx.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yn.shxzskj.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oo.jianghongdianzi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rs.muxihuayi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rs.newstarts.cn


<!-- 参考信息 -->