代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hp.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://gj.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://qh.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://lg.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jb.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://dn.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://fb.jctech888.com.cn

[G13] 判断对象类型
来源：http://jw.colortex.cn

Py:   isinstance(u, User)
来源：http://io.panjiajie.cn

PHP:  $u instanceof User
来源：http://rz.nszjky.cn

JS:   u instanceof User
来源：http://wh.huanxung.cn

TS:   u instanceof User
来源：http://uk.lnxyls.cn

Java: u instanceof User
来源：http://lf.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vn.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://ic.asd995.cn

C#:   u is User
来源：http://vg.shtwfgs.cn

[G14] 数据类 / record
来源：http://nn.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wp.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://gi.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yi.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://ac.hahajie.cn

Java: record User(String name, int age) {}
来源：http://vo.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://cn.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mp.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://cm.shtwfgs.cn

[G15] 枚举
来源：http://ax.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ys.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sa.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ol.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jz.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://oj.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gi.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://io.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uf.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://op.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ws.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://vm.hnjuh.cn

JS:   Object.entries(obj)
来源：http://ee.nszjky.cn

TS:   Object.entries(obj)
来源：http://ni.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rt.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pi.nszjky.cn

Ruby: obj.instance_variables
来源：http://xy.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://mw.hnjuh.cn

================================================================================
来源：http://as.jctech888.com.cn

H. 异常与错误处理
来源：http://uv.jianghongdianzi.cn

================================================================================
来源：http://rm.huanxung.cn

[H01] try / catch 基础
来源：http://pv.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://co.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nr.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://be.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hl.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ba.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wf.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pa.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qo.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://bd.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://un.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nu.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zz.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uy.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fp.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ol.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wv.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tz.hahajie.cn

[H03] 主动抛出异常
来源：http://sp.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://yb.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zs.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://fl.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://zu.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hl.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://er.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xu.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fz.colortex.cn

[H04] 自定义异常类型
来源：http://tn.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://rj.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cl.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://up.newstarts.cn

TS:   class MyError extends Error {}
来源：http://xy.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://bh.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ld.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://vr.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://dg.shxzskj.cn

[H05] 捕获特定类型
来源：http://nu.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://lr.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sn.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://vr.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://zd.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://wg.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wy.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://lx.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kk.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://wj.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://lv.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zz.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hn.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ta.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vq.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vv.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://sb.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://hg.shxzukj.cn

[H07] 断言
来源：http://gg.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://az.newstarts.cn

PHP:  assert($x > 0);
来源：http://zp.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://wn.9csxet.cn

TS:   console.assert(x > 0);
来源：http://fe.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://vc.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bh.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ux.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://sh.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://tu.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://su.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mc.colortex.cn

JS:   e.message;  e.stack
来源：http://av.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ov.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qr.shxzskj.cn

Go:   err.Error()
来源：http://io.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://uo.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://jx.9csxet.cn

[H09] 带错误码的异常
来源：http://qo.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kt.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://js.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wq.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wv.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dj.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qc.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xv.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tm.shtwfgs.cn

[H10] 资源自动释放
来源：http://dk.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pu.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://su.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bp.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lq.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rs.521024.cn

Go:   defer f.Close()
来源：http://gu.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fw.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://me.nicolike.cn

================================================================================
来源：http://hm.wgjwhj.cn

I. 正则表达式
来源：http://ze.shxzukj.cn

================================================================================
来源：http://gl.panjiajie.cn

[I01] 判断是否匹配
来源：http://dy.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lv.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://br.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://oz.newstarts.cn

TS:   /\d+/.test(s)
来源：http://tv.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hw.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sy.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://mi.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lb.hnjuh.cn

[I02] 提取所有匹配
来源：http://am.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://ub.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cw.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nz.colortex.cn

TS:   s.match(/\d+/g)
来源：http://fu.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kq.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yv.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://sh.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jp.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://fe.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pm.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ro.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gd.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ll.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ef.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://im.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ie.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mv.shxzukj.cn

[I04] 正则替换
来源：http://fi.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wz.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vs.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fr.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cn.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wn.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bu.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cg.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ls.nszjky.cn

[I05] 按正则拆分
来源：http://km.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jf.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ih.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://mi.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ob.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://qc.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gh.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gv.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hh.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sr.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ta.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ek.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xl.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cq.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zl.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ta.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nc.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ax.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://mu.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vr.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lp.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fj.szsharing.cn

TS:   /error/gim
来源：http://kq.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lh.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://px.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://gc.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dd.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://no.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yo.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hh.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ml.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ws.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cm.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yp.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://be.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kh.shxzukj.cn

================================================================================
来源：http://ne.shxzukj.cn

J. 日期与时间
来源：http://ja.yuexingan06.cn

================================================================================
来源：http://fx.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://md.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hh.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ve.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://up.521024.cn

TS:   new Date();  Date.now()
来源：http://eo.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kv.shxzskj.cn

Go:   time.Now()
来源：http://cz.nicolike.cn

Ruby: Time.now
来源：http://tr.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://se.bookmarksfly.cn

[J02] 格式化输出
来源：http://bt.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sp.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ka.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zc.panjiajie.cn

TS:   d.toISOString()
来源：http://bd.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pv.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ht.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bj.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://in.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://bj.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kx.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gp.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://pl.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://gt.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ke.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://km.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://lp.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hn.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://cc.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ro.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zk.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dw.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zn.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://il.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uh.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yy.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cm.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://vb.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://uc.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qb.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eb.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jh.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://uu.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pa.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://uy.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jb.huixiangedu.cn

[J06] 计算两时间之差
来源：http://bn.jianghongdianzi.cn

Py:   (end - start).total_seconds()
来源：http://an.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://pg.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hi.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gz.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sq.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://va.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://jf.521024.cn

C#:   (end - start).TotalSeconds
来源：http://vb.hahajie.cn

[J07] 比较两个日期
来源：http://nw.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ig.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zp.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hn.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://us.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kv.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ti.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://in.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://lc.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://un.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xh.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ol.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cb.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cr.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ps.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zt.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xx.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yt.huanxung.cn

[J09] 时区处理
来源：http://so.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pg.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cz.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wu.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ue.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ur.panjiajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bp.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yo.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jn.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://qo.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pa.hnjuh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ho.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bm.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bg.asd995.cn


<!-- 参考信息 -->