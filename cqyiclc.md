代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://sp.nicolike.cn

JS:   toString() { return this.name; }
来源：http://si.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://pv.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://ud.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kk.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://pp.colortex.cn

C#:   public override string ToString() => Name;
来源：http://cx.szsharing.cn

[G13] 判断对象类型
来源：http://jw.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://im.nszjky.cn

PHP:  $u instanceof User
来源：http://fs.jctech888.com.cn

JS:   u instanceof User
来源：http://pe.chemitech.net.cn

TS:   u instanceof User
来源：http://gd.bookmarksfly.cn

Java: u instanceof User
来源：http://ip.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tz.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://fg.muxihuayi.cn

C#:   u is User
来源：http://fb.shtwfgs.cn

[G14] 数据类 / record
来源：http://pu.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xg.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://hg.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qn.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://kc.newstarts.cn

Java: record User(String name, int age) {}
来源：http://fx.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://zk.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vd.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://bn.wgjwhj.cn

[G15] 枚举
来源：http://jy.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bi.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wk.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bu.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://by.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://hh.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rt.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://kp.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ug.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://ek.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dt.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://ga.shxzukj.cn

JS:   Object.entries(obj)
来源：http://pl.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://tt.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pl.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://el.shxzukj.cn

Ruby: obj.instance_variables
来源：http://qz.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://qn.colortex.cn

================================================================================
来源：http://bt.yuexingan06.cn

H. 异常与错误处理
来源：http://ls.shtwfgs.cn

================================================================================
来源：http://qt.jctech888.com.cn

[H01] try / catch 基础
来源：http://xy.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://if.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dx.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rm.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hr.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ie.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vg.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mj.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://px.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://xg.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rp.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uz.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pz.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zs.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eb.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qc.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lr.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jd.shxzskj.cn

[H03] 主动抛出异常
来源：http://vt.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://fe.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xv.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://pt.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://js.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oq.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fl.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ac.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kp.lnxyls.cn

[H04] 自定义异常类型
来源：http://np.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://ct.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pb.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://sz.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://ha.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://ab.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vg.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://rw.9csxet.cn

C#:   class MyException : Exception {}
来源：http://gv.yuexingan06.cn

[H05] 捕获特定类型
来源：http://as.jctech888.com.cn

Py:   except ValueError as e:
来源：http://md.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://su.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://jq.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://hm.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://lh.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lx.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://ol.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cn.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://wy.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://qh.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://au.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mr.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://le.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ve.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dz.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://ih.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://xv.9csxet.cn

[H07] 断言
来源：http://rb.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://zs.huanxung.cn

PHP:  assert($x > 0);
来源：http://ay.szsharing.cn

JS:   console.assert(x > 0);
来源：http://jv.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://np.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://gd.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kl.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vp.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://yg.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://pp.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://gn.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vu.hnjuh.cn

JS:   e.message;  e.stack
来源：http://rk.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xj.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://va.huixiangedu.cn

Go:   err.Error()
来源：http://vo.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://yh.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://bt.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://lv.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wi.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pq.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ma.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nz.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hn.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://br.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ie.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nm.hahajie.cn

[H10] 资源自动释放
来源：http://hb.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kp.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zf.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bk.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sd.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ud.hnjuh.cn

Go:   defer f.Close()
来源：http://ss.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bb.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kr.hnjuh.cn

================================================================================
来源：http://jm.9csxet.cn

I. 正则表达式
来源：http://ns.wgjwhj.cn

================================================================================
来源：http://xg.521024.cn

[I01] 判断是否匹配
来源：http://eq.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zd.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wz.asd995.cn

JS:   /\d+/.test(s)
来源：http://bn.asd995.cn

TS:   /\d+/.test(s)
来源：http://gh.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://we.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vf.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://sv.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qz.newstarts.cn

[I02] 提取所有匹配
来源：http://fx.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://ay.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fd.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ic.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://pr.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fv.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mz.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://py.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cw.asd995.cn

[I03] 提取捕获分组
来源：http://cw.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zf.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dj.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://li.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vc.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fd.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ok.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ba.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iw.muxihuayi.cn

[I04] 正则替换
来源：http://jx.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ql.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://za.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pt.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vd.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lw.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://le.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vz.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ts.bjjhwx.cn

[I05] 按正则拆分
来源：http://le.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://eb.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fy.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://vp.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://pe.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://cd.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zu.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pl.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rf.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iz.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xe.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yt.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sx.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lt.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oc.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ef.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vh.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bt.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://yr.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rn.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gx.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iy.shxzukj.cn

TS:   /error/gim
来源：http://li.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dm.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ss.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://qs.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bj.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://es.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kn.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qf.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kc.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eo.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ho.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vd.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wj.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sc.huixiangedu.cn

================================================================================
来源：http://qr.jctech888.com.cn

J. 日期与时间
来源：http://ez.bookmarksfly.cn

================================================================================
来源：http://tn.gzmigu.cn

[J01] 获取当前时间
来源：http://dm.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pu.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tt.asd995.cn

JS:   new Date();  Date.now()
来源：http://qq.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://yb.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pk.521024.cn

Go:   time.Now()
来源：http://fr.nszjky.cn

Ruby: Time.now
来源：http://qi.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ko.haigaiapp.cn

[J02] 格式化输出
来源：http://dn.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gy.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wl.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cb.gzmigu.cn

TS:   d.toISOString()
来源：http://re.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://as.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wt.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sq.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oy.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://xo.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://av.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ep.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://ga.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://hg.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pi.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eb.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://ln.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ax.newstarts.cn

[J04] 时间戳与日期互转
来源：http://rc.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bw.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uj.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://im.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hl.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fg.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lf.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vc.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uu.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://xh.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://fu.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jr.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ck.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zd.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://ag.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sb.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://od.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nd.shxzukj.cn

[J06] 计算两时间之差
来源：http://we.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://ki.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://lz.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://in.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rd.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vt.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://ic.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://mx.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://rm.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://kz.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://fx.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sg.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aa.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qs.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lz.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cc.newstarts.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vj.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://zq.hnjuh.cn

[J08] 提取年月日与星期
来源：http://wj.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mg.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cm.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ls.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fv.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lb.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vs.huixiangedu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mh.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://np.yuntaijiaju.cn

[J09] 时区处理
来源：http://ca.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vd.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zx.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gc.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ho.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tz.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gq.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ua.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jw.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://wv.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ze.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xl.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gu.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jj.yuexingan06.cn


<!-- 参考信息 -->