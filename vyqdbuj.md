代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://pl.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vr.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://gd.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yx.asd995.cn

PHP:  get_object_vars($obj);
来源：http://xt.hnjuh.cn

JS:   Object.entries(obj)
来源：http://fp.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://up.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://av.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://au.521024.cn

Ruby: obj.instance_variables
来源：http://bg.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://jw.colortex.cn

================================================================================
来源：http://cp.gzmigu.cn

H. 异常与错误处理
来源：http://ep.shxzskj.cn

================================================================================
来源：http://og.szsharing.cn

[H01] try / catch 基础
来源：http://ku.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dk.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zy.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mp.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://we.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uy.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pg.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xy.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fx.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ec.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://er.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qf.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qk.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wz.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zy.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://el.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uu.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ja.colortex.cn

[H03] 主动抛出异常
来源：http://oo.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://db.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uu.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://st.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://jj.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pd.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ny.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ib.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tc.huixiangedu.cn

[H04] 自定义异常类型
来源：http://wh.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://ja.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://un.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://dj.9csxet.cn

TS:   class MyError extends Error {}
来源：http://nt.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://ho.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cw.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://vx.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://oe.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://oe.9csxet.cn

Py:   except ValueError as e:
来源：http://wm.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gw.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://pq.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://gv.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ul.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://in.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://fa.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yx.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://yn.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://op.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iw.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fv.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rk.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zj.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ew.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://vo.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://sk.nszjky.cn

[H07] 断言
来源：http://eu.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://sb.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://mi.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://tt.huanxung.cn

TS:   console.assert(x > 0);
来源：http://uk.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://wn.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gn.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qx.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://nb.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://au.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://nw.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zj.newstarts.cn

JS:   e.message;  e.stack
来源：http://ns.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wu.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qg.shtwfgs.cn

Go:   err.Error()
来源：http://fz.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://rm.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://mm.huixiangedu.cn

[H09] 带错误码的异常
来源：http://nv.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://td.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vv.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yl.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jx.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ug.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://id.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://it.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fn.hahajie.cn

[H10] 资源自动释放
来源：http://af.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ip.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oq.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xu.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tf.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zi.haigaiapp.cn

Go:   defer f.Close()
来源：http://mw.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ch.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qv.haigaiapp.cn

================================================================================
来源：http://aw.jctech888.com.cn

I. 正则表达式
来源：http://af.muxihuayi.cn

================================================================================
来源：http://ou.nszjky.cn

[I01] 判断是否匹配
来源：http://gp.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yp.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jy.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://le.colortex.cn

TS:   /\d+/.test(s)
来源：http://cm.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fh.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fi.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://yc.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uk.521024.cn

[I02] 提取所有匹配
来源：http://sy.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://gq.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fa.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sk.521024.cn

TS:   s.match(/\d+/g)
来源：http://ly.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cm.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bq.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://vg.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gn.yuexingan06.cn

[I03] 提取捕获分组
来源：http://sz.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yq.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ik.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ww.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lg.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ur.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qu.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sw.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fw.9csxet.cn

[I04] 正则替换
来源：http://vz.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pu.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hb.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mz.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bu.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bk.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kt.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xl.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.huanxung.cn

[I05] 按正则拆分
来源：http://tv.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bt.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hq.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ez.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ph.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://dt.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bd.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sb.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sc.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fr.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mh.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jv.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://az.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cz.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fe.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vn.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cr.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pw.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://uc.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://su.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ar.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sr.newstarts.cn

TS:   /error/gim
来源：http://ug.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hi.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xz.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://fy.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yr.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://sd.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hv.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://do.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wi.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rv.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nn.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wm.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wu.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bl.hnjuh.cn

================================================================================
来源：http://ih.huixiangedu.cn

J. 日期与时间
来源：http://uh.9csxet.cn

================================================================================
来源：http://cs.lnxyls.cn

[J01] 获取当前时间
来源：http://ja.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rj.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tw.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://ln.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://qy.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jv.jctech888.com.cn

Go:   time.Now()
来源：http://pc.haigaiapp.cn

Ruby: Time.now
来源：http://kr.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gs.shxzskj.cn

[J02] 格式化输出
来源：http://ev.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dl.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ip.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nb.huixiangedu.cn

TS:   d.toISOString()
来源：http://tu.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dg.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://al.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dd.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pz.521024.cn

[J03] 字符串解析为日期
来源：http://el.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://os.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kt.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://sf.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://fv.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wi.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cx.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://zw.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kj.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://ca.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kq.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gb.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://db.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ct.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tc.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lj.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://se.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gp.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://ss.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://zz.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iu.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://id.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gd.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://qj.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ye.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://hi.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nk.hahajie.cn

[J06] 计算两时间之差
来源：http://xv.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://hw.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://ab.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oh.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://of.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kg.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://vx.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://ha.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://yr.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://vw.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://ci.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dw.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lz.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ds.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zv.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gc.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vq.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://ss.colortex.cn

[J08] 提取年月日与星期
来源：http://du.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://er.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bp.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bt.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pf.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://id.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cl.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xy.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mf.chemitech.net.cn

[J09] 时区处理
来源：http://vf.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hm.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://at.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hd.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jt.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hs.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dy.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cm.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dk.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://ih.szxytkj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gr.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eu.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mc.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sd.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qx.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bj.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bt.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://us.9csxet.cn

================================================================================
来源：http://kg.huanxung.cn

K. JSON 与序列化
来源：http://jx.shxzukj.cn

================================================================================
来源：http://hp.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://bg.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rl.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yz.hahajie.cn

JS:   JSON.stringify(obj)
来源：http://oq.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://dj.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tv.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://gz.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xf.chemitech.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lt.yuexingan06.cn

[K02] JSON 字符串转对象
来源：http://er.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://ze.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cv.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://ni.lnxyls.cn

TS:   JSON.parse(s)
来源：http://fv.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qc.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://ja.nszjky.cn

Ruby: JSON.parse(s)
来源：http://kb.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ud.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://gr.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mb.9csxet.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jk.9csxet.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gx.lnxyls.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bz.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uu.bookmarksfly.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://od.shtwfgs.cn


<!-- 参考信息 -->