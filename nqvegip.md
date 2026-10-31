代发 wailian999

Py:   isinstance(u, User)
来源：http://sd.szsharing.cn

PHP:  $u instanceof User
来源：http://or.panjiajie.cn

JS:   u instanceof User
来源：http://ht.newstarts.cn

TS:   u instanceof User
来源：http://ko.jctech888.com.cn

Java: u instanceof User
来源：http://yt.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bq.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://fv.nszjky.cn

C#:   u is User
来源：http://nq.bookmarksfly.cn

[G14] 数据类 / record
来源：http://gb.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://km.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://fc.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ye.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://bp.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://zz.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://kz.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://te.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://pm.lnxyls.cn

[G15] 枚举
来源：http://mn.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ao.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rt.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ga.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://na.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://fn.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xe.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://rx.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rx.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://ll.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mp.asd995.cn

PHP:  get_object_vars($obj);
来源：http://ro.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://yp.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://yb.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://la.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://js.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://zk.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ih.wgjwhj.cn

================================================================================
来源：http://yr.shxzskj.cn

H. 异常与错误处理
来源：http://jh.9csxet.cn

================================================================================
来源：http://gv.yuexingan06.cn

[H01] try / catch 基础
来源：http://fr.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kg.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ig.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yg.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ml.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jo.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ae.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uy.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ly.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://gf.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://du.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xc.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pb.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ft.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wp.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uu.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fc.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tn.szsharing.cn

[H03] 主动抛出异常
来源：http://ia.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://tw.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pt.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://xi.521024.cn

TS:   throw new Error("错误信息");
来源：http://gx.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jw.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rz.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ru.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xc.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://we.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://ty.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://os.szsharing.cn

JS:   class MyError extends Error {}
来源：http://ym.colortex.cn

TS:   class MyError extends Error {}
来源：http://lq.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://ou.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hk.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://pi.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://ye.hnjuh.cn

[H05] 捕获特定类型
来源：http://qj.521024.cn

Py:   except ValueError as e:
来源：http://vr.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rz.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://qo.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://sy.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://iw.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nn.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://nf.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xa.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://co.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://kf.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yc.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jt.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mt.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rt.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rv.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://uu.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://vi.wgjwhj.cn

[H07] 断言
来源：http://tj.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://qe.colortex.cn

PHP:  assert($x > 0);
来源：http://mc.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ii.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://ls.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://cc.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dn.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cr.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://kx.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://yx.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://go.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jr.huanxung.cn

JS:   e.message;  e.stack
来源：http://hi.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zf.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fh.shtwfgs.cn

Go:   err.Error()
来源：http://bf.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://lw.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://xr.9csxet.cn

[H09] 带错误码的异常
来源：http://zw.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ff.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zj.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kx.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kn.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vm.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vh.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sm.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fh.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://mp.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://at.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xg.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pm.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://my.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://up.szxytkj.cn

Go:   defer f.Close()
来源：http://yi.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ov.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rx.panjiajie.cn

================================================================================
来源：http://cw.jianghongdianzi.cn

I. 正则表达式
来源：http://gr.lnxyls.cn

================================================================================
来源：http://qe.shxzukj.cn

[I01] 判断是否匹配
来源：http://rd.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zh.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gi.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://tk.huanxung.cn

TS:   /\d+/.test(s)
来源：http://ac.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wy.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lf.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://gq.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nm.szxytkj.cn

[I02] 提取所有匹配
来源：http://oo.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://le.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gc.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qb.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://rk.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sr.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qb.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://pn.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gk.huanxung.cn

[I03] 提取捕获分组
来源：http://bv.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://si.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rn.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dd.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ot.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lf.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ih.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rh.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ip.yuexingan06.cn

[I04] 正则替换
来源：http://bx.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gz.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vc.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uo.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bv.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ew.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gm.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gt.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pt.szsharing.cn

[I05] 按正则拆分
来源：http://jy.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dw.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://en.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://ri.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://cb.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://kv.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aw.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ep.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bz.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ni.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xv.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qd.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ql.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gq.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fx.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://et.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bt.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zx.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://af.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bc.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fe.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pq.szxytkj.cn

TS:   /error/gim
来源：http://wz.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ic.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sf.colortex.cn

Ruby: s.scan(/error/i)
来源：http://rg.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ef.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://zt.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://in.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gj.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://di.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cd.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xj.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gq.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kb.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hk.wgjwhj.cn

================================================================================
来源：http://ed.huixiangedu.cn

J. 日期与时间
来源：http://qt.huixinmuqiang.cn

================================================================================
来源：http://pa.muxihuayi.cn

[J01] 获取当前时间
来源：http://rv.shxzukj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fs.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bb.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://ed.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://wg.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vc.yuexingan06.cn

Go:   time.Now()
来源：http://hv.yuexingan06.cn

Ruby: Time.now
来源：http://fo.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ln.hnjuh.cn

[J02] 格式化输出
来源：http://il.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kd.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eo.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ju.9csxet.cn

TS:   d.toISOString()
来源：http://qa.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wk.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ic.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gc.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qd.nicolike.cn

[J03] 字符串解析为日期
来源：http://bj.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://un.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mr.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://qf.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://bd.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nm.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zw.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://pj.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bd.huanxung.cn

[J04] 时间戳与日期互转
来源：http://zq.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sx.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://id.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ip.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zt.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oh.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yl.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hl.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ju.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://as.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://hw.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://id.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cl.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pn.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://pb.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cr.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://dn.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xd.9csxet.cn

[J06] 计算两时间之差
来源：http://pf.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://xl.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://wi.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bo.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jy.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ds.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://cq.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://hq.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://yf.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://ge.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://qq.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hk.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iw.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bj.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ox.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sf.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oj.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://qc.colortex.cn

[J08] 提取年月日与星期
来源：http://mg.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aq.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://si.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vz.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xc.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://td.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mc.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ki.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uj.hahajie.cn

[J09] 时区处理
来源：http://ee.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ve.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xk.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qg.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mk.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jb.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fk.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sb.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ko.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://lo.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ka.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qc.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hn.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://de.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bl.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rs.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hs.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rr.szsharing.cn

================================================================================
来源：http://nm.hnjuh.cn

K. JSON 与序列化
来源：http://up.szsharing.cn

================================================================================
来源：http://vg.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://mw.gzmigu.cn


<!-- 参考信息 -->