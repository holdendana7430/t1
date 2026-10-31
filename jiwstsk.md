代发 wailian999

PHP:  get_object_vars($obj);
来源：http://wt.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://fx.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://oo.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bp.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pe.newstarts.cn

Ruby: obj.instance_variables
来源：http://bd.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://rj.nicolike.cn

================================================================================
来源：http://kn.newstarts.cn

H. 异常与错误处理
来源：http://mo.shxzukj.cn

================================================================================
来源：http://os.gzmigu.cn

[H01] try / catch 基础
来源：http://ut.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://er.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ta.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jz.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fr.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ew.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ek.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dz.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yc.521024.cn

[H02] finally / ensure 收尾
来源：http://gw.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mj.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eq.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ko.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hk.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lv.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pp.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ol.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yu.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://wn.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://di.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yz.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://to.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://jg.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qa.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uj.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dw.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bp.muxihuayi.cn

[H04] 自定义异常类型
来源：http://jn.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://dw.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vg.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://jb.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://en.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://py.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uu.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://iq.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://yj.asd995.cn

[H05] 捕获特定类型
来源：http://es.nszjky.cn

Py:   except ValueError as e:
来源：http://td.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xg.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://rw.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://fk.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://ni.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://le.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://up.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vy.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://ed.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://ve.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wn.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lh.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wd.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ix.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xk.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://cp.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://yr.asd995.cn

[H07] 断言
来源：http://fs.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://zh.hahajie.cn

PHP:  assert($x > 0);
来源：http://qu.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://rv.szsharing.cn

TS:   console.assert(x > 0);
来源：http://pq.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://hy.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sx.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://by.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://cw.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://nn.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://xn.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pb.szxytkj.cn

JS:   e.message;  e.stack
来源：http://tq.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jn.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lq.wgjwhj.cn

Go:   err.Error()
来源：http://kj.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://rh.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ql.panjiajie.cn

[H09] 带错误码的异常
来源：http://ym.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ez.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qi.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oa.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eu.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jq.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cv.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://re.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ab.szsharing.cn

[H10] 资源自动释放
来源：http://hf.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dh.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sx.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://se.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rt.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ti.szsharing.cn

Go:   defer f.Close()
来源：http://wl.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://me.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zy.huixiangedu.cn

================================================================================
来源：http://im.huanxung.cn

I. 正则表达式
来源：http://il.szsharing.cn

================================================================================
来源：http://zp.asd995.cn

[I01] 判断是否匹配
来源：http://yr.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://px.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eq.9csxet.cn

JS:   /\d+/.test(s)
来源：http://la.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://lt.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xr.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dk.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://jt.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qe.colortex.cn

[I02] 提取所有匹配
来源：http://dn.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://em.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qk.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hm.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://ft.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hp.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://at.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://ax.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gj.shxzskj.cn

[I03] 提取捕获分组
来源：http://kj.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ri.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sa.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://my.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wg.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pj.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tg.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://py.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uc.colortex.cn

[I04] 正则替换
来源：http://na.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mv.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://th.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ws.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wc.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hz.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ch.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://al.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zm.521024.cn

[I05] 按正则拆分
来源：http://si.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bc.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oy.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://xf.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://yy.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://kg.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wz.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sr.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iu.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uj.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vq.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xf.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bf.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hf.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fe.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zc.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nd.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tr.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://fm.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oc.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kw.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://to.nszjky.cn

TS:   /error/gim
来源：http://bc.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bt.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ir.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://lx.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hb.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://rm.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tz.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xu.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rt.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cb.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lt.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cx.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tw.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bg.521024.cn

================================================================================
来源：http://vd.panjiajie.cn

J. 日期与时间
来源：http://bo.huanxung.cn

================================================================================
来源：http://gs.nszjky.cn

[J01] 获取当前时间
来源：http://xg.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nl.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nr.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://ec.nszjky.cn

TS:   new Date();  Date.now()
来源：http://kc.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ra.asd995.cn

Go:   time.Now()
来源：http://nl.newstarts.cn

Ruby: Time.now
来源：http://xt.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fv.521024.cn

[J02] 格式化输出
来源：http://lb.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://na.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jr.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dw.yuexingan06.cn

TS:   d.toISOString()
来源：http://iq.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vt.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://to.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tv.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mb.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://os.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ph.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://za.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://cb.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://vq.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kn.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xg.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://xx.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qu.nszjky.cn

[J04] 时间戳与日期互转
来源：http://kt.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ql.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qt.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bt.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ej.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://df.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vb.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wf.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fv.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://oh.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://ka.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qh.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jr.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kv.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://rn.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iu.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://ga.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dg.jctech888.com.cn

[J06] 计算两时间之差
来源：http://om.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://ic.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://lp.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://me.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ki.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://et.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://jl.lnxyls.cn

Ruby: end - start                 # 返回秒数
来源：http://zq.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://gq.newstarts.cn

[J07] 比较两个日期
来源：http://rg.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://mc.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vz.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uf.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dc.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pz.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ue.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://np.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://we.szxytkj.cn

[J08] 提取年月日与星期
来源：http://hd.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yi.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hn.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hu.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zr.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://el.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zb.bookmarksfly.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uc.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ka.yuexingan06.cn

[J09] 时区处理
来源：http://je.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mp.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zx.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wl.wgjwhj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xj.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ob.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vr.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aj.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vx.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://zc.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ph.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jg.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nh.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xf.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ax.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vi.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pg.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ko.bookmarksfly.cn

================================================================================
来源：http://jc.521024.cn

K. JSON 与序列化
来源：http://sk.szsharing.cn

================================================================================
来源：http://rj.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://db.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rb.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xm.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://fh.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://id.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jp.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://we.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cn.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dl.huixiangedu.cn

[K02] JSON 字符串转对象
来源：http://fb.huanxung.cn

Py:   json.loads(s)
来源：http://cx.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hn.colortex.cn

JS:   JSON.parse(s)
来源：http://wa.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://fc.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hs.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://cs.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://hz.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zt.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://wd.chemitech.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uj.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vf.yuntaijiaju.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qd.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ue.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yj.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nc.wgjwhj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zs.hahajie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fu.colortex.cn

[K04] 读取 JSON 文件
来源：http://lj.shxzukj.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ou.lnxyls.cn


<!-- 参考信息 -->