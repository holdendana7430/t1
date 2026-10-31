代发 wailian999

TS:   public / protected / private
来源：http://ip.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://xg.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://is.colortex.cn

Ruby: public / protected / private
来源：http://bh.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://sa.colortex.cn

[G11] getter / setter
来源：http://mw.newstarts.cn

Py:   @property 与 @x.setter
来源：http://kl.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yd.521024.cn

JS:   get name() { return this._name; }
来源：http://ja.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://bn.hahajie.cn

Java: public String getName() { return name; }
来源：http://hd.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fb.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://rh.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://lx.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://os.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://of.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qp.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://my.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://fa.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://hs.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dj.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://re.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://nx.shxzskj.cn

[G13] 判断对象类型
来源：http://ei.asd995.cn

Py:   isinstance(u, User)
来源：http://fj.lnxyls.cn

PHP:  $u instanceof User
来源：http://gq.wgjwhj.cn

JS:   u instanceof User
来源：http://zi.haigaiapp.cn

TS:   u instanceof User
来源：http://jr.9csxet.cn

Java: u instanceof User
来源：http://xa.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pr.9csxet.cn

Ruby: u.is_a?(User)
来源：http://na.haigaiapp.cn

C#:   u is User
来源：http://yj.hahajie.cn

[G14] 数据类 / record
来源：http://ma.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ar.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://bc.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://do.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://ev.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://lt.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://uc.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wx.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://qa.szsharing.cn

[G15] 枚举
来源：http://yr.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mj.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tf.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qn.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fr.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://bu.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ht.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://rs.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ab.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://pr.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pl.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://uy.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ko.panjiajie.cn

TS:   Object.entries(obj)
来源：http://ek.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jf.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pe.newstarts.cn

Ruby: obj.instance_variables
来源：http://bq.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://hg.hahajie.cn

================================================================================
来源：http://pm.yuexingan06.cn

H. 异常与错误处理
来源：http://dw.muxihuayi.cn

================================================================================
来源：http://mp.huanxung.cn

[H01] try / catch 基础
来源：http://js.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ck.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ic.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ui.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gl.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ue.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://se.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://at.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fv.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://bm.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ui.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rh.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cc.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jc.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zr.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kr.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xk.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xb.shtwfgs.cn

[H03] 主动抛出异常
来源：http://oe.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://ff.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yi.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://ba.521024.cn

TS:   throw new Error("错误信息");
来源：http://qn.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jz.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yb.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://au.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kg.szsharing.cn

[H04] 自定义异常类型
来源：http://ee.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://pe.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ke.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ls.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://zs.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://ty.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bf.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://ao.nicolike.cn

C#:   class MyException : Exception {}
来源：http://bm.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://si.hahajie.cn

Py:   except ValueError as e:
来源：http://ba.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://db.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://ag.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://xz.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://dd.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rk.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://lu.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bj.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://kv.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://kv.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://na.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wz.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yf.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dd.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://da.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://lu.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://hh.jctech888.com.cn

[H07] 断言
来源：http://nl.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://ay.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://yy.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://aa.hahajie.cn

TS:   console.assert(x > 0);
来源：http://wr.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://nk.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vm.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://st.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://qh.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://td.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://ps.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ou.hnjuh.cn

JS:   e.message;  e.stack
来源：http://by.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zn.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zd.9csxet.cn

Go:   err.Error()
来源：http://rj.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://tz.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://hj.jctech888.com.cn

[H09] 带错误码的异常
来源：http://jd.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ie.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cn.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vs.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pg.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://um.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sk.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vw.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vv.nszjky.cn

[H10] 资源自动释放
来源：http://fn.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bc.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vr.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kq.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://in.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nv.wgjwhj.cn

Go:   defer f.Close()
来源：http://lp.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://im.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vo.haigaiapp.cn

================================================================================
来源：http://ig.huanxung.cn

I. 正则表达式
来源：http://rs.bookmarksfly.cn

================================================================================
来源：http://bg.hnjuh.cn

[I01] 判断是否匹配
来源：http://yr.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mm.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ht.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://fg.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://cf.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xx.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ia.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://xs.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lp.jctech888.com.cn

[I02] 提取所有匹配
来源：http://pu.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://dr.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wb.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gr.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://zb.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nd.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tx.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://vm.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ew.colortex.cn

[I03] 提取捕获分组
来源：http://lh.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ak.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sq.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zc.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rz.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ak.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qe.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jl.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mt.asd995.cn

[I04] 正则替换
来源：http://re.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://om.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ib.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://by.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qs.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bl.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rm.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fn.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nv.nicolike.cn

[I05] 按正则拆分
来源：http://ls.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pt.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jz.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ag.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://op.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://eb.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lp.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ru.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://by.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lu.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://od.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yi.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vn.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ln.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bx.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fj.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zr.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://el.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://zh.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bn.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vs.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mh.hahajie.cn

TS:   /error/gim
来源：http://bi.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lt.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dm.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://zx.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zt.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://od.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xg.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uq.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xg.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nx.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jm.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zl.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rr.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nv.muxihuayi.cn

================================================================================
来源：http://pj.yuexingan06.cn

J. 日期与时间
来源：http://zl.panjiajie.cn

================================================================================
来源：http://yu.shxzskj.cn

[J01] 获取当前时间
来源：http://be.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gw.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fn.szsharing.cn

JS:   new Date();  Date.now()
来源：http://gl.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://wq.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ub.szxytkj.cn

Go:   time.Now()
来源：http://ti.jianghongdianzi.cn

Ruby: Time.now
来源：http://km.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ju.szxytkj.cn

[J02] 格式化输出
来源：http://km.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bd.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ot.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ts.bookmarksfly.cn

TS:   d.toISOString()
来源：http://cb.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gc.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gt.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zs.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ac.lnxyls.cn

[J03] 字符串解析为日期
来源：http://aj.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://en.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nv.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://kx.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://wa.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ru.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kf.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://qs.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://id.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://dg.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vf.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cv.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dv.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tl.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rb.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pt.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ax.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ca.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://bd.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://or.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rz.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bs.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fy.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://or.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fd.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://hc.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bs.muxihuayi.cn

[J06] 计算两时间之差
来源：http://dl.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://tj.szsharing.cn

PHP:  $end->diff($start)->days;
来源：http://qk.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ed.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://px.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ii.szxytkj.cn

Go:   end.Sub(start).Hours()
来源：http://sc.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://tj.521024.cn

C#:   (end - start).TotalSeconds
来源：http://ig.shtwfgs.cn

[J07] 比较两个日期
来源：http://hw.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://pd.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mn.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ge.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dw.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ar.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://em.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ws.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://ml.nszjky.cn

[J08] 提取年月日与星期
来源：http://le.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gi.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yh.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jz.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lp.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ua.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uo.bjjhwx.cn


<!-- 参考信息 -->