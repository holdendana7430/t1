代发 wailian999

C#:   record User(string Name, int Age);
来源：http://vl.yuntaijiaju.cn

[G15] 枚举
来源：http://tt.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iq.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ga.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rb.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gy.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://lz.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nr.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://rk.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kr.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://vf.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hn.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://hu.shxzukj.cn

JS:   Object.entries(obj)
来源：http://sd.shxzukj.cn

TS:   Object.entries(obj)
来源：http://ni.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vt.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nn.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://gp.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ye.huixiangedu.cn

================================================================================
来源：http://dj.colortex.cn

H. 异常与错误处理
来源：http://ua.newstarts.cn

================================================================================
来源：http://xn.gzmigu.cn

[H01] try / catch 基础
来源：http://fh.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fc.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vu.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nh.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vi.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jd.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mh.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tk.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rq.nszjky.cn

[H02] finally / ensure 收尾
来源：http://pk.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ty.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wa.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fz.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sw.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yf.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ms.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wl.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ow.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://ya.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://fl.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://km.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://eg.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://cd.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fm.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vt.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ma.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uh.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://fo.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://zo.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qq.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://ng.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://jn.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://nb.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qs.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://jc.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://tf.nszjky.cn

[H05] 捕获特定类型
来源：http://vg.colortex.cn

Py:   except ValueError as e:
来源：http://nw.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yd.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://sp.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://mx.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://og.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ft.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://yc.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://li.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://jt.asd995.cn

Py:   value = d.get("k") or default
来源：http://am.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://de.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iq.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mn.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kt.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fv.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://st.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://ui.gzmigu.cn

[H07] 断言
来源：http://yu.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://yj.szsharing.cn

PHP:  assert($x > 0);
来源：http://pt.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://en.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://ps.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://aj.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qc.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://od.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ob.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://bu.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://hd.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://az.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://sa.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mm.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qr.shtwfgs.cn

Go:   err.Error()
来源：http://kn.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://vk.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://ts.szsharing.cn

[H09] 带错误码的异常
来源：http://le.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qb.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vq.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vf.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rr.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mt.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cn.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yg.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://me.chemitech.net.cn

[H10] 资源自动释放
来源：http://qs.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bf.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ta.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xa.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vy.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zk.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://pk.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eu.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pm.chemitech.net.cn

================================================================================
来源：http://en.yuntaijiaju.cn

I. 正则表达式
来源：http://tw.asd995.cn

================================================================================
来源：http://bm.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://xp.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eo.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jy.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://yx.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://km.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nd.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uc.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://kr.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fv.newstarts.cn

[I02] 提取所有匹配
来源：http://tl.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://in.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kp.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rz.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://gq.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jj.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oj.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://ce.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://za.bjjhwx.cn

[I03] 提取捕获分组
来源：http://lm.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rv.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pf.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kd.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aw.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oy.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ka.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hq.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hp.huanxung.cn

[I04] 正则替换
来源：http://yi.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jl.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://do.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ss.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rm.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tg.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qc.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kd.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qw.hahajie.cn

[I05] 按正则拆分
来源：http://fd.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wl.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dt.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://yj.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://fc.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://sy.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://up.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bs.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zn.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vn.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hi.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dw.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wn.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vb.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rz.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xf.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gf.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pm.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://co.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xw.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tp.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vu.newstarts.cn

TS:   /error/gim
来源：http://ep.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pl.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ik.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://ff.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ev.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://rn.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ov.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ld.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uo.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ko.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ns.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kr.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dz.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cd.nicolike.cn

================================================================================
来源：http://nj.muxihuayi.cn

J. 日期与时间
来源：http://fp.shxzskj.cn

================================================================================
来源：http://wr.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://xk.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vh.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pz.colortex.cn

JS:   new Date();  Date.now()
来源：http://mp.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://en.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ov.huixinmuqiang.cn

Go:   time.Now()
来源：http://yd.panjiajie.cn

Ruby: Time.now
来源：http://dn.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tp.521024.cn

[J02] 格式化输出
来源：http://tw.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jw.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ya.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jq.haigaiapp.cn

TS:   d.toISOString()
来源：http://la.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://be.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fj.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mr.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://af.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://jh.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ww.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ge.colortex.cn

JS:   new Date("2024-01-02")
来源：http://eq.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://ov.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lf.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bb.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://zj.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://le.asd995.cn

[J04] 时间戳与日期互转
来源：http://te.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://av.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mo.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://io.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ry.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ei.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lq.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oe.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rq.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://rf.asd995.cn

Py:   now + timedelta(days=7)
来源：http://qf.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sq.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mb.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mp.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://ex.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ah.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://ng.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nf.haigaiapp.cn

[J06] 计算两时间之差
来源：http://rf.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://bk.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://ii.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pa.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hu.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ge.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://ft.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://oy.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://rm.bookmarksfly.cn

[J07] 比较两个日期
来源：http://tp.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://lr.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hp.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ub.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wh.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gk.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mi.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bd.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://gq.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://my.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jc.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fq.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lx.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qi.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://va.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bk.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kr.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tt.9csxet.cn

[J09] 时区处理
来源：http://ir.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sx.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wv.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ef.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kv.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lc.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vo.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kq.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://lb.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lf.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zb.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mm.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ub.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ma.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qx.521024.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hd.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ur.lnxyls.cn

================================================================================
来源：http://ps.nszjky.cn

K. JSON 与序列化
来源：http://qq.nszjky.cn

================================================================================
来源：http://is.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://nx.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vy.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ud.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://rs.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://tt.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nh.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://ex.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tg.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cx.9csxet.cn

[K02] JSON 字符串转对象
来源：http://uc.haigaiapp.cn

Py:   json.loads(s)
来源：http://fq.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rw.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://gm.shxzukj.cn

TS:   JSON.parse(s)
来源：http://ph.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://do.nicolike.cn

Go:   json.Unmarshal(data, &v)
来源：http://oz.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://ym.huanxung.cn


<!-- 参考信息 -->