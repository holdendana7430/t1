代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://tp.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://lx.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://sd.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cs.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://rk.gzmigu.cn

[G15] 枚举
来源：http://aq.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zz.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tg.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://at.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bn.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://qb.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ya.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://gt.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wt.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://ro.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jn.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://wh.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://gl.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://wx.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ls.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gu.lnxyls.cn

Ruby: obj.instance_variables
来源：http://vq.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://je.colortex.cn

================================================================================
来源：http://zh.wgjwhj.cn

H. 异常与错误处理
来源：http://px.muxihuayi.cn

================================================================================
来源：http://fp.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://ui.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nb.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ip.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kt.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fu.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ud.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gd.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qv.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://go.colortex.cn

[H02] finally / ensure 收尾
来源：http://xv.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qg.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nt.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sk.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qq.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hq.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wi.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gn.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ka.shxzskj.cn

[H03] 主动抛出异常
来源：http://rj.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://fo.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wa.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://je.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://sl.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://om.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tm.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://si.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hf.nicolike.cn

[H04] 自定义异常类型
来源：http://fu.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://il.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://db.huanxung.cn

JS:   class MyError extends Error {}
来源：http://dk.521024.cn

TS:   class MyError extends Error {}
来源：http://fg.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://sv.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vz.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://fz.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://st.yuexingan06.cn

[H05] 捕获特定类型
来源：http://pk.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://pj.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dt.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://mm.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://nm.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://nr.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nu.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://yg.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lu.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://is.colortex.cn

Py:   value = d.get("k") or default
来源：http://mo.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fw.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rk.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lc.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sl.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bm.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://qj.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://da.jianghongdianzi.cn

[H07] 断言
来源：http://iz.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://qa.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://if.hahajie.cn

JS:   console.assert(x > 0);
来源：http://vt.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://ed.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://hp.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ti.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ch.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://tx.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://vq.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://gv.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zq.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://ce.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sj.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rl.wgjwhj.cn

Go:   err.Error()
来源：http://rr.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://qc.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://ff.521024.cn

[H09] 带错误码的异常
来源：http://gz.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zf.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bv.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uq.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wr.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bb.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fq.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mc.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://li.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://dw.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ky.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://px.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qy.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ji.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vv.haigaiapp.cn

Go:   defer f.Close()
来源：http://hl.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kv.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://od.huixinmuqiang.cn

================================================================================
来源：http://ee.newstarts.cn

I. 正则表达式
来源：http://xc.521024.cn

================================================================================
来源：http://cj.521024.cn

[I01] 判断是否匹配
来源：http://ga.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ar.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eh.hahajie.cn

JS:   /\d+/.test(s)
来源：http://vs.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ww.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jq.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kq.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://qx.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ro.521024.cn

[I02] 提取所有匹配
来源：http://oq.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://pu.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kf.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://og.521024.cn

TS:   s.match(/\d+/g)
来源：http://lc.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://es.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bc.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://hu.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yu.colortex.cn

[I03] 提取捕获分组
来源：http://yi.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vf.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://im.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ow.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aj.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mq.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ku.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://be.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gt.szxytkj.cn

[I04] 正则替换
来源：http://yl.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://go.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uc.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xc.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mi.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ag.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uz.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xn.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ld.shtwfgs.cn

[I05] 按正则拆分
来源：http://dp.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qe.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yp.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://in.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://zw.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ko.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bo.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vh.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nq.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ya.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hl.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dg.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lt.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://on.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xd.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://io.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zr.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bi.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://mg.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oq.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uy.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sd.huanxung.cn

TS:   /error/gim
来源：http://tl.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rv.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ll.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://pk.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sl.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://xc.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zy.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lj.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pp.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ry.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kz.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jd.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sd.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ad.nszjky.cn

================================================================================
来源：http://qm.chemitech.net.cn

J. 日期与时间
来源：http://yk.panjiajie.cn

================================================================================
来源：http://jt.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://ca.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wu.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dn.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://mm.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://hq.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ad.shxzskj.cn

Go:   time.Now()
来源：http://lw.shtwfgs.cn

Ruby: Time.now
来源：http://jy.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wg.yuntaijiaju.cn

[J02] 格式化输出
来源：http://xs.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cv.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kz.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dl.9csxet.cn

TS:   d.toISOString()
来源：http://sr.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fp.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gg.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jc.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cf.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://dt.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vk.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bf.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://ik.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://ls.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dy.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tm.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://va.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hb.huanxung.cn

[J04] 时间戳与日期互转
来源：http://or.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vn.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ce.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iu.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://in.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iu.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://al.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://af.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aj.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://ag.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://uw.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nq.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qw.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lu.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ru.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sf.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://rg.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rf.shxzskj.cn

[J06] 计算两时间之差
来源：http://uz.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://yq.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://sz.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://go.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nj.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gr.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://rg.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://tl.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://ci.nicolike.cn

[J07] 比较两个日期
来源：http://dh.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://yh.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vy.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oc.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://so.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ou.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xg.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sb.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://kh.huanxung.cn

[J08] 提取年月日与星期
来源：http://bk.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ba.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dd.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oh.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cy.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mh.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ut.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lv.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wl.panjiajie.cn

[J09] 时区处理
来源：http://aj.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://at.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pn.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iz.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ep.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ju.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xb.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pc.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kg.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://sg.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qx.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ie.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fz.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eu.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ni.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pl.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bg.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gj.gzmigu.cn

================================================================================
来源：http://rp.gzmigu.cn

K. JSON 与序列化
来源：http://iz.huanxung.cn

================================================================================
来源：http://vr.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://kq.szsharing.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nk.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dv.yuexingan06.cn

JS:   JSON.stringify(obj)
来源：http://fz.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://iy.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sb.haigaiapp.cn

Go:   json.Marshal(obj)
来源：http://ql.shtwfgs.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mt.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pz.hahajie.cn

[K02] JSON 字符串转对象
来源：http://ku.nszjky.cn

Py:   json.loads(s)
来源：http://by.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mw.lnxyls.cn

JS:   JSON.parse(s)
来源：http://oh.szxytkj.cn


<!-- 参考信息 -->