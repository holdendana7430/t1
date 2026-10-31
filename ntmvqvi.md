代发 wailian999

C#:   public / protected / private / internal
来源：http://xi.hnjuh.cn

[G11] getter / setter
来源：http://xz.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ji.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yw.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://le.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://si.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://da.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://or.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://vb.colortex.cn

C#:   public string Name { get; set; }
来源：http://ow.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://do.colortex.cn

Py:   def __str__(self): return self.name
来源：http://et.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ws.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://sd.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://li.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://pg.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yc.9csxet.cn

Ruby: def to_s; @name; end
来源：http://gt.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://zs.newstarts.cn

[G13] 判断对象类型
来源：http://di.newstarts.cn

Py:   isinstance(u, User)
来源：http://gr.521024.cn

PHP:  $u instanceof User
来源：http://kq.newstarts.cn

JS:   u instanceof User
来源：http://fx.bookmarksfly.cn

TS:   u instanceof User
来源：http://cd.muxihuayi.cn

Java: u instanceof User
来源：http://as.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bx.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ku.huixiangedu.cn

C#:   u is User
来源：http://ni.9csxet.cn

[G14] 数据类 / record
来源：http://sj.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cj.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://xq.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uk.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://ia.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://oq.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://nt.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fb.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://qz.jianghongdianzi.cn

[G15] 枚举
来源：http://os.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ph.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://km.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://em.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yn.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://yn.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hm.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://jf.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ov.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://ju.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://na.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://mh.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://xq.hahajie.cn

TS:   Object.entries(obj)
来源：http://pd.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ee.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.huanxung.cn

Ruby: obj.instance_variables
来源：http://zj.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ul.jctech888.com.cn

================================================================================
来源：http://mh.gzmigu.cn

H. 异常与错误处理
来源：http://kq.panjiajie.cn

================================================================================
来源：http://ig.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://hx.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ev.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fu.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ui.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oy.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ol.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fy.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lc.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ue.colortex.cn

[H02] finally / ensure 收尾
来源：http://rx.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rm.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qb.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qt.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://po.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ws.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zm.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fz.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ij.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://hk.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://hr.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pc.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://ug.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://uh.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qk.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kh.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tz.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jw.panjiajie.cn

[H04] 自定义异常类型
来源：http://kr.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://xo.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ud.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://mv.9csxet.cn

TS:   class MyError extends Error {}
来源：http://ui.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://tj.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zo.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://dc.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://xh.asd995.cn

[H05] 捕获特定类型
来源：http://kt.gzmigu.cn

Py:   except ValueError as e:
来源：http://qq.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://an.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://uc.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://my.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://dt.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mi.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://cs.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://na.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://et.9csxet.cn

Py:   value = d.get("k") or default
来源：http://rb.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sz.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ml.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jt.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ca.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pt.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://ab.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://xb.huixinmuqiang.cn

[H07] 断言
来源：http://rx.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://do.nicolike.cn

PHP:  assert($x > 0);
来源：http://yg.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://ic.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://fs.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ph.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vm.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ap.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://iu.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://en.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://vm.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pc.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://cy.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nr.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://th.wgjwhj.cn

Go:   err.Error()
来源：http://jx.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://gj.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://qf.521024.cn

[H09] 带错误码的异常
来源：http://un.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ae.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xa.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vx.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lv.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qw.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://am.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sk.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tz.nszjky.cn

[H10] 资源自动释放
来源：http://ct.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vs.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ic.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jk.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cw.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ul.gzmigu.cn

Go:   defer f.Close()
来源：http://le.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://al.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uq.colortex.cn

================================================================================
来源：http://nx.muxihuayi.cn

I. 正则表达式
来源：http://tt.szsharing.cn

================================================================================
来源：http://pb.szsharing.cn

[I01] 判断是否匹配
来源：http://kc.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mh.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ot.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://el.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://vu.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tn.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oy.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://yl.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ky.wgjwhj.cn

[I02] 提取所有匹配
来源：http://fn.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ln.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://um.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rj.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://me.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wp.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fb.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://rx.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nc.chemitech.net.cn

[I03] 提取捕获分组
来源：http://jy.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vc.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://le.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pc.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xc.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vq.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vj.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://si.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ms.chemitech.net.cn

[I04] 正则替换
来源：http://eq.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yl.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ta.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gn.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://of.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kh.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qe.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iz.haigaiapp.cn

[I05] 按正则拆分
来源：http://js.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ix.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zm.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://rv.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://hs.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://qe.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qq.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zl.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pu.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zj.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rw.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dn.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ky.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hl.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fi.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vs.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ws.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ms.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://de.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ky.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vp.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vx.nszjky.cn

TS:   /error/gim
来源：http://cu.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hj.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ht.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://bj.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kr.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://zn.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qv.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bs.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://et.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ye.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xg.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tt.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ci.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xq.jctech888.com.cn

================================================================================
来源：http://lc.lnxyls.cn

J. 日期与时间
来源：http://oe.shxzukj.cn

================================================================================
来源：http://ms.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://kf.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ot.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jl.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://cy.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://tq.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fg.yuntaijiaju.cn

Go:   time.Now()
来源：http://rp.hnjuh.cn

Ruby: Time.now
来源：http://fe.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pj.chemitech.net.cn

[J02] 格式化输出
来源：http://zy.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ko.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lz.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tm.szsharing.cn

TS:   d.toISOString()
来源：http://cl.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nq.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fm.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://su.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sx.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://tu.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mx.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ie.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://dh.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://xe.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pu.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pu.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://af.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://to.nszjky.cn

[J04] 时间戳与日期互转
来源：http://dd.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lo.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oq.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gn.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://st.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sy.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uz.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yk.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gf.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://sn.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://xe.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zm.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gk.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rr.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://eh.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nh.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://lc.szsharing.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gu.colortex.cn

[J06] 计算两时间之差
来源：http://li.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://qu.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://hk.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wc.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gk.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bo.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://un.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://rd.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://me.shxzukj.cn

[J07] 比较两个日期
来源：http://lc.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://bp.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bh.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xt.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iu.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wj.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lz.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bi.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://zc.szsharing.cn

[J08] 提取年月日与星期
来源：http://om.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iy.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jo.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yx.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://is.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ua.chemitech.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qa.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ce.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ph.bookmarksfly.cn

[J09] 时区处理
来源：http://ik.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ad.haigaiapp.cn


<!-- 参考信息 -->