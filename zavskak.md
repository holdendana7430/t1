代发 wailian999

C#:   public / protected / private / internal
来源：http://ms.chemitech.net.cn

[G11] getter / setter
来源：http://tx.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://qf.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ot.colortex.cn

JS:   get name() { return this._name; }
来源：http://em.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://wl.huanxung.cn

Java: public String getName() { return name; }
来源：http://ag.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kd.nszjky.cn

Ruby: attr_accessor :name
来源：http://my.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://on.shtwfgs.cn

[G12] 对象转字符串
来源：http://gk.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://jn.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yz.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://wb.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://rn.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://nf.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zf.huanxung.cn

Ruby: def to_s; @name; end
来源：http://hs.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://fn.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://an.asd995.cn

Py:   isinstance(u, User)
来源：http://nt.nszjky.cn

PHP:  $u instanceof User
来源：http://ha.nszjky.cn

JS:   u instanceof User
来源：http://ev.521024.cn

TS:   u instanceof User
来源：http://iq.jctech888.com.cn

Java: u instanceof User
来源：http://lk.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dt.nszjky.cn

Ruby: u.is_a?(User)
来源：http://nt.jctech888.com.cn

C#:   u is User
来源：http://ge.bookmarksfly.cn

[G14] 数据类 / record
来源：http://fx.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wf.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://eg.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ry.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://rn.nszjky.cn

Java: record User(String name, int age) {}
来源：http://ob.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://ac.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rb.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://al.haigaiapp.cn

[G15] 枚举
来源：http://oc.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ee.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ua.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aq.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yk.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://hf.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hw.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://sm.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tn.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://xe.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qw.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://sf.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://ld.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://it.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://di.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zh.nszjky.cn

Ruby: obj.instance_variables
来源：http://lk.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://ny.nszjky.cn

================================================================================
来源：http://vz.521024.cn

H. 异常与错误处理
来源：http://it.gzmigu.cn

================================================================================
来源：http://jr.lnxyls.cn

[H01] try / catch 基础
来源：http://hr.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ue.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yb.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://re.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xg.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jg.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tw.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://il.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eg.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://ty.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yj.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ig.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jv.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sj.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vi.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uk.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hi.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dx.asd995.cn

[H03] 主动抛出异常
来源：http://do.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://vl.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xv.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://ke.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://zh.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://so.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yz.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qo.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kq.yuexingan06.cn

[H04] 自定义异常类型
来源：http://at.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://kg.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://de.nszjky.cn

JS:   class MyError extends Error {}
来源：http://nw.nszjky.cn

TS:   class MyError extends Error {}
来源：http://mh.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://sh.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gr.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://et.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://wk.nszjky.cn

[H05] 捕获特定类型
来源：http://fq.colortex.cn

Py:   except ValueError as e:
来源：http://za.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zd.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://wi.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://xk.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://uw.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hx.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://pe.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ns.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://hv.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://ik.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yp.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bs.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xe.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kj.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xw.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://hz.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://tj.huanxung.cn

[H07] 断言
来源：http://pc.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://dn.colortex.cn

PHP:  assert($x > 0);
来源：http://df.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://fj.nszjky.cn

TS:   console.assert(x > 0);
来源：http://xm.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://bf.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wr.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wn.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://av.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://nn.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://lt.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cq.shxzukj.cn

JS:   e.message;  e.stack
来源：http://hz.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://op.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mz.newstarts.cn

Go:   err.Error()
来源：http://pc.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://na.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://uw.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://bc.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lw.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zh.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://os.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ob.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nj.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ie.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ax.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qv.hahajie.cn

[H10] 资源自动释放
来源：http://mv.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lb.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nv.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aw.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ee.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://to.wgjwhj.cn

Go:   defer f.Close()
来源：http://mt.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ym.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pl.bookmarksfly.cn

================================================================================
来源：http://ey.shxzukj.cn

I. 正则表达式
来源：http://xv.jctech888.com.cn

================================================================================
来源：http://ba.gzmigu.cn

[I01] 判断是否匹配
来源：http://er.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vn.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wk.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://vk.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://su.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yc.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ud.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://yv.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ug.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://nu.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ia.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ts.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cm.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://vs.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vy.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gt.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ge.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cx.hnjuh.cn

[I03] 提取捕获分组
来源：http://dk.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iw.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yp.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fc.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://za.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ps.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iw.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vt.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sm.muxihuayi.cn

[I04] 正则替换
来源：http://sp.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vj.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gx.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hx.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://li.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iw.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qp.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://th.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zm.szxytkj.cn

[I05] 按正则拆分
来源：http://ol.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qp.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ye.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://nf.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://su.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://xm.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://je.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ih.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qf.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zw.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qe.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wh.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://il.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nk.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fm.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bz.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qp.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bf.521024.cn

[I07] 忽略大小写与多行模式
来源：http://wy.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ev.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ev.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ax.shxzskj.cn

TS:   /error/gim
来源：http://rj.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vr.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xp.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://uk.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zr.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://eq.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aw.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tu.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ji.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lp.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://my.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zi.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ca.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dz.newstarts.cn

================================================================================
来源：http://my.wgjwhj.cn

J. 日期与时间
来源：http://iy.shxzskj.cn

================================================================================
来源：http://pj.panjiajie.cn

[J01] 获取当前时间
来源：http://xx.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ti.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vh.nicolike.cn

JS:   new Date();  Date.now()
来源：http://vd.asd995.cn

TS:   new Date();  Date.now()
来源：http://ma.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dq.bjjhwx.cn

Go:   time.Now()
来源：http://qw.nicolike.cn

Ruby: Time.now
来源：http://vv.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://br.newstarts.cn

[J02] 格式化输出
来源：http://pc.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jn.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sc.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://am.muxihuayi.cn

TS:   d.toISOString()
来源：http://cx.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oj.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://od.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wk.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dd.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://ex.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bx.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cq.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://so.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://xm.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cl.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nx.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://vz.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lg.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://cj.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cr.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jl.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cv.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ea.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ro.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://in.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rh.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ov.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://vx.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://nw.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gn.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://il.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rm.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://tf.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nr.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://vb.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sx.panjiajie.cn

[J06] 计算两时间之差
来源：http://yg.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://cz.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://qk.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eb.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wz.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xg.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://nu.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://by.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://wg.yuexingan06.cn

[J07] 比较两个日期
来源：http://ta.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://kw.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gw.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wa.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zs.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wd.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wr.shtwfgs.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ox.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ca.hnjuh.cn

[J08] 提取年月日与星期
来源：http://ol.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bs.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dk.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lb.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uq.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ru.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ka.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ae.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ik.huixiangedu.cn

[J09] 时区处理
来源：http://jm.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vm.szxytkj.cn


<!-- 参考信息 -->