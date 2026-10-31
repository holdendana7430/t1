代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hq.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fc.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://gr.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fz.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://wc.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://vm.nicolike.cn

TS:   Object.entries(obj)
来源：http://wx.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ro.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hr.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://ov.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://zl.asd995.cn

================================================================================
来源：http://uf.nicolike.cn

H. 异常与错误处理
来源：http://qg.colortex.cn

================================================================================
来源：http://bi.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://iq.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://in.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dz.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vy.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wl.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wi.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tz.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vw.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gu.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://tb.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rv.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cr.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yz.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tx.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bf.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jw.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://at.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tz.szxytkj.cn

[H03] 主动抛出异常
来源：http://sw.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://ph.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lg.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://sr.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://vz.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ad.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qk.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tq.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://br.nicolike.cn

[H04] 自定义异常类型
来源：http://pm.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://ub.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://du.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://yc.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://gx.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ha.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xd.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://wi.9csxet.cn

C#:   class MyException : Exception {}
来源：http://lq.wgjwhj.cn

[H05] 捕获特定类型
来源：http://ue.521024.cn

Py:   except ValueError as e:
来源：http://wg.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hx.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://hs.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://ho.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://jg.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fs.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://wv.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ic.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://zn.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://zp.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qt.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yu.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pu.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://js.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iu.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://gg.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://qu.shxzskj.cn

[H07] 断言
来源：http://bz.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://vc.nicolike.cn

PHP:  assert($x > 0);
来源：http://pa.colortex.cn

JS:   console.assert(x > 0);
来源：http://wg.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://ij.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://fl.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ie.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mj.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://yh.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://nj.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://vv.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qd.hnjuh.cn

JS:   e.message;  e.stack
来源：http://cn.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ew.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://im.szsharing.cn

Go:   err.Error()
来源：http://hc.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://pe.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://yk.521024.cn

[H09] 带错误码的异常
来源：http://tq.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hc.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hd.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fs.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xo.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aq.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lo.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ap.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oi.9csxet.cn

[H10] 资源自动释放
来源：http://aa.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ha.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bm.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fq.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jw.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ep.colortex.cn

Go:   defer f.Close()
来源：http://fd.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://me.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wc.jianghongdianzi.cn

================================================================================
来源：http://zf.muxihuayi.cn

I. 正则表达式
来源：http://he.colortex.cn

================================================================================
来源：http://ae.hahajie.cn

[I01] 判断是否匹配
来源：http://ru.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mb.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ov.newstarts.cn

JS:   /\d+/.test(s)
来源：http://vk.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://by.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jn.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://us.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://kz.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mk.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ue.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://ud.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jq.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zb.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://fj.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://me.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lr.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://ew.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fa.szxytkj.cn

[I03] 提取捕获分组
来源：http://mj.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://th.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://co.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pp.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nr.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sf.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yc.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oi.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://de.szxytkj.cn

[I04] 正则替换
来源：http://zf.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ar.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dr.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://we.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ij.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xi.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ts.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jz.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://km.bjjhwx.cn

[I05] 按正则拆分
来源：http://ev.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://je.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tk.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://lf.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://re.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://ou.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pt.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iz.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sg.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uy.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://md.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jy.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vy.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lq.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ui.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ws.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rv.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jj.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://cp.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gx.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jm.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lf.jianghongdianzi.cn

TS:   /error/gim
来源：http://tb.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ot.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cy.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://oc.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ov.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://uf.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://op.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sx.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vn.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vm.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dj.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ru.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dy.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ao.szxytkj.cn

================================================================================
来源：http://if.bookmarksfly.cn

J. 日期与时间
来源：http://wm.muxihuayi.cn

================================================================================
来源：http://qq.panjiajie.cn

[J01] 获取当前时间
来源：http://ao.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gy.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qj.newstarts.cn

JS:   new Date();  Date.now()
来源：http://zd.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://gk.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jz.nszjky.cn

Go:   time.Now()
来源：http://tf.muxihuayi.cn

Ruby: Time.now
来源：http://vg.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nw.jctech888.com.cn

[J02] 格式化输出
来源：http://gq.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zd.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qr.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pf.newstarts.cn

TS:   d.toISOString()
来源：http://vu.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ie.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wh.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rn.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xx.521024.cn

[J03] 字符串解析为日期
来源：http://wc.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ss.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vv.521024.cn

JS:   new Date("2024-01-02")
来源：http://qx.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://dv.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dv.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eg.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://lx.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://if.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://yy.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jv.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tg.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vl.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qz.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bf.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tf.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ge.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ru.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://mm.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://kj.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ou.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://un.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vk.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ok.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yw.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://me.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wn.shxzskj.cn

[J06] 计算两时间之差
来源：http://zq.colortex.cn

Py:   (end - start).total_seconds()
来源：http://ix.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://em.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xc.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vw.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mj.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://xn.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://nf.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://sd.huanxung.cn

[J07] 比较两个日期
来源：http://yp.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://sj.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aj.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://se.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://id.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tk.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hy.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yt.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://fq.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://zy.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ld.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yu.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://af.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cm.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ie.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wa.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hb.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lp.bookmarksfly.cn

[J09] 时区处理
来源：http://dm.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gx.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jp.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xi.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yx.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kp.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://au.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oa.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://um.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xu.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nb.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://se.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ve.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gk.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gf.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jc.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sj.nicolike.cn

================================================================================
来源：http://yn.muxihuayi.cn

K. JSON 与序列化
来源：http://cv.bjjhwx.cn

================================================================================
来源：http://if.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://pv.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jd.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://th.chemitech.net.cn

JS:   JSON.stringify(obj)
来源：http://gj.huixinmuqiang.cn

TS:   JSON.stringify(obj)
来源：http://il.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lr.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://at.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ok.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ib.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://mu.huixiangedu.cn

Py:   json.loads(s)
来源：http://op.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ep.nszjky.cn

JS:   JSON.parse(s)
来源：http://jw.szxytkj.cn

TS:   JSON.parse(s)
来源：http://qk.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pt.9csxet.cn

Go:   json.Unmarshal(data, &v)
来源：http://tv.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://bu.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oa.asd995.cn

[K03] JSON 美化输出（带缩进）
来源：http://mx.bookmarksfly.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rx.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zw.wgjwhj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ad.hnjuh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yj.muxihuayi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kd.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ak.nicolike.cn


<!-- 参考信息 -->