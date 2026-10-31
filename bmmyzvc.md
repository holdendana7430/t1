代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://yx.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://al.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://mf.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yo.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://yp.hnjuh.cn

JS:   Object.entries(obj)
来源：http://bq.521024.cn

TS:   Object.entries(obj)
来源：http://on.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ny.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hj.lnxyls.cn

Ruby: obj.instance_variables
来源：http://zv.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://pa.lnxyls.cn

================================================================================
来源：http://gs.huixinmuqiang.cn

H. 异常与错误处理
来源：http://bp.hahajie.cn

================================================================================
来源：http://pt.gzmigu.cn

[H01] try / catch 基础
来源：http://tr.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://as.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kt.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zc.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://av.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yl.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qi.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oz.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pk.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://le.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vo.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lh.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uu.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ru.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qx.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sj.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vd.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zo.jctech888.com.cn

[H03] 主动抛出异常
来源：http://wk.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://ga.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hy.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://wn.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://js.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mk.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://az.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ru.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ep.shxzskj.cn

[H04] 自定义异常类型
来源：http://da.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://lo.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kt.nszjky.cn

JS:   class MyError extends Error {}
来源：http://ns.szsharing.cn

TS:   class MyError extends Error {}
来源：http://tj.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://vw.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vi.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://bx.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://jg.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://rf.hahajie.cn

Py:   except ValueError as e:
来源：http://yb.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fj.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://nh.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://gs.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://mj.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://it.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://xp.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yq.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://xc.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://bc.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ye.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bd.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ds.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://la.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uo.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://ij.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://am.hnjuh.cn

[H07] 断言
来源：http://rz.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://cz.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://sv.huanxung.cn

JS:   console.assert(x > 0);
来源：http://ot.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://yu.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://tx.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hj.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zi.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://jx.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://mx.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://si.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zd.szxytkj.cn

JS:   e.message;  e.stack
来源：http://ke.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kz.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fy.gzmigu.cn

Go:   err.Error()
来源：http://wu.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://oh.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://gd.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://fz.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yc.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zw.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vw.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ma.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pi.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bw.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jm.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uc.jctech888.com.cn

[H10] 资源自动释放
来源：http://oz.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ot.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qe.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sr.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cx.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vk.szxytkj.cn

Go:   defer f.Close()
来源：http://gn.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sb.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ui.huixiangedu.cn

================================================================================
来源：http://oj.nicolike.cn

I. 正则表达式
来源：http://tc.jianghongdianzi.cn

================================================================================
来源：http://of.nicolike.cn

[I01] 判断是否匹配
来源：http://gh.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cq.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://te.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://ey.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://tk.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://th.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kf.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://qq.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bq.9csxet.cn

[I02] 提取所有匹配
来源：http://ym.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://cc.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://by.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aw.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://it.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zl.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qy.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://ut.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ug.colortex.cn

[I03] 提取捕获分组
来源：http://kv.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xs.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ij.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jy.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eh.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cu.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ed.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fm.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cp.nicolike.cn

[I04] 正则替换
来源：http://ib.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hi.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://na.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://az.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lc.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cd.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rc.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kt.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ai.muxihuayi.cn

[I05] 按正则拆分
来源：http://bn.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tg.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tj.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://qj.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://lt.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://zg.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vr.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yk.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qb.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://em.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vx.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ly.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uy.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ef.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cu.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fj.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sg.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ij.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://jp.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rg.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jg.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bw.gzmigu.cn

TS:   /error/gim
来源：http://kd.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bo.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qq.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://md.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qd.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://mg.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vb.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wa.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ru.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vk.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sl.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vd.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kw.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vb.szsharing.cn

================================================================================
来源：http://ot.huixinmuqiang.cn

J. 日期与时间
来源：http://dy.szsharing.cn

================================================================================
来源：http://kw.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://je.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hd.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zo.hahajie.cn

JS:   new Date();  Date.now()
来源：http://nr.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://pe.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ru.hnjuh.cn

Go:   time.Now()
来源：http://zf.shxzukj.cn

Ruby: Time.now
来源：http://tm.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://by.9csxet.cn

[J02] 格式化输出
来源：http://dl.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ww.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iw.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ol.yuexingan06.cn

TS:   d.toISOString()
来源：http://lj.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qu.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lg.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jk.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://en.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://ar.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bp.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rq.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://hr.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://xo.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nk.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hn.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://sg.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ps.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://vb.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jv.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://il.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fi.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tq.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rc.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://af.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wk.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hn.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://qj.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://pr.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ga.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ov.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://is.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://au.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iu.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://nf.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mp.wgjwhj.cn

[J06] 计算两时间之差
来源：http://pb.asd995.cn

Py:   (end - start).total_seconds()
来源：http://zt.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://ho.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vq.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hq.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xa.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://ha.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://tv.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://pv.hahajie.cn

[J07] 比较两个日期
来源：http://pg.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://oq.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://in.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wo.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zy.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://se.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qb.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fc.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ny.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://yc.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rt.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yp.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nv.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yx.huanxung.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bl.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ej.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zv.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hv.szxytkj.cn

[J09] 时区处理
来源：http://lj.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cr.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nx.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ag.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tw.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tc.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://el.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vo.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nf.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://qz.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rg.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fr.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ui.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sf.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zq.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pi.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ks.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wn.yuntaijiaju.cn

================================================================================
来源：http://uo.bjjhwx.cn

K. JSON 与序列化
来源：http://cv.yuexingan06.cn

================================================================================
来源：http://ko.huixiangedu.cn

[K01] 对象转 JSON 字符串
来源：http://tg.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tl.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qr.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://yx.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ls.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xz.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://sd.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pf.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://va.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://gz.huanxung.cn

Py:   json.loads(s)
来源：http://gd.panjiajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cr.gzmigu.cn

JS:   JSON.parse(s)
来源：http://ko.nicolike.cn

TS:   JSON.parse(s)
来源：http://hm.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ny.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://uh.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://qy.bookmarksfly.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oe.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://hf.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://al.muxihuayi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hj.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mo.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bt.szxytkj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wa.nicolike.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ev.szxytkj.cn


<!-- 参考信息 -->