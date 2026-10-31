代发 wailian999

[G10] 访问控制
来源：http://kk.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://gv.chemitech.net.cn

PHP:  public / protected / private
来源：http://ug.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://np.hnjuh.cn

TS:   public / protected / private
来源：http://qv.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://kn.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eo.colortex.cn

Ruby: public / protected / private
来源：http://oh.9csxet.cn

C#:   public / protected / private / internal
来源：http://vt.shxzskj.cn

[G11] getter / setter
来源：http://un.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://fo.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tk.newstarts.cn

JS:   get name() { return this._name; }
来源：http://mc.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://ja.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://bu.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wy.colortex.cn

Ruby: attr_accessor :name
来源：http://pz.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://gq.colortex.cn

[G12] 对象转字符串
来源：http://xa.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://qq.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ci.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://yy.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://or.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://ai.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lc.newstarts.cn

Ruby: def to_s; @name; end
来源：http://kw.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://yt.huixiangedu.cn

[G13] 判断对象类型
来源：http://md.shxzukj.cn

Py:   isinstance(u, User)
来源：http://vt.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://ra.hnjuh.cn

JS:   u instanceof User
来源：http://ti.panjiajie.cn

TS:   u instanceof User
来源：http://hm.bookmarksfly.cn

Java: u instanceof User
来源：http://fy.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cg.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ve.szxytkj.cn

C#:   u is User
来源：http://br.hnjuh.cn

[G14] 数据类 / record
来源：http://zv.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hw.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://um.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jb.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://dp.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://eg.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ox.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vx.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://fj.newstarts.cn

[G15] 枚举
来源：http://qa.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gj.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mf.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gd.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qq.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://nz.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qb.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://qa.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kz.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://ox.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qg.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://nb.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://aa.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://eq.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zq.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sj.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://zt.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://bj.lnxyls.cn

================================================================================
来源：http://cx.bjjhwx.cn

H. 异常与错误处理
来源：http://zv.bjjhwx.cn

================================================================================
来源：http://dt.9csxet.cn

[H01] try / catch 基础
来源：http://bp.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wd.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ok.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cz.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://un.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mn.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ya.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ya.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xe.huanxung.cn

[H02] finally / ensure 收尾
来源：http://xk.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oq.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tx.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rq.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ee.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sp.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xx.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ut.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iz.9csxet.cn

[H03] 主动抛出异常
来源：http://la.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://af.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wk.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://kc.colortex.cn

TS:   throw new Error("错误信息");
来源：http://jr.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ys.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vk.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ci.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ob.huixiangedu.cn

[H04] 自定义异常类型
来源：http://ba.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://hb.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ze.nszjky.cn

JS:   class MyError extends Error {}
来源：http://wb.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://rl.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://kd.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oo.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://dl.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://yd.shxzskj.cn

[H05] 捕获特定类型
来源：http://ju.muxihuayi.cn

Py:   except ValueError as e:
来源：http://ti.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ka.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ce.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://nh.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://mf.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ey.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://lv.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iw.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://ub.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://av.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fs.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sw.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rj.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gf.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qs.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://yy.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://ns.nszjky.cn

[H07] 断言
来源：http://sk.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://bd.szxytkj.cn

PHP:  assert($x > 0);
来源：http://xv.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://dl.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://cu.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://nd.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fz.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://az.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://rp.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://hs.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://cd.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ac.hnjuh.cn

JS:   e.message;  e.stack
来源：http://xq.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fg.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sd.jianghongdianzi.cn

Go:   err.Error()
来源：http://lh.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://gc.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ak.huixiangedu.cn

[H09] 带错误码的异常
来源：http://di.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vw.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zv.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://va.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cz.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yo.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wz.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://en.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ws.muxihuayi.cn

[H10] 资源自动释放
来源：http://wu.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wq.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ju.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nm.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wj.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jv.hahajie.cn

Go:   defer f.Close()
来源：http://um.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yg.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rm.muxihuayi.cn

================================================================================
来源：http://qp.hahajie.cn

I. 正则表达式
来源：http://jx.jctech888.com.cn

================================================================================
来源：http://fv.huanxung.cn

[I01] 判断是否匹配
来源：http://at.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vk.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gg.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://ks.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://zd.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sg.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uz.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://hf.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uu.hahajie.cn

[I02] 提取所有匹配
来源：http://fb.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://du.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ce.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kx.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://yj.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qm.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qm.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://zl.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qe.yuexingan06.cn

[I03] 提取捕获分组
来源：http://kl.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yi.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ii.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jb.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sb.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wc.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sv.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vk.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xc.bjjhwx.cn

[I04] 正则替换
来源：http://to.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zw.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rh.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://av.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gx.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iu.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://il.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zb.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hx.asd995.cn

[I05] 按正则拆分
来源：http://mr.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qp.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wp.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://my.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://kw.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://aw.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qn.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mk.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ou.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rt.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qw.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jz.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mq.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xr.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ji.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lg.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uc.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qp.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://nt.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oj.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vl.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ma.lnxyls.cn

TS:   /error/gim
来源：http://jr.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mx.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ut.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://ew.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ak.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ec.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vo.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vk.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://og.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ou.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bo.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zm.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xj.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ya.szsharing.cn

================================================================================
来源：http://qm.haigaiapp.cn

J. 日期与时间
来源：http://tu.hahajie.cn

================================================================================
来源：http://bq.shxzukj.cn

[J01] 获取当前时间
来源：http://ci.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://iz.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mb.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://bc.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://ax.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fy.szxytkj.cn

Go:   time.Now()
来源：http://qm.521024.cn

Ruby: Time.now
来源：http://tx.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://be.panjiajie.cn

[J02] 格式化输出
来源：http://em.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ry.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gk.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xi.bjjhwx.cn

TS:   d.toISOString()
来源：http://tc.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sc.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kz.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qt.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bz.nszjky.cn

[J03] 字符串解析为日期
来源：http://pp.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dk.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jm.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://hi.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://xt.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tk.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ji.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://mj.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hp.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://js.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wg.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dq.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cg.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ur.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cv.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ap.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iq.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fl.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://wb.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://gn.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gr.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ug.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eu.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://kd.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hb.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://uh.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nx.newstarts.cn

[J06] 计算两时间之差
来源：http://qz.521024.cn

Py:   (end - start).total_seconds()
来源：http://yg.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://gs.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sy.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zc.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uu.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://kf.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://gm.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://sn.nszjky.cn

[J07] 比较两个日期
来源：http://kx.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://ix.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lp.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wy.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ck.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rv.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ki.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gm.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://hv.gzmigu.cn

[J08] 提取年月日与星期
来源：http://ey.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mi.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mb.yuexingan06.cn


<!-- 参考信息 -->