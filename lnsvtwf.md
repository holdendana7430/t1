代发 wailian999

Ruby: attr_accessor :name
来源：http://tg.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://pk.newstarts.cn

[G12] 对象转字符串
来源：http://bl.colortex.cn

Py:   def __str__(self): return self.name
来源：http://bu.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cq.hahajie.cn

JS:   toString() { return this.name; }
来源：http://uz.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://lo.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://hm.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fr.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://jk.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://fq.lnxyls.cn

[G13] 判断对象类型
来源：http://lx.521024.cn

Py:   isinstance(u, User)
来源：http://bc.hnjuh.cn

PHP:  $u instanceof User
来源：http://za.lnxyls.cn

JS:   u instanceof User
来源：http://ik.nszjky.cn

TS:   u instanceof User
来源：http://ga.hahajie.cn

Java: u instanceof User
来源：http://pr.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jm.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://lh.szsharing.cn

C#:   u is User
来源：http://tm.yuexingan06.cn

[G14] 数据类 / record
来源：http://ks.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gt.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://em.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rz.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://js.521024.cn

Java: record User(String name, int age) {}
来源：http://hn.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://rs.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kq.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://ub.521024.cn

[G15] 枚举
来源：http://iw.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zq.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vy.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://au.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wn.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://ah.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pj.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://yy.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vr.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://np.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ml.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://fw.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://is.szsharing.cn

TS:   Object.entries(obj)
来源：http://xt.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yi.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://je.hnjuh.cn

Ruby: obj.instance_variables
来源：http://cu.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://nx.hahajie.cn

================================================================================
来源：http://vb.newstarts.cn

H. 异常与错误处理
来源：http://fj.yuexingan06.cn

================================================================================
来源：http://sx.9csxet.cn

[H01] try / catch 基础
来源：http://gy.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pc.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tc.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ff.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gk.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rn.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bu.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jc.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sz.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://oa.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jv.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ng.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cl.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mw.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yl.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eo.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hn.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yl.haigaiapp.cn

[H03] 主动抛出异常
来源：http://dw.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://bo.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dl.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://cx.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://hy.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tp.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://db.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pj.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ly.9csxet.cn

[H04] 自定义异常类型
来源：http://fu.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://if.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ql.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://ir.huanxung.cn

TS:   class MyError extends Error {}
来源：http://as.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://hc.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kg.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://xh.asd995.cn

C#:   class MyException : Exception {}
来源：http://bm.hnjuh.cn

[H05] 捕获特定类型
来源：http://ws.huanxung.cn

Py:   except ValueError as e:
来源：http://wb.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vr.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://wr.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://cd.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://lf.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ws.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://hh.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zd.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://di.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://hi.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://no.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pp.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ep.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vi.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lz.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://bq.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://wz.asd995.cn

[H07] 断言
来源：http://ya.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://wa.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://ag.newstarts.cn

JS:   console.assert(x > 0);
来源：http://li.521024.cn

TS:   console.assert(x > 0);
来源：http://kd.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://cu.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://je.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://me.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://sv.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://ey.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://na.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://by.nszjky.cn

JS:   e.message;  e.stack
来源：http://jv.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dt.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hy.wgjwhj.cn

Go:   err.Error()
来源：http://to.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://ab.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://tf.colortex.cn

[H09] 带错误码的异常
来源：http://jp.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hn.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hg.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oa.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ox.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jj.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rj.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wx.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tw.yuexingan06.cn

[H10] 资源自动释放
来源：http://uh.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ig.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ib.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sh.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sx.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gi.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://mc.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gr.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fd.shxzskj.cn

================================================================================
来源：http://af.newstarts.cn

I. 正则表达式
来源：http://ng.bjjhwx.cn

================================================================================
来源：http://az.panjiajie.cn

[I01] 判断是否匹配
来源：http://bs.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xh.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jw.nicolike.cn

JS:   /\d+/.test(s)
来源：http://es.hahajie.cn

TS:   /\d+/.test(s)
来源：http://vs.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gv.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kv.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://qm.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wl.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ap.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ti.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ia.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yt.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://wb.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ol.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tj.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://vk.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ee.gzmigu.cn

[I03] 提取捕获分组
来源：http://sl.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://su.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ad.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ex.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ak.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eb.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://se.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kd.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ik.shxzskj.cn

[I04] 正则替换
来源：http://nh.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ek.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wx.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dz.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ls.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zs.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sn.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://le.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xm.nicolike.cn

[I05] 按正则拆分
来源：http://qd.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bc.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://da.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://qc.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://vy.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://et.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gp.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kz.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tj.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://za.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mk.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ss.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vw.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kz.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bm.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uj.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://at.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vp.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://qn.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oc.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mb.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://te.asd995.cn

TS:   /error/gim
来源：http://dz.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uu.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xy.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://kp.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vj.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://sr.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://si.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wg.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vc.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://te.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fz.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vv.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iq.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sz.hahajie.cn

================================================================================
来源：http://uv.huixinmuqiang.cn

J. 日期与时间
来源：http://kb.bjjhwx.cn

================================================================================
来源：http://mz.bjjhwx.cn

[J01] 获取当前时间
来源：http://hz.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pc.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ij.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://jd.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://jf.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yr.nszjky.cn

Go:   time.Now()
来源：http://kq.huixiangedu.cn

Ruby: Time.now
来源：http://tm.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ok.muxihuayi.cn

[J02] 格式化输出
来源：http://lo.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gc.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ft.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ca.wgjwhj.cn

TS:   d.toISOString()
来源：http://rz.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mw.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ff.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://md.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wj.shxzskj.cn

[J03] 字符串解析为日期
来源：http://as.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lr.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tl.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://vn.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://bt.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ri.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ci.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://fw.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ey.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://cd.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vs.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vy.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nr.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qv.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ks.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zx.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nk.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sp.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://tc.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://xl.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oy.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nn.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sp.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://fb.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://us.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ma.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pz.huanxung.cn

[J06] 计算两时间之差
来源：http://ou.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://ve.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://zs.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mw.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://je.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ah.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://fv.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://mb.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://ow.lnxyls.cn

[J07] 比较两个日期
来源：http://kk.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://qz.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pv.shxzukj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pb.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vl.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rn.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zt.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hd.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://cb.panjiajie.cn

[J08] 提取年月日与星期
来源：http://mf.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://km.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pq.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://if.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kd.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://up.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uj.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xr.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vx.huixiangedu.cn

[J09] 时区处理
来源：http://mr.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iw.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zk.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fn.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vd.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ni.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nm.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ae.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bg.nicolike.cn

[J10] 取今天 / 本月第一天
来源：http://bh.panjiajie.cn


<!-- 参考信息 -->