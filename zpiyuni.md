代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://yt.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://xl.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://xo.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://es.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ge.yuntaijiaju.cn

[G15] 枚举
来源：http://ny.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zp.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jm.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yi.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jv.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://nu.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mh.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://oh.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lr.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://ng.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zk.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://hz.shxzskj.cn

JS:   Object.entries(obj)
来源：http://wx.nszjky.cn

TS:   Object.entries(obj)
来源：http://pn.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://te.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nn.gzmigu.cn

Ruby: obj.instance_variables
来源：http://gz.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://ji.chemitech.net.cn

================================================================================
来源：http://ve.shxzukj.cn

H. 异常与错误处理
来源：http://vf.colortex.cn

================================================================================
来源：http://zm.gzmigu.cn

[H01] try / catch 基础
来源：http://zi.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pw.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://so.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fa.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tm.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://no.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eu.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vv.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gp.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://rb.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fs.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gc.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://om.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qy.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tg.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oj.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ds.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ha.yuexingan06.cn

[H03] 主动抛出异常
来源：http://ui.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://jx.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pg.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://bf.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://bc.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pq.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uj.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ka.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dq.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://li.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://rs.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ph.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://sp.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://la.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://qw.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nj.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://rm.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://ne.wgjwhj.cn

[H05] 捕获特定类型
来源：http://mn.lnxyls.cn

Py:   except ValueError as e:
来源：http://tp.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yd.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://do.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://us.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://sf.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ly.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://ve.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vt.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://ol.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://bc.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tg.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yz.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vl.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://on.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hm.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://wr.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://sw.hnjuh.cn

[H07] 断言
来源：http://pk.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://lk.shxzukj.cn

PHP:  assert($x > 0);
来源：http://fb.nszjky.cn

JS:   console.assert(x > 0);
来源：http://oz.colortex.cn

TS:   console.assert(x > 0);
来源：http://ew.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://ek.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qe.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://br.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://bo.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://cb.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://hg.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lo.shxzskj.cn

JS:   e.message;  e.stack
来源：http://ls.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tf.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://il.colortex.cn

Go:   err.Error()
来源：http://ua.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://tm.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://ds.shxzukj.cn

[H09] 带错误码的异常
来源：http://ri.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ac.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iz.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ie.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ze.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wt.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bc.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tb.hnjuh.cn

[H10] 资源自动释放
来源：http://sg.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rc.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://be.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vh.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hb.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jz.bookmarksfly.cn

Go:   defer f.Close()
来源：http://dh.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xn.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ep.shtwfgs.cn

================================================================================
来源：http://dp.newstarts.cn

I. 正则表达式
来源：http://md.nicolike.cn

================================================================================
来源：http://tc.szsharing.cn

[I01] 判断是否匹配
来源：http://mg.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wq.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://up.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://dt.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://og.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ca.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xi.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://sj.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gx.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://or.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://lz.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mt.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bu.colortex.cn

TS:   s.match(/\d+/g)
来源：http://wy.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vn.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ac.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://fc.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aq.huixiangedu.cn

[I03] 提取捕获分组
来源：http://yy.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zo.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://as.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ou.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://md.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mx.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oi.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oz.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gr.hnjuh.cn

[I04] 正则替换
来源：http://pa.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fs.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wp.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uj.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nf.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mi.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ls.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gl.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ev.colortex.cn

[I05] 按正则拆分
来源：http://ja.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://er.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tp.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://nu.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://tm.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://ul.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cm.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ny.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ff.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sk.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hd.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ky.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oy.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cy.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sq.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ry.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wv.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yi.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://rl.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mg.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ms.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mm.bjjhwx.cn

TS:   /error/gim
来源：http://kj.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cd.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kq.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://lh.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qo.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://mh.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dg.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ti.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://te.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rn.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lt.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vr.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ir.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mv.colortex.cn

================================================================================
来源：http://uf.gzmigu.cn

J. 日期与时间
来源：http://fc.szsharing.cn

================================================================================
来源：http://uw.hahajie.cn

[J01] 获取当前时间
来源：http://gr.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hx.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sp.9csxet.cn

JS:   new Date();  Date.now()
来源：http://ql.huanxung.cn

TS:   new Date();  Date.now()
来源：http://gu.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ja.hahajie.cn

Go:   time.Now()
来源：http://py.9csxet.cn

Ruby: Time.now
来源：http://oi.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ae.wgjwhj.cn

[J02] 格式化输出
来源：http://gm.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yz.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bf.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jz.szsharing.cn

TS:   d.toISOString()
来源：http://xk.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lg.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zb.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gh.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ke.panjiajie.cn

[J03] 字符串解析为日期
来源：http://vm.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gq.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xh.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://xk.asd995.cn

TS:   new Date("2024-01-02")
来源：http://if.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aw.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tp.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://to.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cw.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://yw.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ld.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://su.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rx.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ql.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tl.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kz.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vd.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wv.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://zp.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://ma.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tp.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dq.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pr.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://wv.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nw.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://th.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zn.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://ok.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://pu.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://hw.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yp.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://se.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ll.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://ba.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://uf.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://yo.shxzskj.cn

[J07] 比较两个日期
来源：http://ht.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://lx.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lv.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ol.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bz.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ai.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kj.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hi.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://sv.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://wi.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nt.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ny.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tt.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kc.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tx.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vd.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fx.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jz.muxihuayi.cn

[J09] 时区处理
来源：http://wr.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cm.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yz.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cs.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ya.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ps.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cd.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ph.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pr.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://ri.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ch.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ld.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cb.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ai.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cv.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nh.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ug.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nb.colortex.cn

================================================================================
来源：http://ia.muxihuayi.cn

K. JSON 与序列化
来源：http://ui.huixiangedu.cn

================================================================================
来源：http://lr.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://hg.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xj.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wj.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://vx.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://oo.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bs.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://zi.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ku.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mi.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://hn.hnjuh.cn

Py:   json.loads(s)
来源：http://vo.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mo.521024.cn

JS:   JSON.parse(s)
来源：http://rr.huixiangedu.cn


<!-- 参考信息 -->