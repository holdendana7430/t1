代发 wailian999

C#:   public / protected / private / internal
来源：http://ni.nszjky.cn

[G11] getter / setter
来源：http://kz.nicolike.cn

Py:   @property 与 @x.setter
来源：http://lh.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://at.hahajie.cn

JS:   get name() { return this._name; }
来源：http://hu.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://qh.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://ln.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qw.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://po.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ud.jctech888.com.cn

[G12] 对象转字符串
来源：http://va.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://rc.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jn.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://ll.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://gq.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://gi.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cz.nicolike.cn

Ruby: def to_s; @name; end
来源：http://yl.asd995.cn

C#:   public override string ToString() => Name;
来源：http://xb.colortex.cn

[G13] 判断对象类型
来源：http://tv.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://vz.huixiangedu.cn

PHP:  $u instanceof User
来源：http://nf.jianghongdianzi.cn

JS:   u instanceof User
来源：http://ur.hahajie.cn

TS:   u instanceof User
来源：http://od.jianghongdianzi.cn

Java: u instanceof User
来源：http://zg.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cy.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://zc.521024.cn

C#:   u is User
来源：http://oz.shtwfgs.cn

[G14] 数据类 / record
来源：http://es.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://br.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://uk.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fn.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://qg.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://fu.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://lr.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rj.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://ix.hahajie.cn

[G15] 枚举
来源：http://an.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ia.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yt.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bn.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://at.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://ad.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yf.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://qp.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xn.colortex.cn

[G16] 对象转数组 / 字典
来源：http://yd.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hl.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://ev.asd995.cn

JS:   Object.entries(obj)
来源：http://wc.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://jd.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://no.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ba.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://lh.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://bc.muxihuayi.cn

================================================================================
来源：http://hg.szxytkj.cn

H. 异常与错误处理
来源：http://jo.szxytkj.cn

================================================================================
来源：http://ke.muxihuayi.cn

[H01] try / catch 基础
来源：http://kn.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mq.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xx.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://by.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ff.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yq.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fw.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uh.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fp.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://ri.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gm.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bx.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cd.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fn.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://af.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://la.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dn.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zh.asd995.cn

[H03] 主动抛出异常
来源：http://ne.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://rb.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sf.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://oz.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://sm.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zz.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pk.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ak.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ae.chemitech.net.cn

[H04] 自定义异常类型
来源：http://qo.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://hi.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pu.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://af.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://et.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://pg.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cm.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://qk.szsharing.cn

C#:   class MyException : Exception {}
来源：http://fg.panjiajie.cn

[H05] 捕获特定类型
来源：http://sm.panjiajie.cn

Py:   except ValueError as e:
来源：http://bk.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://io.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://rz.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://zt.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://dm.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bt.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://wj.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sg.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ag.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://rf.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zw.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dk.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nt.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mi.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nc.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://ve.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://ip.shxzukj.cn

[H07] 断言
来源：http://ui.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://st.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://fd.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ja.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://hz.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://od.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://de.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kr.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://rj.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://xr.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://sj.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ni.newstarts.cn

JS:   e.message;  e.stack
来源：http://ci.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ru.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kb.huixinmuqiang.cn

Go:   err.Error()
来源：http://rh.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://nm.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://ea.chemitech.net.cn

[H09] 带错误码的异常
来源：http://xw.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bl.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hl.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yh.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uk.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ji.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ye.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uz.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nw.yuexingan06.cn

[H10] 资源自动释放
来源：http://yi.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://np.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qj.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xy.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ih.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zv.shtwfgs.cn

Go:   defer f.Close()
来源：http://yz.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pi.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://is.521024.cn

================================================================================
来源：http://lk.shxzskj.cn

I. 正则表达式
来源：http://pa.nicolike.cn

================================================================================
来源：http://it.haigaiapp.cn

[I01] 判断是否匹配
来源：http://fx.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eq.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nf.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://mg.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://lr.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pq.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gq.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://gz.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rb.haigaiapp.cn

[I02] 提取所有匹配
来源：http://dn.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://mj.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ph.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rw.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://sc.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jy.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://no.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://zd.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wy.muxihuayi.cn

[I03] 提取捕获分组
来源：http://fb.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dj.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bz.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qu.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://je.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ru.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ua.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ce.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qb.panjiajie.cn

[I04] 正则替换
来源：http://dt.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ms.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tz.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lm.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bd.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rm.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zg.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qu.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://so.yuexingan06.cn

[I05] 按正则拆分
来源：http://ha.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ls.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jm.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://bw.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://pi.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://gq.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dx.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jf.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ma.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bz.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fc.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lm.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qj.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zx.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zp.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zl.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bg.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kq.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://mv.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fq.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ee.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bn.521024.cn

TS:   /error/gim
来源：http://va.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://im.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vd.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://ue.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ga.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://bv.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tu.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pw.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gt.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fk.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nj.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mh.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xm.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ba.asd995.cn

================================================================================
来源：http://yh.haigaiapp.cn

J. 日期与时间
来源：http://ov.bjjhwx.cn

================================================================================
来源：http://dr.haigaiapp.cn

[J01] 获取当前时间
来源：http://pz.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cx.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lj.newstarts.cn

JS:   new Date();  Date.now()
来源：http://xu.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://sd.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mi.bookmarksfly.cn

Go:   time.Now()
来源：http://lg.hnjuh.cn

Ruby: Time.now
来源：http://bx.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sn.yuntaijiaju.cn

[J02] 格式化输出
来源：http://oo.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hb.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bv.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ed.huanxung.cn

TS:   d.toISOString()
来源：http://kt.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zq.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ql.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xp.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nk.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://mc.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kx.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uv.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://dy.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://lg.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pb.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wu.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://zx.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wg.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://ry.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hp.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tx.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sw.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rq.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ho.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vr.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vt.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kt.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://ic.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://qo.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xq.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zt.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qr.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://tt.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ni.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://sr.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kz.bjjhwx.cn

[J06] 计算两时间之差
来源：http://im.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://ea.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://aq.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zh.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bf.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yv.521024.cn

Go:   end.Sub(start).Hours()
来源：http://xw.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://yu.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://qo.nszjky.cn

[J07] 比较两个日期
来源：http://zb.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://nd.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qh.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://et.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hs.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ka.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lz.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ch.colortex.cn

C#:   d1 < d2;  d1 == d2
来源：http://qr.lnxyls.cn

[J08] 提取年月日与星期
来源：http://zu.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fg.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ia.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cn.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bt.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jf.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://my.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://su.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wh.yuexingan06.cn

[J09] 时区处理
来源：http://qw.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cz.bjjhwx.cn


<!-- 参考信息 -->