代发 wailian999

[G10] 访问控制
来源：http://zr.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://ux.521024.cn

PHP:  public / protected / private
来源：http://wd.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://xw.shtwfgs.cn

TS:   public / protected / private
来源：http://gb.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://hn.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://so.chemitech.net.cn

Ruby: public / protected / private
来源：http://mm.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://sh.shtwfgs.cn

[G11] getter / setter
来源：http://og.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://bz.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ks.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://sq.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://dn.panjiajie.cn

Java: public String getName() { return name; }
来源：http://gy.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zj.szxytkj.cn

Ruby: attr_accessor :name
来源：http://mh.521024.cn

C#:   public string Name { get; set; }
来源：http://hn.newstarts.cn

[G12] 对象转字符串
来源：http://si.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://ko.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sl.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://xn.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://ee.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://jg.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xc.szsharing.cn

Ruby: def to_s; @name; end
来源：http://xn.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://kt.panjiajie.cn

[G13] 判断对象类型
来源：http://dr.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://ru.szsharing.cn

PHP:  $u instanceof User
来源：http://va.huixiangedu.cn

JS:   u instanceof User
来源：http://ct.colortex.cn

TS:   u instanceof User
来源：http://sh.nicolike.cn

Java: u instanceof User
来源：http://vb.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fn.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://ym.huixiangedu.cn

C#:   u is User
来源：http://pz.hnjuh.cn

[G14] 数据类 / record
来源：http://mv.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qe.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://xg.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mr.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://cx.9csxet.cn

Java: record User(String name, int age) {}
来源：http://ec.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://wh.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ay.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://xq.huixiangedu.cn

[G15] 枚举
来源：http://hh.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ju.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://is.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pu.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pr.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://ax.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dw.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://pu.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yn.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://ft.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kg.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://yf.hnjuh.cn

JS:   Object.entries(obj)
来源：http://yx.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://lc.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fo.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qq.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://gd.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ch.szxytkj.cn

================================================================================
来源：http://qj.newstarts.cn

H. 异常与错误处理
来源：http://yn.shxzskj.cn

================================================================================
来源：http://gk.szsharing.cn

[H01] try / catch 基础
来源：http://aj.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yu.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uj.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ax.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gd.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://no.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fe.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gv.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qt.asd995.cn

[H02] finally / ensure 收尾
来源：http://fx.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zz.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cn.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yb.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mx.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tr.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lk.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jn.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fd.bjjhwx.cn

[H03] 主动抛出异常
来源：http://pg.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://gn.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bg.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://sy.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://ku.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ce.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://se.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tt.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gz.shxzukj.cn

[H04] 自定义异常类型
来源：http://mm.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://vx.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ti.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://th.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://ib.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://pd.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cm.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://mf.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://uc.lnxyls.cn

[H05] 捕获特定类型
来源：http://aj.panjiajie.cn

Py:   except ValueError as e:
来源：http://dc.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://go.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://ta.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://il.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://rm.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://af.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://xg.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fp.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://jc.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://gb.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kd.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qc.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ld.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lx.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dl.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://ib.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://vi.hahajie.cn

[H07] 断言
来源：http://tl.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://ef.9csxet.cn

PHP:  assert($x > 0);
来源：http://yv.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://tn.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://zv.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://dy.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bm.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rc.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://wk.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://dw.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://rh.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xg.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://sg.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://br.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sv.nicolike.cn

Go:   err.Error()
来源：http://yx.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://pb.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ph.chemitech.net.cn

[H09] 带错误码的异常
来源：http://yb.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xt.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://he.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ui.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ht.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sq.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fs.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yj.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rt.yuexingan06.cn

[H10] 资源自动释放
来源：http://sg.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://an.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gd.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fc.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oi.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dr.521024.cn

Go:   defer f.Close()
来源：http://ta.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qw.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rt.jctech888.com.cn

================================================================================
来源：http://vo.nicolike.cn

I. 正则表达式
来源：http://qf.yuexingan06.cn

================================================================================
来源：http://zb.chemitech.net.cn

[I01] 判断是否匹配
来源：http://ol.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rf.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vr.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://af.szsharing.cn

TS:   /\d+/.test(s)
来源：http://pn.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ap.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qs.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://hn.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xp.shxzukj.cn

[I02] 提取所有匹配
来源：http://bk.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://zk.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ew.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wo.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://ce.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xy.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lo.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://we.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fv.haigaiapp.cn

[I03] 提取捕获分组
来源：http://ch.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dp.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ru.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://js.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ub.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yo.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://da.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ph.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pj.szxytkj.cn

[I04] 正则替换
来源：http://vx.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://je.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ob.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rq.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fr.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ww.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vq.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vo.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gg.nicolike.cn

[I05] 按正则拆分
来源：http://si.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yj.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jm.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://ap.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://yr.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://gw.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://at.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fk.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rf.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qv.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nd.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fm.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wj.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hf.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tm.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jw.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dy.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zl.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://xl.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://im.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wi.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kt.haigaiapp.cn

TS:   /error/gim
来源：http://co.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dw.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wi.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://ux.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mu.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://ct.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dy.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sz.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bk.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iv.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tq.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://at.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lv.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xh.bookmarksfly.cn

================================================================================
来源：http://mv.jianghongdianzi.cn

J. 日期与时间
来源：http://vk.chemitech.net.cn

================================================================================
来源：http://gv.muxihuayi.cn

[J01] 获取当前时间
来源：http://we.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hh.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iq.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://yp.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://lw.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://le.szxytkj.cn

Go:   time.Now()
来源：http://ch.haigaiapp.cn

Ruby: Time.now
来源：http://lz.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://on.szsharing.cn

[J02] 格式化输出
来源：http://ed.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cz.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pd.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zy.huanxung.cn

TS:   d.toISOString()
来源：http://ep.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://es.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hr.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://td.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jg.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://ei.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zh.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nk.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://mp.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://ns.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ul.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yr.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ht.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dr.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://nn.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ez.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mv.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ia.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yw.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jr.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oq.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fv.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gn.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://ai.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://vp.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gs.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sm.bookmarksfly.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qf.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://gl.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dy.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://ol.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yw.gzmigu.cn

[J06] 计算两时间之差
来源：http://hf.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://cq.shxzukj.cn

PHP:  $end->diff($start)->days;
来源：http://ql.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hy.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vb.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hq.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ep.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://yx.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://ow.bjjhwx.cn

[J07] 比较两个日期
来源：http://za.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://zj.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fr.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nv.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://go.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zm.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://px.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://in.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://os.szxytkj.cn

[J08] 提取年月日与星期
来源：http://qt.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vz.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ed.nszjky.cn


<!-- 参考信息 -->