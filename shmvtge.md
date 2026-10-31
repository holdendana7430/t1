代发 wailian999

[G10] 访问控制
来源：http://jc.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://jo.colortex.cn

PHP:  public / protected / private
来源：http://zh.colortex.cn

JS:   #private 字段；其余公开
来源：http://zc.9csxet.cn

TS:   public / protected / private
来源：http://yo.colortex.cn

Java: public / protected / private / 默认包级
来源：http://gu.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ja.bookmarksfly.cn

Ruby: public / protected / private
来源：http://sf.nszjky.cn

C#:   public / protected / private / internal
来源：http://iw.chemitech.net.cn

[G11] getter / setter
来源：http://uk.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://iw.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yn.huanxung.cn

JS:   get name() { return this._name; }
来源：http://dx.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://bf.nszjky.cn

Java: public String getName() { return name; }
来源：http://yd.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ga.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://xe.9csxet.cn

C#:   public string Name { get; set; }
来源：http://kn.panjiajie.cn

[G12] 对象转字符串
来源：http://mp.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ko.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pl.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://qd.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://wb.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://nm.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xg.nicolike.cn

Ruby: def to_s; @name; end
来源：http://wv.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://sl.nicolike.cn

[G13] 判断对象类型
来源：http://mo.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://wg.shxzskj.cn

PHP:  $u instanceof User
来源：http://vc.asd995.cn

JS:   u instanceof User
来源：http://oz.wgjwhj.cn

TS:   u instanceof User
来源：http://pe.bookmarksfly.cn

Java: u instanceof User
来源：http://so.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ww.colortex.cn

Ruby: u.is_a?(User)
来源：http://zc.haigaiapp.cn

C#:   u is User
来源：http://ap.panjiajie.cn

[G14] 数据类 / record
来源：http://jc.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gn.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://wb.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://et.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://qe.szsharing.cn

Java: record User(String name, int age) {}
来源：http://zh.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://qk.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://of.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://xa.shxzskj.cn

[G15] 枚举
来源：http://hv.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gw.muxihuayi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ms.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tb.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ia.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://ms.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://if.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://xj.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://js.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://wi.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://np.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://ml.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://qc.hahajie.cn

TS:   Object.entries(obj)
来源：http://ct.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rx.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cy.huanxung.cn

Ruby: obj.instance_variables
来源：http://yl.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://il.shtwfgs.cn

================================================================================
来源：http://aa.jctech888.com.cn

H. 异常与错误处理
来源：http://uo.bookmarksfly.cn

================================================================================
来源：http://en.huixiangedu.cn

[H01] try / catch 基础
来源：http://sy.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ct.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lg.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rk.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tw.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://li.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://df.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pc.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zd.nszjky.cn

[H02] finally / ensure 收尾
来源：http://le.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sj.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vh.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xo.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sl.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://za.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://td.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cu.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ki.nicolike.cn

[H03] 主动抛出异常
来源：http://ab.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://bz.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wd.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://sq.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://fj.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pz.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wp.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fg.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fe.nicolike.cn

[H04] 自定义异常类型
来源：http://zk.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://yg.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vq.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://ct.newstarts.cn

TS:   class MyError extends Error {}
来源：http://gp.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://fs.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ph.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://ah.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://rn.colortex.cn

[H05] 捕获特定类型
来源：http://ok.bjjhwx.cn

Py:   except ValueError as e:
来源：http://gy.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sh.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://df.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://dm.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://bi.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vx.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://ov.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gq.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://ro.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://sv.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cf.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tq.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lt.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hg.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kh.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://tu.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://yv.bjjhwx.cn

[H07] 断言
来源：http://dz.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://po.nicolike.cn

PHP:  assert($x > 0);
来源：http://yu.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://ie.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://bd.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://yk.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bs.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oy.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://yv.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://th.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://tm.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://so.newstarts.cn

JS:   e.message;  e.stack
来源：http://ei.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dd.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gs.newstarts.cn

Go:   err.Error()
来源：http://ak.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://hv.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://lf.newstarts.cn

[H09] 带错误码的异常
来源：http://gn.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qo.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hl.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sd.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bw.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ox.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uh.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bg.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yh.szxytkj.cn

[H10] 资源自动释放
来源：http://kl.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://se.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qv.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qu.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rb.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bf.szsharing.cn

Go:   defer f.Close()
来源：http://fs.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://go.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hq.asd995.cn

================================================================================
来源：http://pe.panjiajie.cn

I. 正则表达式
来源：http://rc.haigaiapp.cn

================================================================================
来源：http://ja.huixiangedu.cn

[I01] 判断是否匹配
来源：http://ol.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ml.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dg.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://kf.huanxung.cn

TS:   /\d+/.test(s)
来源：http://mt.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ei.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qm.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://dc.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ep.gzmigu.cn

[I02] 提取所有匹配
来源：http://tt.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://zx.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ng.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uc.521024.cn

TS:   s.match(/\d+/g)
来源：http://qw.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ci.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rx.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://jx.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://om.bjjhwx.cn

[I03] 提取捕获分组
来源：http://fw.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yr.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tv.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://we.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zg.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tp.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://io.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vt.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jt.chemitech.net.cn

[I04] 正则替换
来源：http://hg.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kx.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yh.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nc.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rk.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ge.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mk.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iq.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yh.shxzukj.cn

[I05] 按正则拆分
来源：http://wk.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gy.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zt.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://jc.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rf.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ae.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ny.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://di.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ao.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nv.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gw.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zk.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rg.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vk.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zr.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jg.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cf.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nh.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://kl.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bf.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bc.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vm.hnjuh.cn

TS:   /error/gim
来源：http://eh.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ov.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rt.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://pm.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tc.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://op.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bn.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ex.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ts.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yi.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fe.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kx.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xw.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dg.huanxung.cn

================================================================================
来源：http://sc.huanxung.cn

J. 日期与时间
来源：http://jy.szxytkj.cn

================================================================================
来源：http://dt.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://pq.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pg.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nt.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://hw.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://au.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hf.szxytkj.cn

Go:   time.Now()
来源：http://vq.521024.cn

Ruby: Time.now
来源：http://zi.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ng.muxihuayi.cn

[J02] 格式化输出
来源：http://to.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qz.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pz.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sr.521024.cn

TS:   d.toISOString()
来源：http://ln.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eh.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ve.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pb.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ri.521024.cn

[J03] 字符串解析为日期
来源：http://jv.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ud.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bw.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://wu.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://cl.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mk.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fg.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://fj.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yn.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://nl.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sc.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ca.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://in.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fu.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ag.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mm.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bm.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://re.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://va.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://jy.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xc.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bf.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ee.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://yi.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wl.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://ac.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uq.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://tj.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://th.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://ih.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jr.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ps.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kd.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://us.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://eu.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://xh.chemitech.net.cn

[J07] 比较两个日期
来源：http://zo.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://qa.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nv.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://no.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bq.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eq.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ck.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ns.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://fj.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://dr.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://by.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pc.newstarts.cn


<!-- 参考信息 -->