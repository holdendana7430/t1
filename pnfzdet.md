代发 wailian999

JS:   get name() { return this._name; }
来源：http://aa.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://fp.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://vy.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://se.newstarts.cn

Ruby: attr_accessor :name
来源：http://jg.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://ml.newstarts.cn

[G12] 对象转字符串
来源：http://ri.colortex.cn

Py:   def __str__(self): return self.name
来源：http://rh.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qn.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://ao.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://kt.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://gz.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cj.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://oe.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://su.asd995.cn

[G13] 判断对象类型
来源：http://xl.521024.cn

Py:   isinstance(u, User)
来源：http://yk.shtwfgs.cn

PHP:  $u instanceof User
来源：http://un.yuntaijiaju.cn

JS:   u instanceof User
来源：http://gq.yuntaijiaju.cn

TS:   u instanceof User
来源：http://kp.huixiangedu.cn

Java: u instanceof User
来源：http://qn.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zg.hahajie.cn

Ruby: u.is_a?(User)
来源：http://uk.asd995.cn

C#:   u is User
来源：http://ar.szxytkj.cn

[G14] 数据类 / record
来源：http://eg.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oy.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://hf.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ty.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://os.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://sd.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://pt.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jp.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://gg.muxihuayi.cn

[G15] 枚举
来源：http://wr.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rn.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rj.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ix.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ud.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://dq.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vy.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://wb.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ce.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://sa.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yr.colortex.cn

PHP:  get_object_vars($obj);
来源：http://ab.asd995.cn

JS:   Object.entries(obj)
来源：http://va.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://jn.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ui.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rx.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://yl.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://tt.jctech888.com.cn

================================================================================
来源：http://qe.gzmigu.cn

H. 异常与错误处理
来源：http://zw.bookmarksfly.cn

================================================================================
来源：http://is.newstarts.cn

[H01] try / catch 基础
来源：http://za.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ai.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cf.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yd.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hl.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eu.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yt.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jc.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mc.asd995.cn

[H02] finally / ensure 收尾
来源：http://fj.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lb.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gh.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tp.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://on.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qj.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sy.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nz.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uj.nszjky.cn

[H03] 主动抛出异常
来源：http://ha.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://vo.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://en.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://bk.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://zs.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jv.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bo.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sx.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ht.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://mw.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://tf.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qk.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://ua.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://yx.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://gf.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vj.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://if.szsharing.cn

C#:   class MyException : Exception {}
来源：http://nl.nszjky.cn

[H05] 捕获特定类型
来源：http://ex.muxihuayi.cn

Py:   except ValueError as e:
来源：http://gy.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qs.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://ac.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://dw.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://jl.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hj.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://tx.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://by.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://ra.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://td.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ke.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ta.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pp.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://au.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://za.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://ze.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://dm.lnxyls.cn

[H07] 断言
来源：http://tn.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://gp.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://ux.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://pq.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://kw.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://zj.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xb.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lw.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://vj.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://aj.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://bi.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fr.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://eh.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ic.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jx.hnjuh.cn

Go:   err.Error()
来源：http://ch.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://fp.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://cv.haigaiapp.cn

[H09] 带错误码的异常
来源：http://by.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tr.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xv.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yd.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kn.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gj.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pv.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ap.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ji.asd995.cn

[H10] 资源自动释放
来源：http://wt.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qa.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hd.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mj.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ae.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tm.haigaiapp.cn

Go:   defer f.Close()
来源：http://en.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qz.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yn.shxzskj.cn

================================================================================
来源：http://vs.szxytkj.cn

I. 正则表达式
来源：http://gp.shxzukj.cn

================================================================================
来源：http://wh.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://oq.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://od.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ya.asd995.cn

JS:   /\d+/.test(s)
来源：http://bl.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://js.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lx.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jc.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://no.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bo.nicolike.cn

[I02] 提取所有匹配
来源：http://tq.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://ei.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xl.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ps.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://vj.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qt.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ls.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://lh.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oq.shtwfgs.cn

[I03] 提取捕获分组
来源：http://td.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dx.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ny.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ts.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sr.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ox.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kn.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rz.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ln.asd995.cn

[I04] 正则替换
来源：http://qz.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://np.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nd.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ka.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ei.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fh.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rs.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bv.hnjuh.cn

[I05] 按正则拆分
来源：http://xr.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nm.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rf.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://xc.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://eo.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://vz.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://up.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tj.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sq.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sc.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lf.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ex.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bn.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ah.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nq.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zb.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uj.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qf.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://gi.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ch.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ny.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dl.gzmigu.cn

TS:   /error/gim
来源：http://vd.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zm.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fa.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://ok.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vk.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://cq.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ll.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fq.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gj.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zm.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ph.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pu.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pq.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://we.bookmarksfly.cn

================================================================================
来源：http://jq.asd995.cn

J. 日期与时间
来源：http://yr.huanxung.cn

================================================================================
来源：http://rs.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://xy.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nt.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bh.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://sa.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ez.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://px.nszjky.cn

Go:   time.Now()
来源：http://kn.shxzskj.cn

Ruby: Time.now
来源：http://bb.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ub.lnxyls.cn

[J02] 格式化输出
来源：http://hl.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iu.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xl.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bg.huixiangedu.cn

TS:   d.toISOString()
来源：http://tr.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ab.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hb.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ll.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hd.colortex.cn

[J03] 字符串解析为日期
来源：http://gq.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gh.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ee.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://at.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://cp.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wd.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://we.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ht.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wp.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://du.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://al.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://on.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hl.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fn.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://da.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vh.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hl.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sk.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://ph.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://cp.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://or.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ws.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ge.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://hq.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://km.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://dx.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fg.shxzskj.cn

[J06] 计算两时间之差
来源：http://at.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://gg.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://yb.colortex.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qd.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lz.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mu.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://qx.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://uh.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://oz.szxytkj.cn

[J07] 比较两个日期
来源：http://yh.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://qy.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vt.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jj.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tg.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://by.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rk.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ez.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://fd.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://kq.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ba.bjjhwx.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mw.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pg.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vs.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sy.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vl.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fx.asd995.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qp.shtwfgs.cn

[J09] 时区处理
来源：http://ke.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zo.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rt.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yn.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uy.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tn.bjjhwx.cn


<!-- 参考信息 -->