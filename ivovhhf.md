代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hi.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://xs.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://mh.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://sl.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ma.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://vb.asd995.cn

C#:   public override string ToString() => Name;
来源：http://tt.newstarts.cn

[G13] 判断对象类型
来源：http://ax.nszjky.cn

Py:   isinstance(u, User)
来源：http://xi.jctech888.com.cn

PHP:  $u instanceof User
来源：http://ij.521024.cn

JS:   u instanceof User
来源：http://za.gzmigu.cn

TS:   u instanceof User
来源：http://cs.gzmigu.cn

Java: u instanceof User
来源：http://uq.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eu.nszjky.cn

Ruby: u.is_a?(User)
来源：http://hv.gzmigu.cn

C#:   u is User
来源：http://hr.huanxung.cn

[G14] 数据类 / record
来源：http://de.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ob.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://gh.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bw.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://zs.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://aq.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://yl.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://th.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://ss.9csxet.cn

[G15] 枚举
来源：http://oh.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rh.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nx.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://md.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zd.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://yt.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kx.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://li.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ld.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://rv.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lz.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://zi.colortex.cn

JS:   Object.entries(obj)
来源：http://xc.huanxung.cn

TS:   Object.entries(obj)
来源：http://mf.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://so.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nk.asd995.cn

Ruby: obj.instance_variables
来源：http://bz.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://pi.asd995.cn

================================================================================
来源：http://ou.chemitech.net.cn

H. 异常与错误处理
来源：http://vn.haigaiapp.cn

================================================================================
来源：http://ly.lnxyls.cn

[H01] try / catch 基础
来源：http://fg.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vj.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ce.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pk.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qb.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ha.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hc.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kz.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xh.hahajie.cn

[H02] finally / ensure 收尾
来源：http://se.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pa.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uf.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wk.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://li.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hv.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ym.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://va.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xm.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://ks.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://ih.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sm.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://rx.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://kp.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mb.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wn.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://px.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fy.9csxet.cn

[H04] 自定义异常类型
来源：http://zy.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://bt.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nt.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://bt.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://da.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://zz.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ry.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://as.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://hu.jctech888.com.cn

[H05] 捕获特定类型
来源：http://by.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://aq.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mc.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://mm.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://dv.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://em.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jq.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://yq.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://go.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://gl.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://yw.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://os.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vp.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rc.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mj.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rt.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://oq.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://gv.hnjuh.cn

[H07] 断言
来源：http://dr.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://td.colortex.cn

PHP:  assert($x > 0);
来源：http://ao.colortex.cn

JS:   console.assert(x > 0);
来源：http://se.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://hu.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://vh.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sg.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ip.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://ru.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://ft.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://ll.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pv.521024.cn

JS:   e.message;  e.stack
来源：http://fs.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qq.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://by.wgjwhj.cn

Go:   err.Error()
来源：http://fw.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://rj.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://sf.panjiajie.cn

[H09] 带错误码的异常
来源：http://up.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ip.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nb.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sh.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gy.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gx.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ur.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://km.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ck.hahajie.cn

[H10] 资源自动释放
来源：http://hx.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qn.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xd.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kb.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fr.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qz.shxzukj.cn

Go:   defer f.Close()
来源：http://jy.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tv.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hu.shtwfgs.cn

================================================================================
来源：http://jl.bookmarksfly.cn

I. 正则表达式
来源：http://ok.bjjhwx.cn

================================================================================
来源：http://cc.hahajie.cn

[I01] 判断是否匹配
来源：http://vx.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fu.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xp.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://ju.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://in.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yi.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gk.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://cr.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wu.shtwfgs.cn

[I02] 提取所有匹配
来源：http://ll.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://lx.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://na.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fp.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://de.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yh.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ox.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://wt.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gk.newstarts.cn

[I03] 提取捕获分组
来源：http://yx.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nq.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xf.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uj.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rq.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nm.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uf.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fw.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kb.jctech888.com.cn

[I04] 正则替换
来源：http://wp.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xu.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xv.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cz.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rx.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ad.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pi.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uf.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://da.huanxung.cn

[I05] 按正则拆分
来源：http://al.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bg.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dl.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://bc.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://qn.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://jv.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mt.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dq.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hs.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://to.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lp.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fo.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sf.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ya.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xz.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wa.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gd.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sb.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://aq.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mf.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qa.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qn.521024.cn

TS:   /error/gim
来源：http://ki.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yd.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pi.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://ww.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kt.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://nh.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wl.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yk.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yj.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gb.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ep.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kj.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yo.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qn.panjiajie.cn

================================================================================
来源：http://ws.521024.cn

J. 日期与时间
来源：http://ft.panjiajie.cn

================================================================================
来源：http://kx.panjiajie.cn

[J01] 获取当前时间
来源：http://hz.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mf.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ul.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://gy.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://or.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rc.yuntaijiaju.cn

Go:   time.Now()
来源：http://th.wgjwhj.cn

Ruby: Time.now
来源：http://ez.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yz.szxytkj.cn

[J02] 格式化输出
来源：http://ce.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kh.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jo.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ad.nszjky.cn

TS:   d.toISOString()
来源：http://ms.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ju.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nf.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xz.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ju.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://ym.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rp.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eq.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://so.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://ng.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sc.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://us.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://fz.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cv.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://um.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mo.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jj.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ik.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zf.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pi.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kt.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uk.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fx.521024.cn

[J05] 时间加减（加 7 天）
来源：http://gf.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://we.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kr.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pi.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xx.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ky.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://am.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://ip.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mx.9csxet.cn

[J06] 计算两时间之差
来源：http://jj.asd995.cn

Py:   (end - start).total_seconds()
来源：http://zc.521024.cn

PHP:  $end->diff($start)->days;
来源：http://fx.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ue.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qr.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yt.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://te.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://ih.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://gy.nszjky.cn

[J07] 比较两个日期
来源：http://ud.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://ka.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lr.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xz.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yx.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wx.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sy.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cr.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://gc.521024.cn

[J08] 提取年月日与星期
来源：http://iu.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jx.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xj.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uy.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mj.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://br.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hn.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hk.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sm.huanxung.cn

[J09] 时区处理
来源：http://gv.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ex.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yh.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cx.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mj.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oc.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zc.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bt.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cn.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://cq.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yk.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gh.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wk.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ys.hnjuh.cn


<!-- 参考信息 -->