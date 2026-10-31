代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://do.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ub.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://ub.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sv.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://ad.shxzukj.cn

JS:   Object.entries(obj)
来源：http://ld.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://vs.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ed.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kg.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://ij.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://ee.9csxet.cn

================================================================================
来源：http://ii.asd995.cn

H. 异常与错误处理
来源：http://xw.panjiajie.cn

================================================================================
来源：http://zf.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://qt.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ma.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pd.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://na.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://go.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xv.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zi.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ie.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://si.asd995.cn

[H02] finally / ensure 收尾
来源：http://zr.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tx.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cd.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://px.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ck.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rw.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wa.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ba.yuexingan06.cn

[H03] 主动抛出异常
来源：http://ga.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://pb.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bh.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://ed.colortex.cn

TS:   throw new Error("错误信息");
来源：http://un.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xj.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ec.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jk.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iz.hahajie.cn

[H04] 自定义异常类型
来源：http://me.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://dj.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cw.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://gm.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://nx.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://ke.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oq.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://ky.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://ye.9csxet.cn

[H05] 捕获特定类型
来源：http://cu.gzmigu.cn

Py:   except ValueError as e:
来源：http://xo.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yu.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://oj.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://af.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://sz.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://on.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://fk.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gs.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://yv.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://tl.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jk.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ci.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jx.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://md.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mk.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://kx.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://yc.nszjky.cn

[H07] 断言
来源：http://sl.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://rv.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ph.hahajie.cn

JS:   console.assert(x > 0);
来源：http://gy.9csxet.cn

TS:   console.assert(x > 0);
来源：http://hy.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://wg.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kz.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lx.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://pk.521024.cn

[H08] 获取错误信息与堆栈
来源：http://en.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://mf.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vo.hnjuh.cn

JS:   e.message;  e.stack
来源：http://aa.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cp.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lk.lnxyls.cn

Go:   err.Error()
来源：http://fo.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://hd.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://hk.chemitech.net.cn

[H09] 带错误码的异常
来源：http://gj.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ki.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vs.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ur.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hw.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ea.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nk.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sz.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pv.521024.cn

[H10] 资源自动释放
来源：http://mc.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vc.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vc.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ae.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fe.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://os.asd995.cn

Go:   defer f.Close()
来源：http://gt.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wf.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vq.wgjwhj.cn

================================================================================
来源：http://fa.shxzukj.cn

I. 正则表达式
来源：http://kz.gzmigu.cn

================================================================================
来源：http://tj.yuexingan06.cn

[I01] 判断是否匹配
来源：http://fr.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vf.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sx.hahajie.cn

JS:   /\d+/.test(s)
来源：http://sg.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://ex.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fa.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ug.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://mg.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tm.bjjhwx.cn

[I02] 提取所有匹配
来源：http://fl.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://bp.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gv.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bz.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://ja.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dn.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ry.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://qe.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fu.yuexingan06.cn

[I03] 提取捕获分组
来源：http://vo.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gy.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rg.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ew.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uw.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rq.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jm.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://er.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://je.nszjky.cn

[I04] 正则替换
来源：http://ks.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://de.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ln.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vt.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://us.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wd.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ih.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kh.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ll.asd995.cn

[I05] 按正则拆分
来源：http://ef.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aa.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://id.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ll.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://tv.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://dh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vf.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pe.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uo.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uc.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pv.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dl.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cd.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bv.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jg.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dd.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gi.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xa.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://yn.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://se.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ws.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dm.bjjhwx.cn

TS:   /error/gim
来源：http://es.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vf.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qm.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://xk.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://te.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://ku.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hk.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wf.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ur.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aj.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ib.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cq.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ob.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ss.gzmigu.cn

================================================================================
来源：http://ik.panjiajie.cn

J. 日期与时间
来源：http://qy.muxihuayi.cn

================================================================================
来源：http://pn.muxihuayi.cn

[J01] 获取当前时间
来源：http://su.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://za.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://he.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ab.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://jg.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://em.nicolike.cn

Go:   time.Now()
来源：http://tx.huixiangedu.cn

Ruby: Time.now
来源：http://mb.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bv.huixinmuqiang.cn

[J02] 格式化输出
来源：http://mc.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fb.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rb.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rw.shtwfgs.cn

TS:   d.toISOString()
来源：http://js.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://om.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bl.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mu.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dp.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://zx.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sd.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iv.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://cs.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://ib.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tk.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nr.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://wf.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cw.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://zj.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qn.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hn.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ip.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yn.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yi.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kh.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yo.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yy.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://kk.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://ea.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sg.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lo.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://al.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://wh.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yg.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://vt.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uz.colortex.cn

[J06] 计算两时间之差
来源：http://ve.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://hj.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://rf.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://af.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qi.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kd.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://ya.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://wh.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://xv.jctech888.com.cn

[J07] 比较两个日期
来源：http://bf.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://xp.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gx.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wq.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://no.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ar.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kd.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fe.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ku.gzmigu.cn

[J08] 提取年月日与星期
来源：http://yt.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tu.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mt.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eu.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uv.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://te.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://od.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lj.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://az.yuntaijiaju.cn

[J09] 时区处理
来源：http://oj.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ve.jianghongdianzi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iv.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bu.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://us.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://da.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yu.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ub.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ag.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://ok.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wg.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zt.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hp.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kv.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ly.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jl.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nx.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gq.muxihuayi.cn

================================================================================
来源：http://em.bjjhwx.cn

K. JSON 与序列化
来源：http://bb.asd995.cn

================================================================================
来源：http://dw.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://ml.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uq.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dj.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://kf.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://xr.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iv.hnjuh.cn

Go:   json.Marshal(obj)
来源：http://fe.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pf.muxihuayi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jo.jctech888.com.cn

[K02] JSON 字符串转对象
来源：http://kl.bjjhwx.cn

Py:   json.loads(s)
来源：http://wb.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rd.shxzukj.cn

JS:   JSON.parse(s)
来源：http://qf.nszjky.cn

TS:   JSON.parse(s)
来源：http://zz.muxihuayi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rr.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://sr.521024.cn

Ruby: JSON.parse(s)
来源：http://bl.nszjky.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hm.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://ij.gzmigu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ms.bjjhwx.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://po.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wm.hahajie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tl.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ap.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fj.shtwfgs.cn


<!-- 参考信息 -->