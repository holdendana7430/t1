代发 wailian999

JS:   get name() { return this._name; }
来源：http://qe.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://zw.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://tr.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vn.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://of.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://fq.shtwfgs.cn

[G12] 对象转字符串
来源：http://rw.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://cj.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zr.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://bg.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://vb.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://pz.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tq.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://ls.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://xp.nszjky.cn

[G13] 判断对象类型
来源：http://ly.szsharing.cn

Py:   isinstance(u, User)
来源：http://aw.shxzukj.cn

PHP:  $u instanceof User
来源：http://dr.newstarts.cn

JS:   u instanceof User
来源：http://dp.shtwfgs.cn

TS:   u instanceof User
来源：http://cl.bjjhwx.cn

Java: u instanceof User
来源：http://sg.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oy.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://vs.gzmigu.cn

C#:   u is User
来源：http://yy.szsharing.cn

[G14] 数据类 / record
来源：http://ll.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tl.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://bw.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bw.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://ek.huanxung.cn

Java: record User(String name, int age) {}
来源：http://jm.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://da.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ci.asd995.cn

C#:   record User(string Name, int Age);
来源：http://hq.nicolike.cn

[G15] 枚举
来源：http://lz.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kb.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zv.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://to.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nz.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://uo.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sp.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://ze.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bp.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://ek.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jt.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://aw.521024.cn

JS:   Object.entries(obj)
来源：http://es.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://ka.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vp.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bd.asd995.cn

Ruby: obj.instance_variables
来源：http://wn.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://jj.9csxet.cn

================================================================================
来源：http://ux.hnjuh.cn

H. 异常与错误处理
来源：http://yl.nszjky.cn

================================================================================
来源：http://qr.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://sa.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sh.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xc.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sj.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ft.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rs.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xh.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dn.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dc.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://xa.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mj.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://io.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ou.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vj.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rh.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ab.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dk.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jk.hahajie.cn

[H03] 主动抛出异常
来源：http://he.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://eo.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ni.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://gk.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://mu.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fv.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zo.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ff.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ov.muxihuayi.cn

[H04] 自定义异常类型
来源：http://tb.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://jd.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yt.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://mm.nszjky.cn

TS:   class MyError extends Error {}
来源：http://yx.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://ai.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zx.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://px.nszjky.cn

C#:   class MyException : Exception {}
来源：http://iu.newstarts.cn

[H05] 捕获特定类型
来源：http://gx.szxytkj.cn

Py:   except ValueError as e:
来源：http://uq.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wt.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://ld.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://rb.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://dm.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yn.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://zs.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gn.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://mk.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://kh.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://md.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wc.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cs.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sn.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pq.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://vu.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://hg.521024.cn

[H07] 断言
来源：http://ro.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://aq.shxzskj.cn

PHP:  assert($x > 0);
来源：http://tx.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://jp.szsharing.cn

TS:   console.assert(x > 0);
来源：http://of.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://nq.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ni.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wt.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://mz.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://re.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://md.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ec.9csxet.cn

JS:   e.message;  e.stack
来源：http://ia.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://as.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fp.szsharing.cn

Go:   err.Error()
来源：http://fj.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://da.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://vp.wgjwhj.cn

[H09] 带错误码的异常
来源：http://sn.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tw.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xf.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tq.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hh.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://te.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xg.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jb.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://go.colortex.cn

[H10] 资源自动释放
来源：http://lq.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xl.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mr.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iy.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ic.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xi.szsharing.cn

Go:   defer f.Close()
来源：http://ix.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kg.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wr.bjjhwx.cn

================================================================================
来源：http://tw.chemitech.net.cn

I. 正则表达式
来源：http://es.asd995.cn

================================================================================
来源：http://lm.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://dn.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jk.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bj.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://ep.521024.cn

TS:   /\d+/.test(s)
来源：http://ap.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tp.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zf.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://jx.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sb.shtwfgs.cn

[I02] 提取所有匹配
来源：http://ef.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://wn.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cf.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fs.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://kg.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ki.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kj.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://wn.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ad.hnjuh.cn

[I03] 提取捕获分组
来源：http://ig.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ti.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ys.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oe.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ww.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fo.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dn.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cv.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jk.wgjwhj.cn

[I04] 正则替换
来源：http://ii.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kx.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://po.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nf.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zv.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vu.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dm.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hb.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qw.szsharing.cn

[I05] 按正则拆分
来源：http://fd.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sl.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cv.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://sm.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://hg.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://pb.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fs.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lr.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ow.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zc.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ic.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cm.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tc.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pu.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wm.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gp.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gi.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oc.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://wl.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qs.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cj.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jf.huixiangedu.cn

TS:   /error/gim
来源：http://jf.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ss.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wf.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://iq.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tx.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://rp.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tq.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cs.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bn.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qs.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uy.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gc.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xh.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yg.panjiajie.cn

================================================================================
来源：http://ab.shxzskj.cn

J. 日期与时间
来源：http://vm.shxzukj.cn

================================================================================
来源：http://ad.9csxet.cn

[J01] 获取当前时间
来源：http://du.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ma.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xu.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://bv.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://om.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ot.shxzskj.cn

Go:   time.Now()
来源：http://gl.gzmigu.cn

Ruby: Time.now
来源：http://cj.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sc.colortex.cn

[J02] 格式化输出
来源：http://pz.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lt.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qz.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mg.haigaiapp.cn

TS:   d.toISOString()
来源：http://pf.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bw.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lb.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vm.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lq.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://gv.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://up.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ci.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://ah.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://jq.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cr.muxihuayi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ck.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://xb.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://in.szsharing.cn

[J04] 时间戳与日期互转
来源：http://ab.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ka.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xm.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://de.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gc.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mm.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cq.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fr.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://np.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://mj.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://wh.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ji.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gy.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xl.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://sp.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vb.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://fj.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://he.gzmigu.cn

[J06] 计算两时间之差
来源：http://ex.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://tn.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://kz.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ca.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jg.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nn.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://zz.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://cz.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://vu.bookmarksfly.cn

[J07] 比较两个日期
来源：http://lh.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://sl.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nz.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yw.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zv.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://br.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bp.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rb.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://yd.newstarts.cn

[J08] 提取年月日与星期
来源：http://vt.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bn.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sg.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jy.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uz.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ph.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vc.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yh.muxihuayi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fg.bookmarksfly.cn

[J09] 时区处理
来源：http://za.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hy.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gi.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cp.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jk.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qn.yuexingan06.cn


<!-- 参考信息 -->