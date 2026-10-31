代发 wailian999

C#:   public / protected / private / internal
来源：http://px.huixiangedu.cn

[G11] getter / setter
来源：http://ca.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://nd.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vw.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://tw.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://zp.lnxyls.cn

Java: public String getName() { return name; }
来源：http://jr.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://up.szsharing.cn

Ruby: attr_accessor :name
来源：http://pn.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://ba.jctech888.com.cn

[G12] 对象转字符串
来源：http://uj.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://wp.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mh.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://ml.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://zj.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://jw.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dg.nszjky.cn

Ruby: def to_s; @name; end
来源：http://vw.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://rt.huixiangedu.cn

[G13] 判断对象类型
来源：http://dy.hahajie.cn

Py:   isinstance(u, User)
来源：http://ms.asd995.cn

PHP:  $u instanceof User
来源：http://ga.haigaiapp.cn

JS:   u instanceof User
来源：http://iw.shxzukj.cn

TS:   u instanceof User
来源：http://ne.bookmarksfly.cn

Java: u instanceof User
来源：http://dx.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://it.asd995.cn

Ruby: u.is_a?(User)
来源：http://pr.bjjhwx.cn

C#:   u is User
来源：http://so.bookmarksfly.cn

[G14] 数据类 / record
来源：http://wp.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yz.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://yf.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ah.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://xr.huanxung.cn

Java: record User(String name, int age) {}
来源：http://cl.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://fu.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mh.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://ad.huixinmuqiang.cn

[G15] 枚举
来源：http://wk.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hs.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gm.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://te.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://th.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://sw.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uz.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://mt.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bj.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://nl.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qx.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://wy.hahajie.cn

JS:   Object.entries(obj)
来源：http://mk.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://sr.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nr.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wk.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://vy.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://vt.asd995.cn

================================================================================
来源：http://gt.panjiajie.cn

H. 异常与错误处理
来源：http://fi.haigaiapp.cn

================================================================================
来源：http://qd.newstarts.cn

[H01] try / catch 基础
来源：http://tf.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qy.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hy.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rg.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://de.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dc.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sn.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lf.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qq.9csxet.cn

[H02] finally / ensure 收尾
来源：http://ut.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ne.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gh.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ns.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gb.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qe.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lk.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sz.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yo.shxzukj.cn

[H03] 主动抛出异常
来源：http://qo.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://mk.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ja.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://xj.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://ga.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bc.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hr.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lk.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pl.chemitech.net.cn

[H04] 自定义异常类型
来源：http://hp.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://nb.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fd.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://hv.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://mg.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://yf.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ef.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://yy.9csxet.cn

C#:   class MyException : Exception {}
来源：http://nl.muxihuayi.cn

[H05] 捕获特定类型
来源：http://vw.chemitech.net.cn

Py:   except ValueError as e:
来源：http://ow.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nc.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://uq.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://wb.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://wq.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tp.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://am.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tw.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://hr.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://mn.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pm.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fy.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uj.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qr.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kr.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://ah.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://sy.colortex.cn

[H07] 断言
来源：http://wh.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://tu.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://rn.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://zg.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://mh.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://sl.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bq.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://ty.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://sy.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://vb.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://de.szxytkj.cn

JS:   e.message;  e.stack
来源：http://up.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ga.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uj.gzmigu.cn

Go:   err.Error()
来源：http://it.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://ai.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://bk.nicolike.cn

[H09] 带错误码的异常
来源：http://qk.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ls.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dq.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://em.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://za.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yw.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zn.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uy.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://af.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://ss.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sy.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rf.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ez.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bf.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wg.huanxung.cn

Go:   defer f.Close()
来源：http://wd.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mh.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kl.9csxet.cn

================================================================================
来源：http://fs.jianghongdianzi.cn

I. 正则表达式
来源：http://ro.asd995.cn

================================================================================
来源：http://xe.szxytkj.cn

[I01] 判断是否匹配
来源：http://oa.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cg.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oz.hahajie.cn

JS:   /\d+/.test(s)
来源：http://nk.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://wq.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ch.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ja.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://qf.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lp.huixiangedu.cn

[I02] 提取所有匹配
来源：http://ws.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://cj.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bd.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fj.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://rc.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ry.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://he.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://gg.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://af.bjjhwx.cn

[I03] 提取捕获分组
来源：http://fh.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cs.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hf.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wf.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kh.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mt.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vr.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ds.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xa.9csxet.cn

[I04] 正则替换
来源：http://bi.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ie.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ce.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sv.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nt.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://et.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://my.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dc.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lj.bjjhwx.cn

[I05] 按正则拆分
来源：http://lc.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ji.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ss.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://rz.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://gb.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://ak.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eq.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sp.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cs.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zc.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wy.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wi.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ge.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gf.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pz.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yx.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gj.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wl.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://fn.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qq.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qo.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://su.haigaiapp.cn

TS:   /error/gim
来源：http://be.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xu.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dh.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://xz.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wm.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://fg.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zg.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lk.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gx.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qq.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sx.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://za.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bi.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ii.yuexingan06.cn

================================================================================
来源：http://sb.lnxyls.cn

J. 日期与时间
来源：http://au.jianghongdianzi.cn

================================================================================
来源：http://ru.szxytkj.cn

[J01] 获取当前时间
来源：http://aw.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ku.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ki.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://pt.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://kg.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fj.nszjky.cn

Go:   time.Now()
来源：http://qq.shtwfgs.cn

Ruby: Time.now
来源：http://ao.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hl.bookmarksfly.cn

[J02] 格式化输出
来源：http://dk.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vk.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ua.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://do.521024.cn

TS:   d.toISOString()
来源：http://eo.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mx.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yk.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nm.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nn.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://ur.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ax.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dl.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://vk.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://mr.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hj.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kc.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://eq.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rs.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://vg.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qt.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mz.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wh.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lq.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jo.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sp.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sa.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cf.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://qs.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://nj.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ca.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fv.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uu.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://tz.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ss.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://qh.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ge.szxytkj.cn

[J06] 计算两时间之差
来源：http://qt.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://ei.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://qq.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://my.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pn.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ep.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://ji.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://vw.nicolike.cn

C#:   (end - start).TotalSeconds
来源：http://rc.jctech888.com.cn

[J07] 比较两个日期
来源：http://dk.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ii.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hx.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bk.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rh.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vk.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ru.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hu.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://pt.szsharing.cn

[J08] 提取年月日与星期
来源：http://we.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kt.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://im.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://md.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ly.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ms.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yx.huanxung.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jb.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yr.chemitech.net.cn

[J09] 时区处理
来源：http://qy.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ji.chemitech.net.cn


<!-- 参考信息 -->