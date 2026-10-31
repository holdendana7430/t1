代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://aa.huanxung.cn

Java: record User(String name, int age) {}
来源：http://br.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://an.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eb.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://mg.gzmigu.cn

[G15] 枚举
来源：http://kd.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bo.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nq.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sg.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sm.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://cq.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yi.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://gf.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qk.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://ip.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ls.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://la.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://kn.521024.cn

TS:   Object.entries(obj)
来源：http://oh.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xs.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qi.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://cv.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://hf.jctech888.com.cn

================================================================================
来源：http://wf.jianghongdianzi.cn

H. 异常与错误处理
来源：http://qg.newstarts.cn

================================================================================
来源：http://ru.newstarts.cn

[H01] try / catch 基础
来源：http://fp.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wi.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pr.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ay.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nt.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qh.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ve.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jl.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ie.521024.cn

[H02] finally / ensure 收尾
来源：http://bf.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gr.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://et.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qa.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wz.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ar.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://by.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mu.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fw.haigaiapp.cn

[H03] 主动抛出异常
来源：http://bh.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://di.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mj.asd995.cn

JS:   throw new Error("错误信息");
来源：http://lf.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://rk.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qn.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gn.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dg.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://db.hnjuh.cn

[H04] 自定义异常类型
来源：http://ta.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://ma.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fm.9csxet.cn

JS:   class MyError extends Error {}
来源：http://nr.hahajie.cn

TS:   class MyError extends Error {}
来源：http://yw.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ow.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ba.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://ba.521024.cn

C#:   class MyException : Exception {}
来源：http://ig.panjiajie.cn

[H05] 捕获特定类型
来源：http://nu.szxytkj.cn

Py:   except ValueError as e:
来源：http://fe.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wf.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://jg.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://ja.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://ra.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sa.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://ut.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ja.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://gx.szsharing.cn

Py:   value = d.get("k") or default
来源：http://sk.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://me.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lm.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zw.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xh.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xo.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ik.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://es.nicolike.cn

[H07] 断言
来源：http://ex.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://pw.szsharing.cn

PHP:  assert($x > 0);
来源：http://yq.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://im.huanxung.cn

TS:   console.assert(x > 0);
来源：http://xs.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://yp.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ki.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://se.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://tn.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://oz.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://at.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pa.lnxyls.cn

JS:   e.message;  e.stack
来源：http://xc.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ks.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tp.asd995.cn

Go:   err.Error()
来源：http://zz.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://ls.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://pi.chemitech.net.cn

[H09] 带错误码的异常
来源：http://cx.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gs.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://te.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://er.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://or.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ea.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fe.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jk.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://js.9csxet.cn

[H10] 资源自动释放
来源：http://jw.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gw.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jx.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tl.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lp.huanxung.cn

Go:   defer f.Close()
来源：http://ux.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://le.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hr.haigaiapp.cn

================================================================================
来源：http://ea.9csxet.cn

I. 正则表达式
来源：http://hu.huanxung.cn

================================================================================
来源：http://tc.bjjhwx.cn

[I01] 判断是否匹配
来源：http://wp.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pe.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ig.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://pr.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://jq.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ih.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yv.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://hi.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ps.521024.cn

[I02] 提取所有匹配
来源：http://yo.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://ww.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vy.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nb.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://sy.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jc.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://un.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://pm.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zt.521024.cn

[I03] 提取捕获分组
来源：http://gt.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sd.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yu.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ao.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ac.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vj.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fm.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wg.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pq.colortex.cn

[I04] 正则替换
来源：http://hg.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zk.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ub.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oy.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hx.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vg.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sv.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uy.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ln.huixiangedu.cn

[I05] 按正则拆分
来源：http://pc.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tt.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bb.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://fj.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://eo.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://xj.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ta.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pt.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lr.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kk.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ve.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pn.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://la.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vf.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kd.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://of.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kq.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ds.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://ve.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rv.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ir.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ie.huixiangedu.cn

TS:   /error/gim
来源：http://nk.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ny.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ap.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://qz.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xl.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://tp.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gb.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zy.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kt.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xp.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ji.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pr.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ek.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ix.muxihuayi.cn

================================================================================
来源：http://jv.asd995.cn

J. 日期与时间
来源：http://pq.yuntaijiaju.cn

================================================================================
来源：http://gl.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://xf.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hm.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cs.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://un.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://jx.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fg.gzmigu.cn

Go:   time.Now()
来源：http://ay.yuexingan06.cn

Ruby: Time.now
来源：http://wo.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://st.huixinmuqiang.cn

[J02] 格式化输出
来源：http://mm.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ju.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zg.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ij.panjiajie.cn

TS:   d.toISOString()
来源：http://gg.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qz.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xt.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gq.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fq.shxzskj.cn

[J03] 字符串解析为日期
来源：http://rz.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://na.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://no.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://mg.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://ip.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ak.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tk.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://al.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gb.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://un.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eh.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://to.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vc.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ow.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://un.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fe.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nt.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gg.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://wp.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://dd.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xy.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rr.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ei.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://bz.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pu.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://ag.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gz.asd995.cn

[J06] 计算两时间之差
来源：http://vl.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://sv.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://te.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uk.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fc.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jq.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://xs.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://vn.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://ul.lnxyls.cn

[J07] 比较两个日期
来源：http://wk.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://gv.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nh.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xw.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dp.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dq.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yx.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bk.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://on.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://qz.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ak.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://an.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xh.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cz.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://un.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xs.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cp.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yf.szxytkj.cn

[J09] 时区处理
来源：http://jv.yuntaijiaju.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gk.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iz.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dl.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ad.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ey.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kw.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cb.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://ir.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rg.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yq.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cx.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ny.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yu.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ul.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://io.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://br.nszjky.cn

================================================================================
来源：http://tb.hnjuh.cn

K. JSON 与序列化
来源：http://mh.newstarts.cn

================================================================================
来源：http://ux.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://dk.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://er.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lc.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://dx.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://kl.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lz.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://di.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mx.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://od.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://ka.yuexingan06.cn

Py:   json.loads(s)
来源：http://jz.jianghongdianzi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://he.asd995.cn

JS:   JSON.parse(s)
来源：http://gq.colortex.cn


<!-- 参考信息 -->