代发 wailian999

C#:   public / protected / private / internal
来源：http://dt.nszjky.cn

[G11] getter / setter
来源：http://hf.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ey.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bo.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://ol.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://cu.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://cc.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dl.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://nr.nszjky.cn

C#:   public string Name { get; set; }
来源：http://lx.jctech888.com.cn

[G12] 对象转字符串
来源：http://cc.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://qr.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jl.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://kl.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://bx.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://rj.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tq.nszjky.cn

Ruby: def to_s; @name; end
来源：http://yx.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://vg.asd995.cn

[G13] 判断对象类型
来源：http://mw.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://bg.chemitech.net.cn

PHP:  $u instanceof User
来源：http://co.hnjuh.cn

JS:   u instanceof User
来源：http://rs.szxytkj.cn

TS:   u instanceof User
来源：http://rs.yuexingan06.cn

Java: u instanceof User
来源：http://ky.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sq.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://kh.szsharing.cn

C#:   u is User
来源：http://gy.lnxyls.cn

[G14] 数据类 / record
来源：http://yd.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://au.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://nn.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rs.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://uq.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://ez.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://fk.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bq.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://uu.hnjuh.cn

[G15] 枚举
来源：http://cs.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://il.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://th.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ox.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xf.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://xk.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://td.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://lo.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xh.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://vw.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sw.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://td.gzmigu.cn

JS:   Object.entries(obj)
来源：http://ys.shxzukj.cn

TS:   Object.entries(obj)
来源：http://bq.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dd.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bq.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://fe.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://uz.szsharing.cn

================================================================================
来源：http://gt.colortex.cn

H. 异常与错误处理
来源：http://cq.hahajie.cn

================================================================================
来源：http://in.nszjky.cn

[H01] try / catch 基础
来源：http://sm.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xc.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ou.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://me.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ca.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ko.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ms.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uj.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://is.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://kp.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cl.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ku.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uz.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tl.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rw.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xl.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sg.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dw.shxzukj.cn

[H03] 主动抛出异常
来源：http://tq.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://bk.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://us.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://up.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://ha.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ho.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ax.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zj.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ru.jctech888.com.cn

[H04] 自定义异常类型
来源：http://yz.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://ii.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sl.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://wr.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://cp.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://hp.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://we.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://as.nszjky.cn

C#:   class MyException : Exception {}
来源：http://eu.szsharing.cn

[H05] 捕获特定类型
来源：http://lx.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://rp.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bd.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://sw.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://nw.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://qy.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zj.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://ii.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://re.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://za.nicolike.cn

Py:   value = d.get("k") or default
来源：http://es.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sy.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hn.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rr.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pf.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qf.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://oh.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://ao.bookmarksfly.cn

[H07] 断言
来源：http://jv.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://vi.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://jj.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://td.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://ym.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://es.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vl.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zu.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://du.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://ss.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://wo.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nn.shxzskj.cn

JS:   e.message;  e.stack
来源：http://yq.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vk.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cp.huanxung.cn

Go:   err.Error()
来源：http://ok.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://xj.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://rw.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://vc.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jb.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lc.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sd.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cj.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ys.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iw.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wn.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://to.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://qu.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zo.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yk.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bh.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vg.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zo.shxzukj.cn

Go:   defer f.Close()
来源：http://oq.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uu.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xv.yuntaijiaju.cn

================================================================================
来源：http://lp.yuexingan06.cn

I. 正则表达式
来源：http://el.muxihuayi.cn

================================================================================
来源：http://xd.jctech888.com.cn

[I01] 判断是否匹配
来源：http://ei.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dc.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ft.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://xt.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://dx.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oh.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://le.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://rd.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ac.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://ea.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://wi.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qp.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fv.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://ap.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qm.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zn.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://tt.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dq.colortex.cn

[I03] 提取捕获分组
来源：http://gy.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rt.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ho.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xc.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xw.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vv.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://je.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gy.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gb.szsharing.cn

[I04] 正则替换
来源：http://gn.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pv.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lu.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://il.jctech888.com.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sw.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ks.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ht.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gu.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sd.chemitech.net.cn

[I05] 按正则拆分
来源：http://hk.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kc.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zq.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://ug.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://js.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://nm.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cg.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qr.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gk.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fv.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ww.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ip.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hw.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ij.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jr.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xt.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bf.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xh.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://am.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jz.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xn.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cz.newstarts.cn

TS:   /error/gim
来源：http://ul.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ki.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rn.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://en.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wb.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://aw.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vy.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hv.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xn.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cr.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dc.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oc.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qg.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://es.hahajie.cn

================================================================================
来源：http://hi.huixiangedu.cn

J. 日期与时间
来源：http://vc.hahajie.cn

================================================================================
来源：http://qq.newstarts.cn

[J01] 获取当前时间
来源：http://ra.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aw.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tl.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://lf.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://pn.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bl.huanxung.cn

Go:   time.Now()
来源：http://xv.szxytkj.cn

Ruby: Time.now
来源：http://hx.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cz.shxzukj.cn

[J02] 格式化输出
来源：http://ld.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cj.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dm.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kb.gzmigu.cn

TS:   d.toISOString()
来源：http://pr.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tg.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yk.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jc.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zd.shxzskj.cn

[J03] 字符串解析为日期
来源：http://yt.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fv.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pc.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://tq.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://zo.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ib.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ei.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ff.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uy.colortex.cn

[J04] 时间戳与日期互转
来源：http://ej.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nz.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mc.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hk.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oc.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ry.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yx.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tm.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xg.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://jv.szsharing.cn

Py:   now + timedelta(days=7)
来源：http://wb.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://op.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sb.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cs.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://fa.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://es.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://wx.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bu.gzmigu.cn

[J06] 计算两时间之差
来源：http://tg.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://nt.asd995.cn

PHP:  $end->diff($start)->days;
来源：http://my.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sg.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ca.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qw.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://mu.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://fo.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://tu.bjjhwx.cn

[J07] 比较两个日期
来源：http://lg.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://ri.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fa.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qe.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://th.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ik.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ot.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mm.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://kx.hahajie.cn

[J08] 提取年月日与星期
来源：http://ib.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ee.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ko.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://um.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jc.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ia.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bz.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hk.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ul.haigaiapp.cn

[J09] 时区处理
来源：http://si.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bf.yuntaijiaju.cn


<!-- 参考信息 -->