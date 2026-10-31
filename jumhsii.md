代发 wailian999

Py:   isinstance(u, User)
来源：http://pr.9csxet.cn

PHP:  $u instanceof User
来源：http://jz.bjjhwx.cn

JS:   u instanceof User
来源：http://gn.colortex.cn

TS:   u instanceof User
来源：http://eu.szsharing.cn

Java: u instanceof User
来源：http://qf.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iw.newstarts.cn

Ruby: u.is_a?(User)
来源：http://te.shtwfgs.cn

C#:   u is User
来源：http://uf.haigaiapp.cn

[G14] 数据类 / record
来源：http://tf.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sf.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://ll.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xp.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://xo.hahajie.cn

Java: record User(String name, int age) {}
来源：http://zh.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ql.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xl.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://gv.shtwfgs.cn

[G15] 枚举
来源：http://ky.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nn.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yc.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ll.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://es.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://qo.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vx.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://ii.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ym.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://rb.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dl.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://gk.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://uw.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://hk.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cs.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://td.shxzukj.cn

Ruby: obj.instance_variables
来源：http://my.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://bw.shxzukj.cn

================================================================================
来源：http://wj.yuntaijiaju.cn

H. 异常与错误处理
来源：http://uc.hnjuh.cn

================================================================================
来源：http://pn.shtwfgs.cn

[H01] try / catch 基础
来源：http://ev.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wq.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mr.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ep.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cx.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yz.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ug.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xg.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xd.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://lz.shxzskj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dh.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://as.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ir.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hb.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ik.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://au.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hv.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xy.huanxung.cn

[H03] 主动抛出异常
来源：http://ea.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://uf.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ta.colortex.cn

JS:   throw new Error("错误信息");
来源：http://ed.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://rh.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://od.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xk.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ja.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jf.gzmigu.cn

[H04] 自定义异常类型
来源：http://en.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://mk.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://re.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://ze.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://nw.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://bb.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uh.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://yl.colortex.cn

C#:   class MyException : Exception {}
来源：http://tu.nszjky.cn

[H05] 捕获特定类型
来源：http://lm.jctech888.com.cn

Py:   except ValueError as e:
来源：http://dn.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xf.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://lu.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://bg.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://if.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gv.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://sp.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://je.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://wo.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://ke.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bk.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bw.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kw.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ga.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kc.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://ox.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://zf.colortex.cn

[H07] 断言
来源：http://ls.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://em.hahajie.cn

PHP:  assert($x > 0);
来源：http://ty.hahajie.cn

JS:   console.assert(x > 0);
来源：http://ik.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://qp.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://fi.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mb.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gw.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://cs.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://gs.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://it.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gh.nszjky.cn

JS:   e.message;  e.stack
来源：http://su.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jr.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ek.jctech888.com.cn

Go:   err.Error()
来源：http://cz.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://by.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://vl.shtwfgs.cn

[H09] 带错误码的异常
来源：http://gb.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nx.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qk.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://it.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ox.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fx.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://np.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ub.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ri.haigaiapp.cn

[H10] 资源自动释放
来源：http://hs.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gp.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wm.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tx.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vq.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bm.szsharing.cn

Go:   defer f.Close()
来源：http://ms.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aq.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pj.huanxung.cn

================================================================================
来源：http://tx.521024.cn

I. 正则表达式
来源：http://on.wgjwhj.cn

================================================================================
来源：http://tl.haigaiapp.cn

[I01] 判断是否匹配
来源：http://vj.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pp.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jn.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://fo.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://nk.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gx.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bx.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://rc.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qi.nicolike.cn

[I02] 提取所有匹配
来源：http://rm.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://xz.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://en.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ms.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://uc.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://my.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pw.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://rk.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uj.wgjwhj.cn

[I03] 提取捕获分组
来源：http://ob.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ht.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ta.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ql.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jq.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hy.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hh.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pz.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ih.bjjhwx.cn

[I04] 正则替换
来源：http://jl.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cd.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mx.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vb.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://de.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zb.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ar.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jj.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wu.newstarts.cn

[I05] 按正则拆分
来源：http://el.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://id.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vr.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ul.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://du.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://dw.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cn.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jx.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://go.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bx.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kv.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jq.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fz.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://by.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ce.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ed.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ap.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jf.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://kd.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ii.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qe.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zz.jianghongdianzi.cn

TS:   /error/gim
来源：http://pg.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lw.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lf.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://yg.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sn.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://wp.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ou.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hj.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ce.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ev.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tf.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qa.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xd.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aq.shxzukj.cn

================================================================================
来源：http://zx.shxzskj.cn

J. 日期与时间
来源：http://li.huixiangedu.cn

================================================================================
来源：http://xf.521024.cn

[J01] 获取当前时间
来源：http://yu.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tg.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pi.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://cg.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://wv.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zt.panjiajie.cn

Go:   time.Now()
来源：http://xn.haigaiapp.cn

Ruby: Time.now
来源：http://hp.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fu.jianghongdianzi.cn

[J02] 格式化输出
来源：http://vc.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tw.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ms.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pg.9csxet.cn

TS:   d.toISOString()
来源：http://rc.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nd.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pk.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kl.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kk.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://nw.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://os.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eb.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://kn.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://bp.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yf.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hx.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://wn.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fw.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ny.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oz.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ua.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ai.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qi.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ef.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qa.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lu.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ib.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://ea.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://cy.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pu.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nd.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ww.shxzukj.cn

Java: LocalDate.now().plusDays(7)
来源：http://fa.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ft.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://hb.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://md.hahajie.cn

[J06] 计算两时间之差
来源：http://qx.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://mj.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://jo.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bk.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hk.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ns.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://wf.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://yz.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://es.asd995.cn

[J07] 比较两个日期
来源：http://um.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://vl.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://al.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dq.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mo.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xa.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vh.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vm.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://ur.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://ut.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hq.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vh.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zs.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bu.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xc.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ww.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nw.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qc.gzmigu.cn

[J09] 时区处理
来源：http://ro.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bt.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vv.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xd.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pi.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wp.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://um.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ao.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://za.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://qc.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tb.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ww.shtwfgs.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jw.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hi.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://su.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hn.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sl.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dz.panjiajie.cn

================================================================================
来源：http://lq.wgjwhj.cn

K. JSON 与序列化
来源：http://xj.szxytkj.cn

================================================================================
来源：http://ie.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://gn.muxihuayi.cn


<!-- 参考信息 -->