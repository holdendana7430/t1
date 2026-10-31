代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zi.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://at.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://gy.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qn.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://rs.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ud.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://hw.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dj.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://eh.asd995.cn

JS:   Object.entries(obj)
来源：http://ry.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://it.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yq.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://op.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://wk.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://kv.nszjky.cn

================================================================================
来源：http://wm.huanxung.cn

H. 异常与错误处理
来源：http://pd.hnjuh.cn

================================================================================
来源：http://tx.chemitech.net.cn

[H01] try / catch 基础
来源：http://eu.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kj.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://en.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dn.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jc.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uu.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iv.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oe.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cn.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://yq.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://en.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oc.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ul.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uj.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zt.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mr.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sl.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oq.yuexingan06.cn

[H03] 主动抛出异常
来源：http://il.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://hk.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gp.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://yd.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://kp.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sp.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bn.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gj.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vm.colortex.cn

[H04] 自定义异常类型
来源：http://fn.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://vt.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pw.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://vr.colortex.cn

TS:   class MyError extends Error {}
来源：http://yo.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://dy.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sp.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://sr.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://ki.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://bw.lnxyls.cn

Py:   except ValueError as e:
来源：http://sy.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kl.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://tp.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://lw.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://nl.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dw.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://yi.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fh.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://eu.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://jj.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rx.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sc.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ay.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qo.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ea.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://lh.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://ck.shtwfgs.cn

[H07] 断言
来源：http://ov.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ne.shxzskj.cn

PHP:  assert($x > 0);
来源：http://ed.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://wf.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://xw.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://kk.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rx.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jf.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://vc.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://ry.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://yr.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hx.huanxung.cn

JS:   e.message;  e.stack
来源：http://qx.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yx.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zu.hahajie.cn

Go:   err.Error()
来源：http://nl.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://wg.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://sx.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://fo.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ni.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kr.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ft.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ra.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hx.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pc.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mn.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nz.521024.cn

[H10] 资源自动释放
来源：http://rj.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ck.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lf.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zy.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gh.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vq.nszjky.cn

Go:   defer f.Close()
来源：http://ju.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pa.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vv.wgjwhj.cn

================================================================================
来源：http://qc.jctech888.com.cn

I. 正则表达式
来源：http://xr.haigaiapp.cn

================================================================================
来源：http://jx.panjiajie.cn

[I01] 判断是否匹配
来源：http://ip.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fk.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hw.newstarts.cn

JS:   /\d+/.test(s)
来源：http://bk.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://bo.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wu.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tt.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://oi.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ai.521024.cn

[I02] 提取所有匹配
来源：http://nd.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://kb.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ww.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ox.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://oy.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qn.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lh.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://gr.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eq.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://vl.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gc.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qf.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qz.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vs.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jc.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sc.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ya.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xo.asd995.cn

[I04] 正则替换
来源：http://gk.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jj.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lj.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xy.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kf.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jw.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zy.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qz.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hw.lnxyls.cn

[I05] 按正则拆分
来源：http://pc.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xb.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dp.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://nn.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://ei.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://sq.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fk.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mu.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sc.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oc.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iz.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nv.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gi.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ff.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uu.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zb.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vx.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://em.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nx.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rg.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lo.9csxet.cn

TS:   /error/gim
来源：http://xs.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vc.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gy.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://tf.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iv.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://ro.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yf.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oy.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ij.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://am.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lv.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xc.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sg.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zq.chemitech.net.cn

================================================================================
来源：http://kq.panjiajie.cn

J. 日期与时间
来源：http://lf.bookmarksfly.cn

================================================================================
来源：http://xb.hnjuh.cn

[J01] 获取当前时间
来源：http://xx.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sr.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wt.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://ip.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://oo.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qr.huixinmuqiang.cn

Go:   time.Now()
来源：http://fr.jctech888.com.cn

Ruby: Time.now
来源：http://pk.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gw.chemitech.net.cn

[J02] 格式化输出
来源：http://zf.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eq.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ju.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ab.wgjwhj.cn

TS:   d.toISOString()
来源：http://ru.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lp.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ot.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sw.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aw.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://ni.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mx.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qx.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ia.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://ht.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jd.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ze.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://rz.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wv.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://vv.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fy.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sp.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oy.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qn.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ue.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qj.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://st.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gr.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://cj.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://hg.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xp.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://go.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yo.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://jo.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wb.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://ra.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pc.hahajie.cn

[J06] 计算两时间之差
来源：http://ya.gzmigu.cn

Py:   (end - start).total_seconds()
来源：http://bl.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://oe.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sx.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qk.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sf.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://xd.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://eq.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://ua.jctech888.com.cn

[J07] 比较两个日期
来源：http://gr.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://oq.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vp.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uh.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pq.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mp.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ak.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ew.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://cz.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://wh.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kh.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eh.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://so.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xq.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zc.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qh.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://am.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rn.bjjhwx.cn

[J09] 时区处理
来源：http://ld.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cv.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jx.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wn.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://na.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ko.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dg.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ms.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bt.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://xb.lnxyls.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iz.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nw.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xx.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jf.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hm.bookmarksfly.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cg.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nm.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ug.521024.cn

================================================================================
来源：http://ho.shxzskj.cn

K. JSON 与序列化
来源：http://th.nicolike.cn

================================================================================
来源：http://rl.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://px.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rg.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://na.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://ix.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://gp.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zy.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://hf.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eg.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qr.9csxet.cn

[K02] JSON 字符串转对象
来源：http://yg.shxzskj.cn

Py:   json.loads(s)
来源：http://qd.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xy.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://vk.szxytkj.cn

TS:   JSON.parse(s)
来源：http://qd.huixinmuqiang.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lq.bookmarksfly.cn

Go:   json.Unmarshal(data, &v)
来源：http://an.nicolike.cn

Ruby: JSON.parse(s)
来源：http://uy.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sj.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://jx.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://np.shxzukj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fk.lnxyls.cn


<!-- 参考信息 -->