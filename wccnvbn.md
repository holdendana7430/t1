代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://dz.nicolike.cn

Java: record User(String name, int age) {}
来源：http://zn.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://af.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nv.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://so.521024.cn

[G15] 枚举
来源：http://ky.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gl.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://or.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hm.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://be.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://ib.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lj.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://ri.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vz.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://ur.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uf.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://sq.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://ek.hnjuh.cn

TS:   Object.entries(obj)
来源：http://fw.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rp.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ec.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://hn.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://qv.huixiangedu.cn

================================================================================
来源：http://ll.bjjhwx.cn

H. 异常与错误处理
来源：http://ih.bjjhwx.cn

================================================================================
来源：http://tq.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://fc.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mb.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://af.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://te.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ne.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://re.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fx.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vy.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kf.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://xd.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ji.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://td.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wr.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pi.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oz.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rh.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gy.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ji.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://qz.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://uk.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ve.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://mc.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://ud.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tb.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jc.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kf.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pa.bjjhwx.cn

[H04] 自定义异常类型
来源：http://dx.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://ju.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qt.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://bx.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://xg.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://sq.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fr.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://va.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://nk.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://is.shtwfgs.cn

Py:   except ValueError as e:
来源：http://dg.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zg.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://bn.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://td.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://jz.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qx.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://nc.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kb.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://ef.colortex.cn

Py:   value = d.get("k") or default
来源：http://xl.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gb.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dz.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mf.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pc.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pg.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://kc.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://kk.gzmigu.cn

[H07] 断言
来源：http://iw.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://hi.shxzukj.cn

PHP:  assert($x > 0);
来源：http://nf.nicolike.cn

JS:   console.assert(x > 0);
来源：http://hw.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://sb.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://nd.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ig.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qf.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://bo.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://bl.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://mn.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qj.9csxet.cn

JS:   e.message;  e.stack
来源：http://wy.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nt.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eu.haigaiapp.cn

Go:   err.Error()
来源：http://gc.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://vz.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://em.hnjuh.cn

[H09] 带错误码的异常
来源：http://ls.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hd.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hg.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tm.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yl.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pi.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://os.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vo.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vb.nicolike.cn

[H10] 资源自动释放
来源：http://lj.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ol.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kk.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yt.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dc.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dh.newstarts.cn

Go:   defer f.Close()
来源：http://os.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ro.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ca.bookmarksfly.cn

================================================================================
来源：http://td.hahajie.cn

I. 正则表达式
来源：http://vk.9csxet.cn

================================================================================
来源：http://do.bjjhwx.cn

[I01] 判断是否匹配
来源：http://eg.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ny.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nr.newstarts.cn

JS:   /\d+/.test(s)
来源：http://iw.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://my.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cv.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wf.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://so.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eu.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://hu.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://br.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kx.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zj.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://np.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vp.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zl.521024.cn

Ruby: s.scan(/\d+/)
来源：http://jd.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://if.bjjhwx.cn

[I03] 提取捕获分组
来源：http://ja.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uu.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yg.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ea.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uw.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sy.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cr.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pj.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hc.muxihuayi.cn

[I04] 正则替换
来源：http://gc.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sh.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hm.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ts.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rb.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yb.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ht.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lo.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pz.huanxung.cn

[I05] 按正则拆分
来源：http://dk.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bf.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rm.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://jz.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ez.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://jd.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jz.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vz.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zv.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bf.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uj.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fe.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://in.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uv.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://el.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dn.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vv.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gv.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://my.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mv.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://up.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dy.chemitech.net.cn

TS:   /error/gim
来源：http://yu.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ym.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://al.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://ct.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nb.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://vb.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fl.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xv.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gz.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://am.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://an.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lt.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vh.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qu.lnxyls.cn

================================================================================
来源：http://nn.bjjhwx.cn

J. 日期与时间
来源：http://uk.szsharing.cn

================================================================================
来源：http://qs.lnxyls.cn

[J01] 获取当前时间
来源：http://ek.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://un.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lc.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://vv.huanxung.cn

TS:   new Date();  Date.now()
来源：http://mf.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ni.bjjhwx.cn

Go:   time.Now()
来源：http://ki.asd995.cn

Ruby: Time.now
来源：http://kz.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bw.shxzskj.cn

[J02] 格式化输出
来源：http://rv.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ff.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oj.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bw.hahajie.cn

TS:   d.toISOString()
来源：http://ms.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nl.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jk.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jn.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ey.panjiajie.cn

[J03] 字符串解析为日期
来源：http://tz.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ta.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wb.521024.cn

JS:   new Date("2024-01-02")
来源：http://ir.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://pp.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://eu.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lp.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ud.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ly.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://xu.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://br.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vf.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dx.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tr.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uh.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ad.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xg.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mb.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://gj.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://gz.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sx.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fn.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dy.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://ka.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ei.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://vn.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sy.colortex.cn

[J06] 计算两时间之差
来源：http://xw.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://fh.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://xs.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bm.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hy.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ji.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://vm.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://br.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://hp.nicolike.cn

[J07] 比较两个日期
来源：http://ay.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://cc.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gx.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ra.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ux.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cq.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wb.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bd.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://xe.9csxet.cn

[J08] 提取年月日与星期
来源：http://gl.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cm.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qy.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yh.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ld.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mj.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ls.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qy.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kl.nszjky.cn

[J09] 时区处理
来源：http://yf.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://no.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gp.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://um.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fl.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mm.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kz.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vx.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wc.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://ws.huanxung.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cp.wgjwhj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oo.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ob.521024.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gz.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zy.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fs.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kg.newstarts.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://np.shtwfgs.cn

================================================================================
来源：http://er.huixiangedu.cn

K. JSON 与序列化
来源：http://ue.shxzskj.cn

================================================================================
来源：http://bb.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://ul.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ct.lnxyls.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hw.huixinmuqiang.cn

JS:   JSON.stringify(obj)
来源：http://jt.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://hh.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zx.szsharing.cn

Go:   json.Marshal(obj)
来源：http://em.yuntaijiaju.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pd.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bf.szsharing.cn

[K02] JSON 字符串转对象
来源：http://iy.szxytkj.cn

Py:   json.loads(s)
来源：http://vr.shxzskj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rz.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://za.lnxyls.cn


<!-- 参考信息 -->