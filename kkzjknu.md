代发 wailian999

PHP:  get_object_vars($obj);
来源：http://az.gzmigu.cn

JS:   Object.entries(obj)
来源：http://vo.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://tj.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pu.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bs.9csxet.cn

Ruby: obj.instance_variables
来源：http://im.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://ly.jctech888.com.cn

================================================================================
来源：http://zf.9csxet.cn

H. 异常与错误处理
来源：http://kz.lnxyls.cn

================================================================================
来源：http://df.shxzskj.cn

[H01] try / catch 基础
来源：http://qg.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ys.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zo.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mr.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dn.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uh.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zu.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rl.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dr.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://rg.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vs.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bz.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cs.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yk.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://un.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yy.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hc.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kh.huixiangedu.cn

[H03] 主动抛出异常
来源：http://tv.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://vv.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dt.asd995.cn

JS:   throw new Error("错误信息");
来源：http://dn.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://ru.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yv.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pm.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qd.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gz.521024.cn

[H04] 自定义异常类型
来源：http://dn.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://uh.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pz.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://ni.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://ui.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://qz.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ex.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://hs.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://jk.nszjky.cn

[H05] 捕获特定类型
来源：http://xg.shxzukj.cn

Py:   except ValueError as e:
来源：http://jg.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mk.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://lp.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://zb.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://rs.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vm.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://zr.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zc.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://pm.asd995.cn

Py:   value = d.get("k") or default
来源：http://lt.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ae.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hk.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://es.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sg.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ie.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://he.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://es.yuexingan06.cn

[H07] 断言
来源：http://ep.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://na.521024.cn

PHP:  assert($x > 0);
来源：http://iy.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://zi.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://iv.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://hv.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://br.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xk.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://kf.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://rj.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://im.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lh.shxzskj.cn

JS:   e.message;  e.stack
来源：http://rw.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yv.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ng.lnxyls.cn

Go:   err.Error()
来源：http://tg.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://qm.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://pp.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://wm.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kh.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qr.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ns.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cc.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pi.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gg.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xf.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qd.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://td.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hq.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://up.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ot.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yr.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://os.gzmigu.cn

Go:   defer f.Close()
来源：http://vi.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pu.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jm.haigaiapp.cn

================================================================================
来源：http://uv.asd995.cn

I. 正则表达式
来源：http://jy.bookmarksfly.cn

================================================================================
来源：http://ck.chemitech.net.cn

[I01] 判断是否匹配
来源：http://zb.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ix.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jf.nszjky.cn

JS:   /\d+/.test(s)
来源：http://vq.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://wx.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rw.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qk.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://pa.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rf.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ul.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://gp.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uq.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cd.asd995.cn

TS:   s.match(/\d+/g)
来源：http://ri.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yg.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wc.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://fq.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://df.521024.cn

[I03] 提取捕获分组
来源：http://fc.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://um.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cv.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aa.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jn.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wy.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ns.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ii.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mx.szxytkj.cn

[I04] 正则替换
来源：http://pc.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://it.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zy.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gv.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vo.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bn.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lb.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dl.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ym.nszjky.cn

[I05] 按正则拆分
来源：http://zx.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://op.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gy.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://zy.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://xj.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://fs.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xz.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ie.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://js.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ro.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ru.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://je.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ew.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vr.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jf.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rh.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lp.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sx.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://yu.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cj.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zv.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://va.521024.cn

TS:   /error/gim
来源：http://fh.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ln.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kx.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://nj.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ds.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://ay.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vu.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fb.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gy.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tm.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gj.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zo.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ja.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ph.lnxyls.cn

================================================================================
来源：http://uw.hahajie.cn

J. 日期与时间
来源：http://mj.haigaiapp.cn

================================================================================
来源：http://ss.lnxyls.cn

[J01] 获取当前时间
来源：http://um.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ea.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://na.521024.cn

JS:   new Date();  Date.now()
来源：http://nv.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://bk.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dk.hahajie.cn

Go:   time.Now()
来源：http://ms.muxihuayi.cn

Ruby: Time.now
来源：http://hv.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qb.hahajie.cn

[J02] 格式化输出
来源：http://ue.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qz.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pg.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yr.shxzukj.cn

TS:   d.toISOString()
来源：http://oa.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://am.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://og.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kz.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://md.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://qo.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gb.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cj.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ye.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://yy.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ww.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ku.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://nc.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uh.9csxet.cn

[J04] 时间戳与日期互转
来源：http://ft.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pr.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vs.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fi.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://me.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ha.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xy.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fn.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yq.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://uz.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://nq.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wc.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hg.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ns.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://yu.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vu.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://pa.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rb.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://lq.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://jz.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://qp.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mj.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ej.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pt.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://vk.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://kl.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://zs.lnxyls.cn

[J07] 比较两个日期
来源：http://sx.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://rj.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ll.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sp.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jr.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pm.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gk.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://to.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://la.asd995.cn

[J08] 提取年月日与星期
来源：http://pl.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://at.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gf.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ww.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ka.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ci.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yz.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fu.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vx.huixinmuqiang.cn

[J09] 时区处理
来源：http://uk.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hq.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ra.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gd.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://um.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kl.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zk.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://og.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jt.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://sw.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oz.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wu.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aj.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rx.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zj.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jo.szxytkj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vu.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zc.muxihuayi.cn

================================================================================
来源：http://qr.9csxet.cn

K. JSON 与序列化
来源：http://tl.szxytkj.cn

================================================================================
来源：http://lx.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://bs.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sm.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hp.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://wv.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://rt.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yv.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://ps.chemitech.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ba.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dv.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ib.521024.cn

Py:   json.loads(s)
来源：http://br.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jl.nszjky.cn

JS:   JSON.parse(s)
来源：http://nw.newstarts.cn

TS:   JSON.parse(s)
来源：http://ib.szxytkj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uz.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://em.huanxung.cn

Ruby: JSON.parse(s)
来源：http://gq.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sl.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://tn.shxzskj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kj.shxzskj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vd.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://km.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://in.chemitech.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://he.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sg.nszjky.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ls.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bz.muxihuayi.cn

[K04] 读取 JSON 文件
来源：http://ar.panjiajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tw.jctech888.com.cn


<!-- 参考信息 -->