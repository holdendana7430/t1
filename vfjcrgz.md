代发 wailian999

[G14] 数据类 / record
来源：http://pq.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iy.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://dr.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mb.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://ay.huanxung.cn

Java: record User(String name, int age) {}
来源：http://yg.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://pa.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xu.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://ti.lnxyls.cn

[G15] 枚举
来源：http://yz.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fd.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fc.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://th.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bl.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://ax.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kd.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://xb.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://je.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://mo.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qu.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://qc.panjiajie.cn

JS:   Object.entries(obj)
来源：http://qk.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://am.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://df.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ic.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://fu.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://hv.huanxung.cn

================================================================================
来源：http://vr.521024.cn

H. 异常与错误处理
来源：http://bv.panjiajie.cn

================================================================================
来源：http://cb.wgjwhj.cn

[H01] try / catch 基础
来源：http://fs.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mq.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gu.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tb.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cx.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nw.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://as.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cy.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fy.9csxet.cn

[H02] finally / ensure 收尾
来源：http://ez.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hl.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ee.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ea.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qz.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://te.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ab.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://we.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iz.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://tl.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://uu.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ft.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://yy.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://zd.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bg.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ti.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gl.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bb.9csxet.cn

[H04] 自定义异常类型
来源：http://tt.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://nv.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://im.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://og.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://mb.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://rn.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nv.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://xv.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://ab.lnxyls.cn

[H05] 捕获特定类型
来源：http://ri.lnxyls.cn

Py:   except ValueError as e:
来源：http://nq.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ax.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://hq.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://mu.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://qp.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jz.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://nd.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cw.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://aw.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://lr.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bn.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kz.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ck.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gp.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ln.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://yf.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://kw.huixiangedu.cn

[H07] 断言
来源：http://km.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://wv.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://sh.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://lu.colortex.cn

TS:   console.assert(x > 0);
来源：http://xh.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://in.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mm.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kv.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://tw.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://ts.yuexingan06.cn

Py:   str(e);  traceback.format_exc()
来源：http://zh.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iq.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://tr.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qx.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://as.hahajie.cn

Go:   err.Error()
来源：http://db.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://ow.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://qa.haigaiapp.cn

[H09] 带错误码的异常
来源：http://mt.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://er.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://my.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tt.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ae.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kp.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xp.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qq.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wq.szxytkj.cn

[H10] 资源自动释放
来源：http://ik.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lc.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fx.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eq.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ax.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jr.wgjwhj.cn

Go:   defer f.Close()
来源：http://sz.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wl.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ei.bookmarksfly.cn

================================================================================
来源：http://jp.wgjwhj.cn

I. 正则表达式
来源：http://hf.bjjhwx.cn

================================================================================
来源：http://bt.9csxet.cn

[I01] 判断是否匹配
来源：http://op.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kn.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gk.szsharing.cn

JS:   /\d+/.test(s)
来源：http://xb.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://lr.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cb.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ug.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://kc.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vq.hnjuh.cn

[I02] 提取所有匹配
来源：http://fh.szsharing.cn

Py:   re.findall(r"\d+", s)
来源：http://tq.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vs.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fm.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://ro.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qm.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wn.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://ts.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dq.haigaiapp.cn

[I03] 提取捕获分组
来源：http://vp.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zr.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hy.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lh.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oz.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fh.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vm.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fl.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yq.lnxyls.cn

[I04] 正则替换
来源：http://af.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wa.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jl.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ek.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nh.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fc.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kp.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vp.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://be.newstarts.cn

[I05] 按正则拆分
来源：http://fc.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xt.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vz.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://yk.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://dl.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://ef.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ae.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bt.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ji.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wq.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bd.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cl.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wo.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cr.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xa.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ys.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tp.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://af.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://fy.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gd.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ks.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cw.yuexingan06.cn

TS:   /error/gim
来源：http://eg.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xt.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ok.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://tq.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://to.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://db.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jp.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pl.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jd.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rf.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gs.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iw.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gv.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vm.yuexingan06.cn

================================================================================
来源：http://kq.szxytkj.cn

J. 日期与时间
来源：http://uj.panjiajie.cn

================================================================================
来源：http://as.gzmigu.cn

[J01] 获取当前时间
来源：http://ov.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qz.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wf.szsharing.cn

JS:   new Date();  Date.now()
来源：http://nd.hahajie.cn

TS:   new Date();  Date.now()
来源：http://go.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hp.huixiangedu.cn

Go:   time.Now()
来源：http://zg.yuexingan06.cn

Ruby: Time.now
来源：http://wn.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uk.muxihuayi.cn

[J02] 格式化输出
来源：http://vr.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://re.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wk.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oo.chemitech.net.cn

TS:   d.toISOString()
来源：http://vz.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://co.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ty.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mj.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ma.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://lb.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qb.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iw.521024.cn

JS:   new Date("2024-01-02")
来源：http://wt.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://zi.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bb.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xr.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://zb.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rc.huanxung.cn

[J04] 时间戳与日期互转
来源：http://sa.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ua.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lv.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qc.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ed.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pa.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kw.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://is.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mw.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://jt.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://ts.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sp.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jh.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kq.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ca.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sm.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://ic.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fd.haigaiapp.cn

[J06] 计算两时间之差
来源：http://hk.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://dr.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://oi.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nd.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://it.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ep.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://xj.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://bi.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://su.colortex.cn

[J07] 比较两个日期
来源：http://ly.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://az.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pf.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jn.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rw.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uz.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://op.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vb.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://pg.9csxet.cn

[J08] 提取年月日与星期
来源：http://ff.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xs.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rf.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://be.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ch.shxzskj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wb.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jp.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ih.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tu.chemitech.net.cn

[J09] 时区处理
来源：http://bh.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bo.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://za.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jz.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ej.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fg.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cj.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tg.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bo.newstarts.cn

[J10] 取今天 / 本月第一天
来源：http://em.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mk.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ud.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wz.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bf.panjiajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iz.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qe.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rg.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ui.szxytkj.cn

================================================================================
来源：http://tw.hahajie.cn

K. JSON 与序列化
来源：http://ke.jianghongdianzi.cn

================================================================================
来源：http://wq.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://dd.huanxung.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://df.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zn.shtwfgs.cn

JS:   JSON.stringify(obj)
来源：http://cv.521024.cn

TS:   JSON.stringify(obj)
来源：http://pf.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://si.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://dz.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xy.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rl.newstarts.cn


<!-- 参考信息 -->