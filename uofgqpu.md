代发 wailian999

[G10] 访问控制
来源：http://ji.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://wu.jctech888.com.cn

PHP:  public / protected / private
来源：http://be.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://rl.huixiangedu.cn

TS:   public / protected / private
来源：http://hm.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://vf.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oe.huixiangedu.cn

Ruby: public / protected / private
来源：http://lz.shxzskj.cn

C#:   public / protected / private / internal
来源：http://ld.jianghongdianzi.cn

[G11] getter / setter
来源：http://ij.newstarts.cn

Py:   @property 与 @x.setter
来源：http://wk.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jx.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://sj.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://ep.panjiajie.cn

Java: public String getName() { return name; }
来源：http://dk.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://um.9csxet.cn

Ruby: attr_accessor :name
来源：http://xg.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://pp.szsharing.cn

[G12] 对象转字符串
来源：http://jf.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://tz.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kz.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://da.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://ul.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://gv.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cq.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://da.asd995.cn

C#:   public override string ToString() => Name;
来源：http://uv.haigaiapp.cn

[G13] 判断对象类型
来源：http://le.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://ha.nszjky.cn

PHP:  $u instanceof User
来源：http://ww.chemitech.net.cn

JS:   u instanceof User
来源：http://lj.bookmarksfly.cn

TS:   u instanceof User
来源：http://qc.huixiangedu.cn

Java: u instanceof User
来源：http://bh.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uh.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://hx.wgjwhj.cn

C#:   u is User
来源：http://bm.haigaiapp.cn

[G14] 数据类 / record
来源：http://rk.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fg.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://rc.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ab.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://uu.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://sv.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://ap.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vq.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://zl.szsharing.cn

[G15] 枚举
来源：http://sw.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://by.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vp.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fw.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vy.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://ap.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jc.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://uq.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://em.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://nq.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ix.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://lv.shxzukj.cn

JS:   Object.entries(obj)
来源：http://fn.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://tn.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bc.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ve.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://kr.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ks.bookmarksfly.cn

================================================================================
来源：http://yj.nicolike.cn

H. 异常与错误处理
来源：http://iq.colortex.cn

================================================================================
来源：http://zg.szxytkj.cn

[H01] try / catch 基础
来源：http://ew.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://al.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zo.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ig.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ld.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sh.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vs.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cf.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mc.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://ur.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tx.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xl.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ut.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fj.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fm.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jx.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ga.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wo.hahajie.cn

[H03] 主动抛出异常
来源：http://eg.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://aw.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zu.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://io.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://sk.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jo.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nl.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ay.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bl.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://xj.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://kb.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://is.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://ag.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://ey.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://ii.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fr.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://pe.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://nd.newstarts.cn

[H05] 捕获特定类型
来源：http://cx.szxytkj.cn

Py:   except ValueError as e:
来源：http://ku.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mr.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://bb.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://pl.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://ew.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gj.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://si.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eh.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://dg.asd995.cn

Py:   value = d.get("k") or default
来源：http://gn.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ta.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xg.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vc.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://li.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tn.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://mh.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://vf.newstarts.cn

[H07] 断言
来源：http://cd.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://dy.9csxet.cn

PHP:  assert($x > 0);
来源：http://yr.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://ow.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://jm.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://br.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ca.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ud.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://mb.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://bm.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://nw.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uv.shxzskj.cn

JS:   e.message;  e.stack
来源：http://wh.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pb.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nl.9csxet.cn

Go:   err.Error()
来源：http://nr.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://ow.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://gl.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://rv.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xm.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mm.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rt.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zb.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hu.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yd.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xb.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://to.9csxet.cn

[H10] 资源自动释放
来源：http://ob.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lz.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jl.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nu.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gb.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yn.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://sr.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yz.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jt.panjiajie.cn

================================================================================
来源：http://vo.521024.cn

I. 正则表达式
来源：http://ch.szxytkj.cn

================================================================================
来源：http://dd.panjiajie.cn

[I01] 判断是否匹配
来源：http://ho.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xe.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://io.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ts.asd995.cn

TS:   /\d+/.test(s)
来源：http://vp.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oe.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gs.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://qk.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://df.wgjwhj.cn

[I02] 提取所有匹配
来源：http://pj.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://zm.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ng.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fb.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://sc.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pq.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://jm.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qg.chemitech.net.cn

[I03] 提取捕获分组
来源：http://qe.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://il.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sv.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kh.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mo.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mg.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vh.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vm.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nk.chemitech.net.cn

[I04] 正则替换
来源：http://hr.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fo.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ka.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qr.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ok.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ex.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ys.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gi.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zz.521024.cn

[I05] 按正则拆分
来源：http://ch.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sy.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://be.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://um.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://xx.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://ww.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rs.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://au.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ex.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uk.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vw.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hy.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://va.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mv.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bt.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gf.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eg.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bc.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://hn.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ci.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://to.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wl.panjiajie.cn

TS:   /error/gim
来源：http://rv.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qp.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fx.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://cd.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mx.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://lv.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wv.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ne.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hh.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bp.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ky.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nh.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xm.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tt.szsharing.cn

================================================================================
来源：http://dk.nszjky.cn

J. 日期与时间
来源：http://pg.hnjuh.cn

================================================================================
来源：http://os.bookmarksfly.cn

[J01] 获取当前时间
来源：http://gl.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bu.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ls.szsharing.cn

JS:   new Date();  Date.now()
来源：http://au.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://sr.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bc.521024.cn

Go:   time.Now()
来源：http://ha.shxzukj.cn

Ruby: Time.now
来源：http://nd.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ol.bookmarksfly.cn

[J02] 格式化输出
来源：http://bm.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yu.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qt.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://um.nicolike.cn

TS:   d.toISOString()
来源：http://wg.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jn.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yo.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iu.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ni.hahajie.cn

[J03] 字符串解析为日期
来源：http://xg.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vb.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nz.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://kw.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://pl.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://db.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mm.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://gm.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://if.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://kz.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iv.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pf.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xh.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fk.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wr.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yt.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ei.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gp.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://bd.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://ct.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tn.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://it.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dz.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://cn.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zr.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ra.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aj.521024.cn

[J06] 计算两时间之差
来源：http://zr.9csxet.cn

Py:   (end - start).total_seconds()
来源：http://pz.colortex.cn

PHP:  $end->diff($start)->days;
来源：http://re.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ks.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zx.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mf.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://eu.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://he.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://vm.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://lg.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://eq.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uu.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://un.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fj.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ss.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uh.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xt.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://es.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://pf.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jz.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gv.shxzukj.cn


<!-- 参考信息 -->