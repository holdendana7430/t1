代发 wailian999

C#:   record User(string Name, int Age);
来源：http://bq.szsharing.cn

[G15] 枚举
来源：http://fo.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ox.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://am.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ka.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pv.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://rg.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eh.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://xp.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kn.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://yn.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pz.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://om.shxzskj.cn

JS:   Object.entries(obj)
来源：http://kx.hahajie.cn

TS:   Object.entries(obj)
来源：http://ja.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ql.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yi.panjiajie.cn

Ruby: obj.instance_variables
来源：http://gk.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://qy.newstarts.cn

================================================================================
来源：http://eb.colortex.cn

H. 异常与错误处理
来源：http://nx.yuexingan06.cn

================================================================================
来源：http://ee.bookmarksfly.cn

[H01] try / catch 基础
来源：http://hy.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ua.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wf.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://py.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gz.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uh.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bc.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://om.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bn.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://iy.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jn.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lo.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fb.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sh.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://it.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gz.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ba.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ez.newstarts.cn

[H03] 主动抛出异常
来源：http://qw.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://hz.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ms.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://mb.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://ua.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://th.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uo.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vb.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://da.521024.cn

[H04] 自定义异常类型
来源：http://rt.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://mh.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ru.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://rr.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://yd.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://xj.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nf.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://ef.szsharing.cn

C#:   class MyException : Exception {}
来源：http://tu.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://ll.hahajie.cn

Py:   except ValueError as e:
来源：http://er.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oi.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://bp.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://jq.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://xc.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mk.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://ou.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pg.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://tr.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://lm.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pt.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yp.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://db.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uf.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nl.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://qb.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://vp.jianghongdianzi.cn

[H07] 断言
来源：http://kw.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://ii.nszjky.cn

PHP:  assert($x > 0);
来源：http://mo.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://tq.asd995.cn

TS:   console.assert(x > 0);
来源：http://gv.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://nk.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eh.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cw.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://et.521024.cn

[H08] 获取错误信息与堆栈
来源：http://ad.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://fq.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gg.asd995.cn

JS:   e.message;  e.stack
来源：http://xw.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lq.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vw.panjiajie.cn

Go:   err.Error()
来源：http://lv.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://kc.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://sm.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://hs.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://li.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ic.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://na.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mm.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kz.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sj.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://af.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wm.asd995.cn

[H10] 资源自动释放
来源：http://rp.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wv.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lx.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dh.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cn.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oh.bookmarksfly.cn

Go:   defer f.Close()
来源：http://ss.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rs.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zo.lnxyls.cn

================================================================================
来源：http://gj.yuexingan06.cn

I. 正则表达式
来源：http://xt.hahajie.cn

================================================================================
来源：http://un.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://eo.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lz.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hp.nszjky.cn

JS:   /\d+/.test(s)
来源：http://lg.521024.cn

TS:   /\d+/.test(s)
来源：http://dk.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yv.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bg.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://xh.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bx.colortex.cn

[I02] 提取所有匹配
来源：http://cj.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://cl.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pj.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uh.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://jx.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gi.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cb.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://oj.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sd.panjiajie.cn

[I03] 提取捕获分组
来源：http://xu.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mo.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xc.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oy.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://et.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wt.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qb.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tj.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rf.jianghongdianzi.cn

[I04] 正则替换
来源：http://co.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kd.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pg.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zl.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tn.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fk.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://we.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rw.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hy.haigaiapp.cn

[I05] 按正则拆分
来源：http://sd.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hn.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ik.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://kr.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://yd.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://is.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rj.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ld.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lb.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ao.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ib.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xd.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vm.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wy.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://es.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ch.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ku.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jz.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://it.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mr.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ga.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bf.hahajie.cn

TS:   /error/gim
来源：http://vq.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ck.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hu.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://cm.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ty.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://vu.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ns.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tv.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pr.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dv.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tf.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zx.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ut.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qj.hahajie.cn

================================================================================
来源：http://oq.newstarts.cn

J. 日期与时间
来源：http://ey.shxzukj.cn

================================================================================
来源：http://bd.szsharing.cn

[J01] 获取当前时间
来源：http://rz.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lq.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fa.newstarts.cn

JS:   new Date();  Date.now()
来源：http://ob.nicolike.cn

TS:   new Date();  Date.now()
来源：http://nh.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hw.jctech888.com.cn

Go:   time.Now()
来源：http://sk.hahajie.cn

Ruby: Time.now
来源：http://vx.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ze.huixiangedu.cn

[J02] 格式化输出
来源：http://ka.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vb.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ma.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wb.lnxyls.cn

TS:   d.toISOString()
来源：http://dh.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fn.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zb.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hn.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sy.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://nl.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sb.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://em.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://lh.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://gp.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hu.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jc.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://ti.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zs.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://zd.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ah.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lb.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vr.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dr.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jb.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ba.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sm.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vf.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://rx.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://ej.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ga.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lt.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pc.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://op.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zw.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://zz.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lx.chemitech.net.cn

[J06] 计算两时间之差
来源：http://xh.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://py.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://ob.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://be.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://px.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://am.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://mb.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://qz.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://qb.shtwfgs.cn

[J07] 比较两个日期
来源：http://ir.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://rk.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lb.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ia.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://te.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xf.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ik.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iy.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://yk.lnxyls.cn

[J08] 提取年月日与星期
来源：http://ie.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lx.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ul.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ul.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ih.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rd.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://io.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wg.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fj.huixiangedu.cn

[J09] 时区处理
来源：http://hn.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ns.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yv.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vv.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rh.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mb.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tc.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yo.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://ry.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nt.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ha.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zq.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uy.szxytkj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qd.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zj.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bd.asd995.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zi.haigaiapp.cn

================================================================================
来源：http://mm.nicolike.cn

K. JSON 与序列化
来源：http://xn.nicolike.cn

================================================================================
来源：http://zz.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://gn.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zf.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://me.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://ay.shxzukj.cn

TS:   JSON.stringify(obj)
来源：http://vc.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ia.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://zg.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ev.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pt.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://yy.szsharing.cn

Py:   json.loads(s)
来源：http://ut.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tg.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://xn.shxzskj.cn

TS:   JSON.parse(s)
来源：http://rz.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://or.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://ng.haigaiapp.cn

Ruby: JSON.parse(s)
来源：http://se.hahajie.cn


<!-- 参考信息 -->