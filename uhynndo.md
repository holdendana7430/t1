代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sb.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wy.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://mw.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fk.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://un.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xy.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://sx.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ki.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://pm.shxzukj.cn

JS:   Object.entries(obj)
来源：http://db.nicolike.cn

TS:   Object.entries(obj)
来源：http://hd.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://en.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xh.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://lr.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://ov.nszjky.cn

================================================================================
来源：http://in.muxihuayi.cn

H. 异常与错误处理
来源：http://yw.hnjuh.cn

================================================================================
来源：http://xo.shxzskj.cn

[H01] try / catch 基础
来源：http://rh.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oi.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ha.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wb.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ak.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fe.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ex.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hr.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xz.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://oc.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cm.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ck.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qr.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ry.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hr.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://li.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://it.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wu.shtwfgs.cn

[H03] 主动抛出异常
来源：http://ly.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://gp.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rq.colortex.cn

JS:   throw new Error("错误信息");
来源：http://pv.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://ls.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ji.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zw.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://os.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gi.huixiangedu.cn

[H04] 自定义异常类型
来源：http://nl.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://gt.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fm.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://zf.colortex.cn

TS:   class MyError extends Error {}
来源：http://kx.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://vg.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sq.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://jy.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://fy.szsharing.cn

[H05] 捕获特定类型
来源：http://ua.bjjhwx.cn

Py:   except ValueError as e:
来源：http://ln.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kq.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://om.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://ua.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://mn.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fz.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://ye.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fy.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://er.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://dg.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kc.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yw.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cm.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lp.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ku.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://tl.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://kt.nicolike.cn

[H07] 断言
来源：http://ek.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://yx.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://rg.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://ei.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://zr.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://yj.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kp.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://up.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://np.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://yn.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://gk.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ti.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://gn.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ql.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gh.yuexingan06.cn

Go:   err.Error()
来源：http://rt.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://my.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://xb.nicolike.cn

[H09] 带错误码的异常
来源：http://gn.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xm.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fx.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ad.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ns.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://av.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gm.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yn.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jp.szxytkj.cn

[H10] 资源自动释放
来源：http://ev.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dg.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jv.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wg.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eh.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yj.hahajie.cn

Go:   defer f.Close()
来源：http://uj.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://en.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bd.asd995.cn

================================================================================
来源：http://nf.bookmarksfly.cn

I. 正则表达式
来源：http://sz.panjiajie.cn

================================================================================
来源：http://mg.haigaiapp.cn

[I01] 判断是否匹配
来源：http://wv.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wp.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aa.521024.cn

JS:   /\d+/.test(s)
来源：http://vi.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://rh.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yp.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hm.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://cb.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://am.szsharing.cn

[I02] 提取所有匹配
来源：http://tf.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://rf.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pl.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sf.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://gi.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tc.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wn.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://wz.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yx.muxihuayi.cn

[I03] 提取捕获分组
来源：http://mb.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tz.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wl.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vl.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xm.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kl.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vn.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ja.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jb.gzmigu.cn

[I04] 正则替换
来源：http://px.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jm.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uw.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jx.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://od.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ox.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ww.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hk.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ne.bjjhwx.cn

[I05] 按正则拆分
来源：http://tl.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qm.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mw.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://dz.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ot.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://fk.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://og.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rn.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cr.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://md.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pd.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sj.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gb.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fc.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vh.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qi.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rn.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kj.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://gn.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vr.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dg.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ls.shxzukj.cn

TS:   /error/gim
来源：http://rq.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://up.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yh.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://du.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ai.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://gf.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gt.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lp.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ng.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uh.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hm.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bn.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ri.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lx.chemitech.net.cn

================================================================================
来源：http://ev.hahajie.cn

J. 日期与时间
来源：http://ll.asd995.cn

================================================================================
来源：http://zu.chemitech.net.cn

[J01] 获取当前时间
来源：http://ox.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kn.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yi.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://lo.huanxung.cn

TS:   new Date();  Date.now()
来源：http://hf.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://go.9csxet.cn

Go:   time.Now()
来源：http://qr.jianghongdianzi.cn

Ruby: Time.now
来源：http://ts.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hl.szsharing.cn

[J02] 格式化输出
来源：http://fp.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nl.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dw.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bw.shxzukj.cn

TS:   d.toISOString()
来源：http://gp.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qj.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uq.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://io.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vh.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://yz.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ds.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://og.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://pb.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://wx.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jr.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qy.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://eb.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cb.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://xw.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ig.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gd.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yt.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iu.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nw.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ay.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dw.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sz.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://qm.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://lv.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tz.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://km.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sm.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://gm.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eq.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://lq.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qq.9csxet.cn

[J06] 计算两时间之差
来源：http://as.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://wr.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://qs.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cr.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xw.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ny.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://fu.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://di.521024.cn

C#:   (end - start).TotalSeconds
来源：http://jh.lnxyls.cn

[J07] 比较两个日期
来源：http://gq.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://xr.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nz.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wk.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lo.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fe.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ta.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zz.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://jz.shxzukj.cn

[J08] 提取年月日与星期
来源：http://rq.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ws.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pv.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kl.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eb.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lj.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fg.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jy.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bg.jianghongdianzi.cn

[J09] 时区处理
来源：http://cs.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cc.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hm.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ry.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fl.chemitech.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://no.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gi.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hk.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ko.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://xf.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wp.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nw.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hl.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://af.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fb.asd995.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yb.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://us.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wg.szsharing.cn

================================================================================
来源：http://go.yuntaijiaju.cn

K. JSON 与序列化
来源：http://uf.nszjky.cn

================================================================================
来源：http://ih.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ne.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hp.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ai.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://qb.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://ms.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qi.bjjhwx.cn

Go:   json.Marshal(obj)
来源：http://zn.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xl.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ev.nicolike.cn

[K02] JSON 字符串转对象
来源：http://ls.yuexingan06.cn

Py:   json.loads(s)
来源：http://oo.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jg.chemitech.net.cn

JS:   JSON.parse(s)
来源：http://vb.colortex.cn

TS:   JSON.parse(s)
来源：http://ni.chemitech.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zr.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://nf.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://yz.521024.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ad.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://ak.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://br.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oz.huanxung.cn


<!-- 参考信息 -->