代发 wailian999

[G14] 数据类 / record
来源：http://vu.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ej.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://cp.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dy.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://pb.nszjky.cn

Java: record User(String name, int age) {}
来源：http://fp.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://ta.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://la.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://jw.huixiangedu.cn

[G15] 枚举
来源：http://sy.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ta.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zw.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hw.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cg.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://xi.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mb.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://ub.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ad.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://ds.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://em.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://gq.gzmigu.cn

JS:   Object.entries(obj)
来源：http://mi.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://dn.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gi.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rt.szxytkj.cn

Ruby: obj.instance_variables
来源：http://nn.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://jk.hahajie.cn

================================================================================
来源：http://jw.haigaiapp.cn

H. 异常与错误处理
来源：http://hn.nszjky.cn

================================================================================
来源：http://qv.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://eb.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tz.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jg.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nv.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mt.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jp.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dm.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qt.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xx.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://qx.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rw.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hf.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://at.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rl.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ww.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wj.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kt.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tm.nicolike.cn

[H03] 主动抛出异常
来源：http://aq.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://fl.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ix.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://fh.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://fz.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ci.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kw.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bm.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ku.shxzukj.cn

[H04] 自定义异常类型
来源：http://hs.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://nt.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wp.asd995.cn

JS:   class MyError extends Error {}
来源：http://qx.hahajie.cn

TS:   class MyError extends Error {}
来源：http://qi.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://ij.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zj.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://by.newstarts.cn

C#:   class MyException : Exception {}
来源：http://lz.asd995.cn

[H05] 捕获特定类型
来源：http://vm.bjjhwx.cn

Py:   except ValueError as e:
来源：http://of.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fz.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://hb.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://gx.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://xr.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fc.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://pe.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zt.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://eu.nszjky.cn

Py:   value = d.get("k") or default
来源：http://hb.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uh.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nc.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mg.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ce.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fj.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://wd.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://yj.9csxet.cn

[H07] 断言
来源：http://bb.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://ey.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://hx.9csxet.cn

JS:   console.assert(x > 0);
来源：http://gk.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://my.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://ox.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lv.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xj.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://il.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://pe.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://hc.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sf.asd995.cn

JS:   e.message;  e.stack
来源：http://nw.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xg.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jl.chemitech.net.cn

Go:   err.Error()
来源：http://mr.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://kn.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://vw.521024.cn

[H09] 带错误码的异常
来源：http://wu.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jd.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ci.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bm.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cc.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dm.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://il.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wb.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tr.huixiangedu.cn

[H10] 资源自动释放
来源：http://wj.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fd.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iy.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hm.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ky.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lu.521024.cn

Go:   defer f.Close()
来源：http://it.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sh.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yz.jianghongdianzi.cn

================================================================================
来源：http://to.bjjhwx.cn

I. 正则表达式
来源：http://iz.gzmigu.cn

================================================================================
来源：http://bm.huanxung.cn

[I01] 判断是否匹配
来源：http://nc.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zm.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qo.colortex.cn

JS:   /\d+/.test(s)
来源：http://qz.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://pu.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://em.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://az.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://xr.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vo.asd995.cn

[I02] 提取所有匹配
来源：http://ey.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://sx.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ym.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nz.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://zc.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zn.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xo.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://iv.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mz.haigaiapp.cn

[I03] 提取捕获分组
来源：http://nf.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aa.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ra.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yc.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fb.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ue.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cu.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zk.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://em.gzmigu.cn

[I04] 正则替换
来源：http://pc.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mi.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xk.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wh.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tf.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lw.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fb.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qt.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zn.szsharing.cn

[I05] 按正则拆分
来源：http://ma.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nq.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zo.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ob.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://vw.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://fa.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://te.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jx.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ze.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ip.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kk.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xo.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ab.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bu.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ba.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tq.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ax.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ws.521024.cn

[I07] 忽略大小写与多行模式
来源：http://mz.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xr.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pe.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fu.wgjwhj.cn

TS:   /error/gim
来源：http://rz.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bx.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ay.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://dh.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ev.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://iv.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cs.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://io.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uq.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wi.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://do.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iv.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yt.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sc.nicolike.cn

================================================================================
来源：http://ta.shtwfgs.cn

J. 日期与时间
来源：http://vx.bookmarksfly.cn

================================================================================
来源：http://pu.gzmigu.cn

[J01] 获取当前时间
来源：http://cv.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yn.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lo.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://az.nszjky.cn

TS:   new Date();  Date.now()
来源：http://kx.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tw.muxihuayi.cn

Go:   time.Now()
来源：http://az.huixiangedu.cn

Ruby: Time.now
来源：http://sw.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rv.huanxung.cn

[J02] 格式化输出
来源：http://qo.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ca.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bj.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pk.bjjhwx.cn

TS:   d.toISOString()
来源：http://mq.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ie.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://co.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ee.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pk.shxzukj.cn

[J03] 字符串解析为日期
来源：http://hq.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ad.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hp.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://za.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://sl.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dn.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://al.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://gp.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://to.asd995.cn

[J04] 时间戳与日期互转
来源：http://hv.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wp.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tp.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pr.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xn.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qn.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://td.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xx.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fm.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://xp.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://nx.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ny.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ax.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iq.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://op.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yu.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://vj.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bh.yuexingan06.cn

[J06] 计算两时间之差
来源：http://to.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://wk.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://bi.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fr.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sf.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lx.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ke.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://ks.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://wp.9csxet.cn

[J07] 比较两个日期
来源：http://vc.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ij.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sm.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uh.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ld.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://au.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ll.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://es.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://cl.9csxet.cn

[J08] 提取年月日与星期
来源：http://ed.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://su.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bt.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pb.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jw.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gx.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wy.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ix.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sj.haigaiapp.cn

[J09] 时区处理
来源：http://eo.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lj.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mf.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ha.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ld.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pa.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mt.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ml.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pc.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://rz.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jh.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oh.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ky.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qj.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zf.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://em.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cf.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bx.yuntaijiaju.cn

================================================================================
来源：http://xo.szsharing.cn

K. JSON 与序列化
来源：http://cn.huixinmuqiang.cn

================================================================================
来源：http://ay.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://df.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pi.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nu.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://id.hahajie.cn

TS:   JSON.stringify(obj)
来源：http://uj.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dp.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://ni.gzmigu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uy.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ra.yuexingan06.cn


<!-- 参考信息 -->