代发 wailian999

Py:   isinstance(u, User)
来源：http://cj.nicolike.cn

PHP:  $u instanceof User
来源：http://at.colortex.cn

JS:   u instanceof User
来源：http://lh.panjiajie.cn

TS:   u instanceof User
来源：http://uv.chemitech.net.cn

Java: u instanceof User
来源：http://lu.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ap.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://sf.haigaiapp.cn

C#:   u is User
来源：http://av.huixiangedu.cn

[G14] 数据类 / record
来源：http://uo.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xl.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ui.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://si.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://kp.asd995.cn

Java: record User(String name, int age) {}
来源：http://en.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://wv.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ux.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://px.9csxet.cn

[G15] 枚举
来源：http://rb.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vu.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qj.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bz.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://in.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://hh.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kv.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://uc.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jy.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://wn.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gi.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ri.lnxyls.cn

JS:   Object.entries(obj)
来源：http://py.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://yv.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uv.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://el.nszjky.cn

Ruby: obj.instance_variables
来源：http://ug.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://jk.szxytkj.cn

================================================================================
来源：http://bo.nszjky.cn

H. 异常与错误处理
来源：http://mu.huixinmuqiang.cn

================================================================================
来源：http://at.bjjhwx.cn

[H01] try / catch 基础
来源：http://ki.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qq.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yq.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://or.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rj.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vn.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kr.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wx.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ci.521024.cn

[H02] finally / ensure 收尾
来源：http://yf.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jn.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ci.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://se.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cu.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qq.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://to.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dy.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xp.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://ue.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://zv.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gp.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://lt.asd995.cn

TS:   throw new Error("错误信息");
来源：http://vs.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eh.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yc.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hn.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sa.wgjwhj.cn

[H04] 自定义异常类型
来源：http://za.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://vl.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zu.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://zp.asd995.cn

TS:   class MyError extends Error {}
来源：http://jw.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://mc.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://en.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://nw.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://hq.szxytkj.cn

[H05] 捕获特定类型
来源：http://us.521024.cn

Py:   except ValueError as e:
来源：http://ci.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://el.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://nv.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://dl.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://vu.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jz.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://bn.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cr.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://oy.newstarts.cn

Py:   value = d.get("k") or default
来源：http://mn.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ao.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ed.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aa.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bt.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://au.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://hg.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://un.yuexingan06.cn

[H07] 断言
来源：http://eu.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://ho.9csxet.cn

PHP:  assert($x > 0);
来源：http://yb.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://to.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://iv.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://cf.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kp.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nq.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://pi.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://zc.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://on.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://et.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://ia.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kn.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fm.nszjky.cn

Go:   err.Error()
来源：http://kp.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://dc.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://hk.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ar.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bp.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gj.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ql.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kl.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fl.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://se.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wd.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eb.huanxung.cn

[H10] 资源自动释放
来源：http://wm.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lj.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hp.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oe.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xb.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uk.gzmigu.cn

Go:   defer f.Close()
来源：http://fm.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sa.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wl.lnxyls.cn

================================================================================
来源：http://ce.shxzskj.cn

I. 正则表达式
来源：http://pc.panjiajie.cn

================================================================================
来源：http://go.panjiajie.cn

[I01] 判断是否匹配
来源：http://mt.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qq.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lq.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://ho.colortex.cn

TS:   /\d+/.test(s)
来源：http://ec.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ww.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dh.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://qb.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ep.shxzskj.cn

[I02] 提取所有匹配
来源：http://oh.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://dh.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bp.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dw.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://gq.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vq.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wd.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://dm.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://di.muxihuayi.cn

[I03] 提取捕获分组
来源：http://yg.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iq.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://my.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pd.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nt.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://di.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uu.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ip.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kb.bjjhwx.cn

[I04] 正则替换
来源：http://ir.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ct.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kv.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ml.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eh.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gi.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pd.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nj.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eh.gzmigu.cn

[I05] 按正则拆分
来源：http://pv.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fm.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ep.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://nm.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ez.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://xh.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yg.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hu.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gp.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nn.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ez.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gg.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sw.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://km.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lg.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://me.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vu.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ad.521024.cn

[I07] 忽略大小写与多行模式
来源：http://ls.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tw.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ix.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zz.muxihuayi.cn

TS:   /error/gim
来源：http://kx.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kr.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rz.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://kz.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pk.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ub.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yf.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://so.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fl.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://am.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jo.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ae.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ii.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fl.huixiangedu.cn

================================================================================
来源：http://gj.yuexingan06.cn

J. 日期与时间
来源：http://ul.muxihuayi.cn

================================================================================
来源：http://vd.panjiajie.cn

[J01] 获取当前时间
来源：http://vg.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jt.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wi.9csxet.cn

JS:   new Date();  Date.now()
来源：http://qm.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://yg.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ej.haigaiapp.cn

Go:   time.Now()
来源：http://cs.nszjky.cn

Ruby: Time.now
来源：http://eu.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://du.yuntaijiaju.cn

[J02] 格式化输出
来源：http://kc.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vs.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dv.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gv.521024.cn

TS:   d.toISOString()
来源：http://cx.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tv.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ai.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://el.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tk.shxzskj.cn

[J03] 字符串解析为日期
来源：http://wc.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sm.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gj.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://pj.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://uf.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jh.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hf.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ds.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lh.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://km.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qh.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ws.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zi.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ln.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nq.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ki.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jo.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uj.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://ks.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://oq.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wv.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ar.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gx.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://of.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xp.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://rn.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qy.huixiangedu.cn

[J06] 计算两时间之差
来源：http://qn.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://ko.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://ml.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ls.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ev.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cx.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://bp.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://bx.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://oi.szsharing.cn

[J07] 比较两个日期
来源：http://vy.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://mf.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xe.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lu.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qx.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sc.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xs.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wf.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://rc.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://ov.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fl.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fg.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://he.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ql.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yr.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bm.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fd.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cl.jctech888.com.cn

[J09] 时区处理
来源：http://bb.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yl.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hb.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wq.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uo.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gb.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://te.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yf.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ll.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://hd.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://av.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ey.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dg.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gc.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vy.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lj.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tk.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lk.nicolike.cn

================================================================================
来源：http://ss.wgjwhj.cn

K. JSON 与序列化
来源：http://nu.hnjuh.cn

================================================================================
来源：http://nc.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://bq.yuexingan06.cn


<!-- 参考信息 -->