代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://he.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://ld.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://nq.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ct.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ui.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://qp.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://qh.bjjhwx.cn

[G13] 判断对象类型
来源：http://ot.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://tf.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://ta.bookmarksfly.cn

JS:   u instanceof User
来源：http://dy.huixiangedu.cn

TS:   u instanceof User
来源：http://te.colortex.cn

Java: u instanceof User
来源：http://pg.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cm.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://hx.bjjhwx.cn

C#:   u is User
来源：http://pa.huixiangedu.cn

[G14] 数据类 / record
来源：http://jl.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nx.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://au.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hs.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://jf.9csxet.cn

Java: record User(String name, int age) {}
来源：http://yu.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://rn.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://so.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://xx.panjiajie.cn

[G15] 枚举
来源：http://pf.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hf.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hx.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xz.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eb.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://ms.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vp.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://qb.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fr.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://cj.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dw.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://at.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://lg.szxytkj.cn

TS:   Object.entries(obj)
来源：http://xr.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ne.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wy.panjiajie.cn

Ruby: obj.instance_variables
来源：http://xw.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://uh.asd995.cn

================================================================================
来源：http://zl.huixinmuqiang.cn

H. 异常与错误处理
来源：http://rq.huanxung.cn

================================================================================
来源：http://qw.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://rg.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ou.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ul.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jg.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xp.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ob.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zl.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dw.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://um.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://yv.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ui.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ou.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dv.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nx.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ii.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gp.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ax.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mt.bjjhwx.cn

[H03] 主动抛出异常
来源：http://pb.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://lr.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://al.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://tr.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://vo.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nn.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rs.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yq.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kd.gzmigu.cn

[H04] 自定义异常类型
来源：http://ic.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://ty.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://se.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://bf.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://td.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://vo.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pk.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://pb.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://hw.haigaiapp.cn

[H05] 捕获特定类型
来源：http://rc.lnxyls.cn

Py:   except ValueError as e:
来源：http://rv.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://su.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://ql.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://lo.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://jp.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zp.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://ux.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://si.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://rz.nicolike.cn

Py:   value = d.get("k") or default
来源：http://fk.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ni.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zb.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ro.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sl.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fb.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://dp.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://yr.shxzskj.cn

[H07] 断言
来源：http://xc.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://rx.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://by.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://ow.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://be.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://sj.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uu.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nu.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://ed.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://kv.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://mb.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hf.shxzukj.cn

JS:   e.message;  e.stack
来源：http://om.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dx.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ve.huanxung.cn

Go:   err.Error()
来源：http://if.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://vf.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://ns.szsharing.cn

[H09] 带错误码的异常
来源：http://fs.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tl.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ni.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lm.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mt.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://np.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wq.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pl.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iu.huixiangedu.cn

[H10] 资源自动释放
来源：http://xg.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://it.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://td.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://as.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oi.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://od.nicolike.cn

Go:   defer f.Close()
来源：http://ft.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://by.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qv.szxytkj.cn

================================================================================
来源：http://br.shxzskj.cn

I. 正则表达式
来源：http://vd.lnxyls.cn

================================================================================
来源：http://ee.shtwfgs.cn

[I01] 判断是否匹配
来源：http://hx.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yl.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ue.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://yy.szsharing.cn

TS:   /\d+/.test(s)
来源：http://mx.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rc.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nc.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://eq.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yt.nicolike.cn

[I02] 提取所有匹配
来源：http://pb.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://cl.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hj.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sk.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://ja.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cy.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://in.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://gs.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iu.muxihuayi.cn

[I03] 提取捕获分组
来源：http://eq.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sk.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gv.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wu.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tu.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lb.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dg.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://my.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ps.huanxung.cn

[I04] 正则替换
来源：http://dy.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://is.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vg.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yh.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ux.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gj.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://et.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://da.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vk.bookmarksfly.cn

[I05] 按正则拆分
来源：http://os.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sf.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jc.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://tk.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://zr.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://wk.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kb.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gb.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xm.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nn.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vw.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://em.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rh.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mx.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zs.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jn.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wm.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wr.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://nn.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lk.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ri.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cn.9csxet.cn

TS:   /error/gim
来源：http://sa.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vv.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://py.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://se.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bl.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://qv.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zq.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rb.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wt.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tu.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ne.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wu.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oz.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://be.panjiajie.cn

================================================================================
来源：http://ef.shtwfgs.cn

J. 日期与时间
来源：http://nr.wgjwhj.cn

================================================================================
来源：http://sy.huanxung.cn

[J01] 获取当前时间
来源：http://lq.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ty.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xv.colortex.cn

JS:   new Date();  Date.now()
来源：http://ty.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://qx.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rs.bookmarksfly.cn

Go:   time.Now()
来源：http://fw.hahajie.cn

Ruby: Time.now
来源：http://lw.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fu.jianghongdianzi.cn

[J02] 格式化输出
来源：http://lh.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ju.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ws.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gf.nszjky.cn

TS:   d.toISOString()
来源：http://ya.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ns.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tt.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pj.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xp.gzmigu.cn

[J03] 字符串解析为日期
来源：http://cf.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ar.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ot.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://dr.asd995.cn

TS:   new Date("2024-01-02")
来源：http://rq.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ih.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cg.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://nj.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gv.nszjky.cn

[J04] 时间戳与日期互转
来源：http://hr.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tt.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://up.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xd.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://is.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cl.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pk.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mj.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hy.521024.cn

[J05] 时间加减（加 7 天）
来源：http://bz.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://am.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wm.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ma.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vy.szsharing.cn

Java: LocalDate.now().plusDays(7)
来源：http://gw.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vt.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://tx.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hl.szxytkj.cn

[J06] 计算两时间之差
来源：http://he.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://ab.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://gf.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zf.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://li.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uc.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://qn.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://em.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://ri.colortex.cn

[J07] 比较两个日期
来源：http://jg.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ke.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ef.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sc.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wj.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uq.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gl.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jd.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://bp.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://gi.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mo.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://px.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ab.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nx.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://do.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hx.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ka.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ik.shtwfgs.cn

[J09] 时区处理
来源：http://fq.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rz.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vz.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jc.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vi.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fu.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zb.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yk.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uf.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://mc.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xw.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ap.wgjwhj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gp.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wp.521024.cn


<!-- 参考信息 -->