代发 wailian999

Py:   isinstance(u, User)
来源：http://bu.wgjwhj.cn

PHP:  $u instanceof User
来源：http://iv.shxzskj.cn

JS:   u instanceof User
来源：http://sg.nszjky.cn

TS:   u instanceof User
来源：http://ht.jctech888.com.cn

Java: u instanceof User
来源：http://qs.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vj.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://oa.wgjwhj.cn

C#:   u is User
来源：http://df.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://nc.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vz.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://rb.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sn.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://ho.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://rg.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://yp.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vp.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://tc.wgjwhj.cn

[G15] 枚举
来源：http://nc.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aq.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rn.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iv.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kb.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://xy.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mm.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://lk.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ek.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://iy.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hr.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://vr.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://lm.huanxung.cn

TS:   Object.entries(obj)
来源：http://gd.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wb.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mk.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://ak.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://cm.shxzskj.cn

================================================================================
来源：http://py.yuntaijiaju.cn

H. 异常与错误处理
来源：http://nh.huixinmuqiang.cn

================================================================================
来源：http://lz.lnxyls.cn

[H01] try / catch 基础
来源：http://ct.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oc.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uh.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cc.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gq.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ww.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jx.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jd.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mt.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://rz.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eb.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nm.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bg.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mq.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yr.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://no.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xv.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tr.gzmigu.cn

[H03] 主动抛出异常
来源：http://tz.521024.cn

Py:   raise ValueError("错误信息")
来源：http://vu.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nz.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://tz.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://hm.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nk.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ul.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oh.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ng.asd995.cn

[H04] 自定义异常类型
来源：http://hs.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://tf.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://im.asd995.cn

JS:   class MyError extends Error {}
来源：http://ql.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ks.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://jk.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dm.521024.cn

Ruby: class MyError < StandardError; end
来源：http://ah.9csxet.cn

C#:   class MyException : Exception {}
来源：http://iw.haigaiapp.cn

[H05] 捕获特定类型
来源：http://ig.chemitech.net.cn

Py:   except ValueError as e:
来源：http://ua.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tk.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://ya.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ao.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://rn.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://du.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://bt.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://na.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://cw.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://jl.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ql.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zy.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ln.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yd.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wl.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://vr.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://lh.panjiajie.cn

[H07] 断言
来源：http://lk.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://gr.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://yf.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://qm.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://mg.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://ki.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dt.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mn.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://oc.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://fu.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://dm.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bl.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://hp.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rd.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yw.yuexingan06.cn

Go:   err.Error()
来源：http://kn.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://ur.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://ca.szsharing.cn

[H09] 带错误码的异常
来源：http://yd.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lu.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cu.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sm.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rh.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fj.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tk.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oh.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dt.nszjky.cn

[H10] 资源自动释放
来源：http://ve.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fy.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ub.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gt.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sp.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sh.panjiajie.cn

Go:   defer f.Close()
来源：http://ab.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dh.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xf.hahajie.cn

================================================================================
来源：http://qt.gzmigu.cn

I. 正则表达式
来源：http://bd.huanxung.cn

================================================================================
来源：http://xt.szsharing.cn

[I01] 判断是否匹配
来源：http://de.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ov.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://he.nszjky.cn

JS:   /\d+/.test(s)
来源：http://ft.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://ls.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yw.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sc.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://xt.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zy.asd995.cn

[I02] 提取所有匹配
来源：http://wz.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://fq.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://in.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sq.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://vx.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dm.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zl.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://ij.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uk.huixiangedu.cn

[I03] 提取捕获分组
来源：http://dn.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qx.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ys.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xt.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xx.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lx.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fw.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pl.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://le.shtwfgs.cn

[I04] 正则替换
来源：http://xm.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qz.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wx.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ba.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lk.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ek.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lc.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://le.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yn.asd995.cn

[I05] 按正则拆分
来源：http://oj.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sg.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oi.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://is.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://rg.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://uf.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rf.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tt.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tj.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yx.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ck.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lu.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qt.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fq.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ge.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fa.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kk.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dq.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://lp.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ee.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://af.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fd.nicolike.cn

TS:   /error/gim
来源：http://ix.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bg.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sc.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://og.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zi.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://us.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://db.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sz.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wf.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gi.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ow.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://no.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ge.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ty.nicolike.cn

================================================================================
来源：http://vi.huanxung.cn

J. 日期与时间
来源：http://lz.szsharing.cn

================================================================================
来源：http://hy.gzmigu.cn

[J01] 获取当前时间
来源：http://va.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qf.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://ui.nicolike.cn

TS:   new Date();  Date.now()
来源：http://qh.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vm.szxytkj.cn

Go:   time.Now()
来源：http://sx.panjiajie.cn

Ruby: Time.now
来源：http://rk.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mz.jianghongdianzi.cn

[J02] 格式化输出
来源：http://ml.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tt.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rm.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sk.yuexingan06.cn

TS:   d.toISOString()
来源：http://qs.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mh.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qo.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eh.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bp.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://oi.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kd.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://og.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://hf.colortex.cn

TS:   new Date("2024-01-02")
来源：http://rx.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zj.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kc.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://xm.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pt.newstarts.cn

[J04] 时间戳与日期互转
来源：http://yy.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pm.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jx.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rs.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qv.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yk.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ox.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oz.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hi.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://wh.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://fw.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yg.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aq.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ur.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://rt.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qe.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://fr.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nk.shxzukj.cn

[J06] 计算两时间之差
来源：http://hh.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://zl.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://vg.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mo.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ud.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ma.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://ig.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://xh.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://vi.gzmigu.cn

[J07] 比较两个日期
来源：http://sr.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://yp.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pg.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://az.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zk.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ao.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wh.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oy.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://rs.9csxet.cn

[J08] 提取年月日与星期
来源：http://hj.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lj.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wb.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://df.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://te.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kk.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ip.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ot.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lu.lnxyls.cn

[J09] 时区处理
来源：http://ut.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gx.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ft.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qa.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xz.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://er.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nd.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qe.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ka.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://io.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mq.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zh.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hb.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://re.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vs.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zl.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ct.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dr.asd995.cn

================================================================================
来源：http://zf.muxihuayi.cn

K. JSON 与序列化
来源：http://vm.yuexingan06.cn

================================================================================
来源：http://ed.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://bh.bjjhwx.cn


<!-- 参考信息 -->