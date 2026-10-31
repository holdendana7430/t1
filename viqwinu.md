代发 wailian999

Java: u instanceof User
来源：http://ph.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lc.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://kd.huanxung.cn

C#:   u is User
来源：http://yn.hahajie.cn

[G14] 数据类 / record
来源：http://oj.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rf.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://ri.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ut.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://ky.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://gl.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://qz.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tm.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://pr.gzmigu.cn

[G15] 枚举
来源：http://sq.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oq.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qh.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fi.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://tn.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://le.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://mg.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vt.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://zb.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jt.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://na.szsharing.cn

JS:   Object.entries(obj)
来源：http://em.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://ab.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hw.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pa.shxzskj.cn

Ruby: obj.instance_variables
来源：http://fj.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://dr.chemitech.net.cn

================================================================================
来源：http://hy.szxytkj.cn

H. 异常与错误处理
来源：http://xp.jianghongdianzi.cn

================================================================================
来源：http://xt.shxzskj.cn

[H01] try / catch 基础
来源：http://dk.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tr.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sg.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wv.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xp.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lm.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xp.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://je.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gs.asd995.cn

[H02] finally / ensure 收尾
来源：http://vu.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oh.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hc.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gz.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mx.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gj.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wm.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qp.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ak.bjjhwx.cn

[H03] 主动抛出异常
来源：http://ad.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://zz.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cm.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://xx.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://hw.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lp.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ip.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dw.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lx.panjiajie.cn

[H04] 自定义异常类型
来源：http://bx.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://ri.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://px.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://sm.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://he.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://dk.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yc.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://xd.asd995.cn

C#:   class MyException : Exception {}
来源：http://zc.huanxung.cn

[H05] 捕获特定类型
来源：http://tb.szxytkj.cn

Py:   except ValueError as e:
来源：http://dg.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://te.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://qj.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://tp.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://pl.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yc.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://rp.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yt.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://vh.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://bj.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dx.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wq.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qv.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://na.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nk.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://tw.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://bq.bookmarksfly.cn

[H07] 断言
来源：http://up.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://tv.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://dz.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://rv.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://vh.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://kd.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yk.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://od.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://fd.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://mn.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://li.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bp.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://pe.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nt.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ag.colortex.cn

Go:   err.Error()
来源：http://nf.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://rd.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://cu.newstarts.cn

[H09] 带错误码的异常
来源：http://at.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sd.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://af.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gp.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sr.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dh.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iz.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://os.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cx.hnjuh.cn

[H10] 资源自动释放
来源：http://pv.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jd.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pu.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mi.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vr.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kt.hnjuh.cn

Go:   defer f.Close()
来源：http://ur.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cc.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pb.hnjuh.cn

================================================================================
来源：http://ih.chemitech.net.cn

I. 正则表达式
来源：http://qo.gzmigu.cn

================================================================================
来源：http://ri.gzmigu.cn

[I01] 判断是否匹配
来源：http://ap.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hb.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xh.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://nu.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ih.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://up.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oe.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://ek.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kk.asd995.cn

[I02] 提取所有匹配
来源：http://ij.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://ot.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ve.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tg.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://rn.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ta.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ax.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://ab.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yl.huanxung.cn

[I03] 提取捕获分组
来源：http://yo.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ri.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ua.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vl.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dy.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wv.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kx.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jm.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rp.9csxet.cn

[I04] 正则替换
来源：http://gd.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://er.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bi.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dc.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sk.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lu.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gy.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xr.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cs.yuexingan06.cn

[I05] 按正则拆分
来源：http://tu.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nf.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vd.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://sv.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://of.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://aw.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qs.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xi.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pm.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ou.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lx.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jx.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ao.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vz.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://er.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xw.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fi.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://di.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://gq.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yi.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nb.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bf.521024.cn

TS:   /error/gim
来源：http://po.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://za.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ub.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://gd.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rr.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://wz.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://px.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ce.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://te.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gq.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vs.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ql.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yt.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aw.szsharing.cn

================================================================================
来源：http://pw.gzmigu.cn

J. 日期与时间
来源：http://iy.jctech888.com.cn

================================================================================
来源：http://bi.szxytkj.cn

[J01] 获取当前时间
来源：http://fu.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zs.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kf.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://wt.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://hu.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zj.bjjhwx.cn

Go:   time.Now()
来源：http://zs.haigaiapp.cn

Ruby: Time.now
来源：http://up.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kd.chemitech.net.cn

[J02] 格式化输出
来源：http://do.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zu.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cr.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jt.gzmigu.cn

TS:   d.toISOString()
来源：http://ca.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dn.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jd.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zh.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cz.gzmigu.cn

[J03] 字符串解析为日期
来源：http://am.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xp.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jn.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://sr.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://tf.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hn.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ed.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://qm.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qq.521024.cn

[J04] 时间戳与日期互转
来源：http://mz.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ua.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://db.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ak.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fr.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gu.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qf.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gd.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vx.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://br.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://hl.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wt.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yd.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://va.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://gd.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qs.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ys.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cr.hnjuh.cn

[J06] 计算两时间之差
来源：http://ui.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://lm.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://op.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ou.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hv.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pr.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://cd.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://nx.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://id.bookmarksfly.cn

[J07] 比较两个日期
来源：http://li.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://uo.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yd.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hr.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jz.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yl.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lq.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qs.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://pg.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://up.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pa.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xz.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wn.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bd.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://em.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xq.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bs.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vp.szxytkj.cn

[J09] 时区处理
来源：http://mx.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://es.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fy.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ad.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nb.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oc.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wo.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ke.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mc.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://nx.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://it.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aa.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://le.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ko.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://of.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dp.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bp.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://br.huixiangedu.cn

================================================================================
来源：http://bn.panjiajie.cn

K. JSON 与序列化
来源：http://vs.hahajie.cn

================================================================================
来源：http://pa.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://et.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xx.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://el.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://fp.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://dt.gzmigu.cn


<!-- 参考信息 -->