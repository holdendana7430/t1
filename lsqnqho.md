代发 wailian999

[G14] 数据类 / record
来源：http://rz.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dt.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://fe.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lv.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://dg.nicolike.cn

Java: record User(String name, int age) {}
来源：http://or.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://ff.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wp.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://gx.nszjky.cn

[G15] 枚举
来源：http://uw.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yr.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sg.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fz.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qr.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://bt.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vk.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://cl.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://do.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://uz.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ed.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://fe.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://mo.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://hf.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kf.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ud.panjiajie.cn

Ruby: obj.instance_variables
来源：http://zu.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ti.shtwfgs.cn

================================================================================
来源：http://dr.shxzukj.cn

H. 异常与错误处理
来源：http://ly.521024.cn

================================================================================
来源：http://eq.newstarts.cn

[H01] try / catch 基础
来源：http://pt.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rz.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jq.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pj.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hm.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pi.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rq.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hp.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gh.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://nv.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kf.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ud.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ki.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lg.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xy.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dh.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fl.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://af.szsharing.cn

[H03] 主动抛出异常
来源：http://ei.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://tz.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zr.colortex.cn

JS:   throw new Error("错误信息");
来源：http://tj.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://xg.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ev.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xp.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gh.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hd.asd995.cn

[H04] 自定义异常类型
来源：http://vj.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://wy.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bd.9csxet.cn

JS:   class MyError extends Error {}
来源：http://mm.asd995.cn

TS:   class MyError extends Error {}
来源：http://zv.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://sy.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rs.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://wx.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://sh.9csxet.cn

[H05] 捕获特定类型
来源：http://zi.jctech888.com.cn

Py:   except ValueError as e:
来源：http://mc.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ko.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://fz.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://au.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://bx.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mg.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://my.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qe.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ut.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://vc.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bm.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dg.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zi.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sw.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xi.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://ka.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://br.muxihuayi.cn

[H07] 断言
来源：http://an.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://aj.huanxung.cn

PHP:  assert($x > 0);
来源：http://of.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://hd.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://gt.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://oo.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://il.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sm.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://tf.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://ip.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://ec.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dw.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://jm.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bo.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dv.asd995.cn

Go:   err.Error()
来源：http://jm.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://vo.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://rc.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://iw.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jm.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zg.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bw.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yx.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ie.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://az.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oj.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hs.newstarts.cn

[H10] 资源自动释放
来源：http://yi.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ti.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vm.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bv.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tn.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://or.bjjhwx.cn

Go:   defer f.Close()
来源：http://xb.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nz.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cw.yuntaijiaju.cn

================================================================================
来源：http://kt.huixiangedu.cn

I. 正则表达式
来源：http://yg.hahajie.cn

================================================================================
来源：http://yb.huixiangedu.cn

[I01] 判断是否匹配
来源：http://tl.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pj.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ml.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://eo.asd995.cn

TS:   /\d+/.test(s)
来源：http://yf.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rc.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kj.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://zk.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://om.huixiangedu.cn

[I02] 提取所有匹配
来源：http://qt.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://vn.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iv.shxzskj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gt.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://ne.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jl.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ld.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://yb.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://la.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://nf.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dz.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gf.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rp.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ke.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rj.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lo.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://is.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cb.hnjuh.cn

[I04] 正则替换
来源：http://sy.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ti.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mw.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ck.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zn.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ke.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nq.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nd.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ip.hnjuh.cn

[I05] 按正则拆分
来源：http://vo.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://in.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gj.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://qq.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ju.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://kg.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pd.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jn.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ex.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vl.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ni.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dv.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pv.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aj.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pp.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zx.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lp.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ye.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://de.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uw.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jb.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yy.nicolike.cn

TS:   /error/gim
来源：http://if.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://km.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://go.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://xc.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bw.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://sk.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dr.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zw.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qr.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jd.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hh.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pg.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nm.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zi.huanxung.cn

================================================================================
来源：http://mt.shxzukj.cn

J. 日期与时间
来源：http://ed.panjiajie.cn

================================================================================
来源：http://yv.asd995.cn

[J01] 获取当前时间
来源：http://aa.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yh.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gt.colortex.cn

JS:   new Date();  Date.now()
来源：http://ea.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://wt.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ws.nszjky.cn

Go:   time.Now()
来源：http://fr.panjiajie.cn

Ruby: Time.now
来源：http://th.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bc.panjiajie.cn

[J02] 格式化输出
来源：http://nz.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://so.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ao.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gu.huixiangedu.cn

TS:   d.toISOString()
来源：http://tt.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ey.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oi.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vb.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ck.hahajie.cn

[J03] 字符串解析为日期
来源：http://nl.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bq.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fj.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://dx.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://yz.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mc.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pz.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://jx.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://it.colortex.cn

[J04] 时间戳与日期互转
来源：http://vm.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ur.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://be.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bn.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yk.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cf.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sc.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gb.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ch.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://cl.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://ai.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kv.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jb.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tx.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://bo.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hx.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://hf.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sy.szsharing.cn

[J06] 计算两时间之差
来源：http://jg.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://wy.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://gw.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nh.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nr.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ob.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://yr.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://yl.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://ih.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://tm.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://kp.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wx.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dq.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kk.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://md.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sn.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://es.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://eq.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://ez.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hx.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qe.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mc.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cy.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ec.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rn.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zi.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zz.shtwfgs.cn

[J09] 时区处理
来源：http://kc.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://br.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rb.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://in.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zt.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dj.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tx.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dy.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bo.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://hg.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jr.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wy.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ie.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wo.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bj.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yd.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://br.newstarts.cn

================================================================================
来源：http://ma.yuntaijiaju.cn

K. JSON 与序列化
来源：http://tu.szxytkj.cn

================================================================================
来源：http://ph.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://fy.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ob.colortex.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://je.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://hw.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://cq.szxytkj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tq.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://id.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zi.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nm.lnxyls.cn


<!-- 参考信息 -->