代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://jt.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://tb.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://wx.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://bl.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wg.asd995.cn

Ruby: def to_s; @name; end
来源：http://kz.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://qk.asd995.cn

[G13] 判断对象类型
来源：http://xu.521024.cn

Py:   isinstance(u, User)
来源：http://qo.nszjky.cn

PHP:  $u instanceof User
来源：http://xx.shxzukj.cn

JS:   u instanceof User
来源：http://hr.asd995.cn

TS:   u instanceof User
来源：http://vi.bookmarksfly.cn

Java: u instanceof User
来源：http://zk.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ov.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://sc.haigaiapp.cn

C#:   u is User
来源：http://ir.huanxung.cn

[G14] 数据类 / record
来源：http://su.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ow.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://tw.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gj.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://xm.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://ai.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://ai.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://je.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://gg.huixinmuqiang.cn

[G15] 枚举
来源：http://jq.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ib.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xk.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zi.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vm.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://zg.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qk.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://iq.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lx.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://lo.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bj.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://fp.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://ii.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://ej.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hp.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://no.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://oh.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://ah.szxytkj.cn

================================================================================
来源：http://ro.szsharing.cn

H. 异常与错误处理
来源：http://aa.huanxung.cn

================================================================================
来源：http://hy.panjiajie.cn

[H01] try / catch 基础
来源：http://uc.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://la.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tb.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kw.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://un.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nr.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uc.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lo.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://at.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://hg.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vq.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mb.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wm.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jt.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vs.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pg.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xf.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qy.521024.cn

[H03] 主动抛出异常
来源：http://rp.521024.cn

Py:   raise ValueError("错误信息")
来源：http://ma.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xe.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://ty.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://yl.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://po.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pm.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dt.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xf.huixiangedu.cn

[H04] 自定义异常类型
来源：http://ju.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://he.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ni.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://pq.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ai.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://qn.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ry.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://em.nicolike.cn

C#:   class MyException : Exception {}
来源：http://mf.szsharing.cn

[H05] 捕获特定类型
来源：http://ml.haigaiapp.cn

Py:   except ValueError as e:
来源：http://rb.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://df.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://vt.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://zb.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://yk.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nk.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://ow.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ie.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://xb.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://ou.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://it.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xm.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ii.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pb.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ps.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://kq.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://sf.hnjuh.cn

[H07] 断言
来源：http://em.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://lr.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://va.newstarts.cn

JS:   console.assert(x > 0);
来源：http://bf.hahajie.cn

TS:   console.assert(x > 0);
来源：http://wx.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ra.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://si.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eq.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://ur.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://kz.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://dh.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zr.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://vs.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xy.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nt.panjiajie.cn

Go:   err.Error()
来源：http://vv.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://dn.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://br.nicolike.cn

[H09] 带错误码的异常
来源：http://eu.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gm.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iz.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hx.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rv.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ab.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cw.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jy.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zf.panjiajie.cn

[H10] 资源自动释放
来源：http://rp.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oz.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tv.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lh.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fk.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dw.hnjuh.cn

Go:   defer f.Close()
来源：http://it.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qs.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fw.hnjuh.cn

================================================================================
来源：http://yc.szxytkj.cn

I. 正则表达式
来源：http://ju.jianghongdianzi.cn

================================================================================
来源：http://oi.chemitech.net.cn

[I01] 判断是否匹配
来源：http://dk.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sq.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vd.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://qn.asd995.cn

TS:   /\d+/.test(s)
来源：http://in.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hp.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cg.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://xq.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://px.newstarts.cn

[I02] 提取所有匹配
来源：http://qr.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://pi.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yi.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ba.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://pv.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xr.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nr.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://xh.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sb.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://hy.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zv.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kz.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zd.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://os.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xu.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xc.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://au.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ab.wgjwhj.cn

[I04] 正则替换
来源：http://wj.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://am.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ww.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rt.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hk.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oe.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ij.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oc.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.panjiajie.cn

[I05] 按正则拆分
来源：http://ar.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fj.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hw.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://nw.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://gt.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://dd.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yc.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jx.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uu.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lk.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ox.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aw.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bp.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qc.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xg.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sp.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://td.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hb.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://pm.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bs.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ks.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://su.colortex.cn

TS:   /error/gim
来源：http://ot.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lv.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hp.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://se.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zv.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://sk.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://so.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hu.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yl.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hn.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bn.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qz.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ni.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eo.yuntaijiaju.cn

================================================================================
来源：http://yk.shxzukj.cn

J. 日期与时间
来源：http://yw.asd995.cn

================================================================================
来源：http://qd.bjjhwx.cn

[J01] 获取当前时间
来源：http://ul.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hn.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aq.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://bh.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://yp.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dp.chemitech.net.cn

Go:   time.Now()
来源：http://ov.9csxet.cn

Ruby: Time.now
来源：http://kr.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ic.newstarts.cn

[J02] 格式化输出
来源：http://ae.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dh.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wp.bookmarksfly.cn

TS:   d.toISOString()
来源：http://ld.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lu.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yg.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ja.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bh.huanxung.cn

[J03] 字符串解析为日期
来源：http://aq.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qv.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ab.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://qb.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://cy.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ng.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rj.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://qj.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fi.szsharing.cn

[J04] 时间戳与日期互转
来源：http://yf.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ph.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pf.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ue.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iu.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oj.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uf.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jz.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lo.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://lg.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://eu.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ay.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ay.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bl.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://aw.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qi.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://dx.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://il.9csxet.cn

[J06] 计算两时间之差
来源：http://ej.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://bp.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://um.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gt.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ks.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xb.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://sq.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://wg.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://xs.521024.cn

[J07] 比较两个日期
来源：http://gu.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://hj.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zn.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://db.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://eg.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zc.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ow.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jm.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://jh.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://hn.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://be.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xs.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://is.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mo.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://id.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hu.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mm.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://in.jctech888.com.cn

[J09] 时区处理
来源：http://cw.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bd.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wk.jctech888.com.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uo.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tg.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mh.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ji.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://re.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bb.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://nn.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rd.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://op.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wp.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://og.bjjhwx.cn


<!-- 参考信息 -->