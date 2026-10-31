代发 wailian999

Ruby: attr_accessor :name
来源：http://jl.nicolike.cn

C#:   public string Name { get; set; }
来源：http://uo.newstarts.cn

[G12] 对象转字符串
来源：http://sc.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://en.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gz.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://ve.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://td.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://fh.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wc.nicolike.cn

Ruby: def to_s; @name; end
来源：http://mr.colortex.cn

C#:   public override string ToString() => Name;
来源：http://tt.shtwfgs.cn

[G13] 判断对象类型
来源：http://en.szsharing.cn

Py:   isinstance(u, User)
来源：http://bb.panjiajie.cn

PHP:  $u instanceof User
来源：http://me.9csxet.cn

JS:   u instanceof User
来源：http://ms.9csxet.cn

TS:   u instanceof User
来源：http://sb.hnjuh.cn

Java: u instanceof User
来源：http://od.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wy.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://cs.wgjwhj.cn

C#:   u is User
来源：http://lp.yuexingan06.cn

[G14] 数据类 / record
来源：http://db.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ld.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://me.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jh.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://dx.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://py.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://vj.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ow.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://cm.hnjuh.cn

[G15] 枚举
来源：http://dh.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yi.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gp.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lf.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://co.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://zz.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pr.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://im.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://od.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://yx.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ji.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://il.hnjuh.cn

JS:   Object.entries(obj)
来源：http://fp.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://ek.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ok.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sr.hahajie.cn

Ruby: obj.instance_variables
来源：http://ii.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://by.newstarts.cn

================================================================================
来源：http://xo.nszjky.cn

H. 异常与错误处理
来源：http://nt.chemitech.net.cn

================================================================================
来源：http://we.szxytkj.cn

[H01] try / catch 基础
来源：http://vc.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jm.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nn.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jf.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qw.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ra.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mh.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mc.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vz.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://am.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jz.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hj.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dd.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bt.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vy.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://av.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oe.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ez.jctech888.com.cn

[H03] 主动抛出异常
来源：http://no.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://ca.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://an.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://cq.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://ka.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ic.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kr.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://om.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fx.huanxung.cn

[H04] 自定义异常类型
来源：http://ox.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://cm.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ue.521024.cn

JS:   class MyError extends Error {}
来源：http://st.colortex.cn

TS:   class MyError extends Error {}
来源：http://pw.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://qz.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zi.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://xv.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://xc.huixiangedu.cn

[H05] 捕获特定类型
来源：http://se.muxihuayi.cn

Py:   except ValueError as e:
来源：http://ks.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fe.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://mw.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ff.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://nq.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ma.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://nf.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aj.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://kq.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://ba.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ko.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ez.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ds.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dg.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ba.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://vz.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://ff.gzmigu.cn

[H07] 断言
来源：http://io.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://aq.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://fb.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://jj.hahajie.cn

TS:   console.assert(x > 0);
来源：http://is.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://ng.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nb.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uf.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://ac.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://ez.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://ch.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fk.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://uf.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xm.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sw.521024.cn

Go:   err.Error()
来源：http://yu.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://eg.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://si.szsharing.cn

[H09] 带错误码的异常
来源：http://eq.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nv.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jl.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bs.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fg.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://us.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oc.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kq.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://on.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://nq.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nr.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yo.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://re.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wc.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xc.asd995.cn

Go:   defer f.Close()
来源：http://qi.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ax.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://da.wgjwhj.cn

================================================================================
来源：http://rp.szsharing.cn

I. 正则表达式
来源：http://ji.colortex.cn

================================================================================
来源：http://us.nicolike.cn

[I01] 判断是否匹配
来源：http://qp.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tg.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wv.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://pn.hahajie.cn

TS:   /\d+/.test(s)
来源：http://ag.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aq.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cz.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://eq.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kl.muxihuayi.cn

[I02] 提取所有匹配
来源：http://xv.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://nw.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fv.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dc.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://nc.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://px.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vq.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://zf.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ah.hahajie.cn

[I03] 提取捕获分组
来源：http://hf.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jd.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sk.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ka.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rx.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aj.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gs.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ur.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ff.asd995.cn

[I04] 正则替换
来源：http://kp.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vw.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dz.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wi.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://si.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lq.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mm.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hy.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cv.szsharing.cn

[I05] 按正则拆分
来源：http://fv.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hj.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ly.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://dk.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://uo.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://pe.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nd.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vp.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mx.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jr.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mq.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oi.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jd.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ch.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lm.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aq.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sf.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yy.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://to.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fx.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fs.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tj.muxihuayi.cn

TS:   /error/gim
来源：http://sr.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://in.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xh.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://ym.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sl.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://at.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://th.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fy.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oc.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mm.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ol.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uq.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hb.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vm.521024.cn

================================================================================
来源：http://um.muxihuayi.cn

J. 日期与时间
来源：http://fs.9csxet.cn

================================================================================
来源：http://vj.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://ul.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kj.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iu.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://kx.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://tp.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sf.yuntaijiaju.cn

Go:   time.Now()
来源：http://uw.bookmarksfly.cn

Ruby: Time.now
来源：http://ow.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mg.jctech888.com.cn

[J02] 格式化输出
来源：http://fy.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pd.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fm.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uj.colortex.cn

TS:   d.toISOString()
来源：http://zd.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qh.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ny.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yc.hnjuh.cn

[J03] 字符串解析为日期
来源：http://dn.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xc.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hu.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://vw.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://cb.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cw.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wk.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://es.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kw.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://sx.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yl.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://os.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://za.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gh.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kk.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ve.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wv.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ub.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://xu.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://pz.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eh.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tk.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uv.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://tt.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bk.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://la.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ca.bjjhwx.cn

[J06] 计算两时间之差
来源：http://ng.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://xz.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://mb.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gd.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kh.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tt.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://wm.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://ig.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://nc.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://xm.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://xm.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gq.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ux.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ri.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ut.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qp.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ak.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://xe.gzmigu.cn

[J08] 提取年月日与星期
来源：http://yt.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zm.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rx.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ys.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mj.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mn.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oc.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zn.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://il.huixinmuqiang.cn

[J09] 时区处理
来源：http://zo.huixinmuqiang.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://be.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dt.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gk.szxytkj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xp.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mj.newstarts.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mf.yuexingan06.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hr.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yp.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://eb.bookmarksfly.cn


<!-- 参考信息 -->