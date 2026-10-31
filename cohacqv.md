代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://yz.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mq.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://of.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yp.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://tq.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://lz.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://qg.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ed.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hw.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://kc.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://gb.colortex.cn

================================================================================
来源：http://ck.shxzukj.cn

H. 异常与错误处理
来源：http://ql.szsharing.cn

================================================================================
来源：http://wm.hnjuh.cn

[H01] try / catch 基础
来源：http://oq.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rz.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pc.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ac.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ll.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pf.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qe.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eg.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qn.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://jf.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ui.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mr.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://um.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lr.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ea.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bv.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gs.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gi.chemitech.net.cn

[H03] 主动抛出异常
来源：http://sa.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://kn.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ed.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://jw.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://uw.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dw.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ni.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fr.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rn.hahajie.cn

[H04] 自定义异常类型
来源：http://zb.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://pp.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ht.521024.cn

JS:   class MyError extends Error {}
来源：http://po.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://eb.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://zq.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ay.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://dh.szsharing.cn

C#:   class MyException : Exception {}
来源：http://fu.bjjhwx.cn

[H05] 捕获特定类型
来源：http://cq.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://tm.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zw.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ql.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://hx.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://hn.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fo.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://rv.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gt.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://zr.colortex.cn

Py:   value = d.get("k") or default
来源：http://wq.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pg.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://os.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dd.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lh.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hb.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://av.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://xt.szxytkj.cn

[H07] 断言
来源：http://aq.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://yk.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://sq.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://my.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://vc.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://oo.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://br.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dx.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ul.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://yr.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://qq.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gp.9csxet.cn

JS:   e.message;  e.stack
来源：http://kn.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vl.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yi.szsharing.cn

Go:   err.Error()
来源：http://ve.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://et.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://ep.hnjuh.cn

[H09] 带错误码的异常
来源：http://ro.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gy.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vk.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yj.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lb.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uu.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lu.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xg.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wi.szxytkj.cn

[H10] 资源自动释放
来源：http://gy.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://os.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://io.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ea.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vy.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ef.szxytkj.cn

Go:   defer f.Close()
来源：http://oq.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vp.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sq.huixinmuqiang.cn

================================================================================
来源：http://su.shxzskj.cn

I. 正则表达式
来源：http://df.nicolike.cn

================================================================================
来源：http://cj.huanxung.cn

[I01] 判断是否匹配
来源：http://tu.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tw.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xx.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://it.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://xb.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vf.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://al.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://vn.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lv.jctech888.com.cn

[I02] 提取所有匹配
来源：http://re.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://dp.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://za.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vt.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://ka.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pv.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tx.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://wa.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uj.gzmigu.cn

[I03] 提取捕获分组
来源：http://vv.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nx.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kw.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yh.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://er.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cn.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://be.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iw.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bc.hnjuh.cn

[I04] 正则替换
来源：http://lj.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ux.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iy.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nd.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dx.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uz.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kc.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gf.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gx.hahajie.cn

[I05] 按正则拆分
来源：http://km.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fr.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gs.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://ij.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://tt.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://fl.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ea.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sr.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dq.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gw.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://te.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jk.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qg.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vq.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yd.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rl.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dq.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qf.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://bs.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sr.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ma.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xm.jianghongdianzi.cn

TS:   /error/gim
来源：http://ty.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cn.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yt.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://xo.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xn.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://xd.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yn.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tx.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yd.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://in.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ql.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pe.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://te.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://po.yuntaijiaju.cn

================================================================================
来源：http://il.huanxung.cn

J. 日期与时间
来源：http://xh.asd995.cn

================================================================================
来源：http://lt.wgjwhj.cn

[J01] 获取当前时间
来源：http://xi.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xm.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://th.newstarts.cn

JS:   new Date();  Date.now()
来源：http://an.hahajie.cn

TS:   new Date();  Date.now()
来源：http://fu.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tr.nszjky.cn

Go:   time.Now()
来源：http://mg.shxzskj.cn

Ruby: Time.now
来源：http://if.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zq.gzmigu.cn

[J02] 格式化输出
来源：http://nd.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zo.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uz.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wt.szxytkj.cn

TS:   d.toISOString()
来源：http://kt.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oq.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ao.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rw.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mj.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://ty.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xv.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iz.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://sa.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://vz.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ov.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://et.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://sb.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gz.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://se.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zm.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ld.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ob.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cm.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eq.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://di.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ys.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hq.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://wr.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://gy.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zw.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ik.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aj.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://mx.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ue.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://tn.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jz.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://zh.asd995.cn

Py:   (end - start).total_seconds()
来源：http://zi.521024.cn

PHP:  $end->diff($start)->days;
来源：http://mw.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://re.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ls.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ce.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://oo.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://rs.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://zr.nszjky.cn

[J07] 比较两个日期
来源：http://dh.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ew.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pk.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sc.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mh.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xq.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zj.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kz.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://co.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://ya.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sb.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yv.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zs.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ti.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uk.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qx.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rl.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zm.shxzukj.cn

[J09] 时区处理
来源：http://ok.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dt.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bb.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uo.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ch.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ve.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://we.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://so.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wi.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://xm.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pl.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://de.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://su.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ol.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yi.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uy.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pl.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cf.szsharing.cn

================================================================================
来源：http://hh.jctech888.com.cn

K. JSON 与序列化
来源：http://vr.szsharing.cn

================================================================================
来源：http://pj.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://ha.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yr.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://or.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://ff.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://gi.yuntaijiaju.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://im.asd995.cn

Go:   json.Marshal(obj)
来源：http://us.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ni.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wi.colortex.cn

[K02] JSON 字符串转对象
来源：http://bj.9csxet.cn

Py:   json.loads(s)
来源：http://ze.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xi.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://ga.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ow.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://or.huixiangedu.cn

Go:   json.Unmarshal(data, &v)
来源：http://nq.huixinmuqiang.cn

Ruby: JSON.parse(s)
来源：http://he.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zk.haigaiapp.cn

[K03] JSON 美化输出（带缩进）
来源：http://wt.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gw.gzmigu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ke.muxihuayi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zd.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qy.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ys.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jy.lnxyls.cn


<!-- 参考信息 -->