代发 wailian999

Java: interface Shape { double area(); }
来源：http://ah.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://fn.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vn.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://lr.shtwfgs.cn

[G10] 访问控制
来源：http://po.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://my.szsharing.cn

PHP:  public / protected / private
来源：http://ov.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://gu.hnjuh.cn

TS:   public / protected / private
来源：http://mz.521024.cn

Java: public / protected / private / 默认包级
来源：http://jz.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gr.hnjuh.cn

Ruby: public / protected / private
来源：http://lb.szsharing.cn

C#:   public / protected / private / internal
来源：http://bi.shxzukj.cn

[G11] getter / setter
来源：http://wd.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://is.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oj.szsharing.cn

JS:   get name() { return this._name; }
来源：http://hs.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://ej.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://zi.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sg.szsharing.cn

Ruby: attr_accessor :name
来源：http://dx.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://bb.yuexingan06.cn

[G12] 对象转字符串
来源：http://cc.521024.cn

Py:   def __str__(self): return self.name
来源：http://qt.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xe.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://hc.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://ta.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://zn.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mi.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ow.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://pf.panjiajie.cn

[G13] 判断对象类型
来源：http://wj.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://ag.haigaiapp.cn

PHP:  $u instanceof User
来源：http://bp.bjjhwx.cn

JS:   u instanceof User
来源：http://oa.lnxyls.cn

TS:   u instanceof User
来源：http://vz.nicolike.cn

Java: u instanceof User
来源：http://yf.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nq.9csxet.cn

Ruby: u.is_a?(User)
来源：http://ix.szsharing.cn

C#:   u is User
来源：http://hq.gzmigu.cn

[G14] 数据类 / record
来源：http://ph.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rq.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://kp.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xp.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://ng.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://dx.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://kd.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ud.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://cr.jianghongdianzi.cn

[G15] 枚举
来源：http://ow.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ob.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tb.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uc.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mb.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://tr.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mu.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://jk.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://or.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://fq.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rz.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://jg.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://nj.9csxet.cn

TS:   Object.entries(obj)
来源：http://ga.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zi.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bn.szsharing.cn

Ruby: obj.instance_variables
来源：http://bd.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://fp.shxzskj.cn

================================================================================
来源：http://gy.huanxung.cn

H. 异常与错误处理
来源：http://fc.shxzukj.cn

================================================================================
来源：http://wb.bookmarksfly.cn

[H01] try / catch 基础
来源：http://hj.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mf.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yx.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ws.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xg.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kz.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xe.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://le.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ht.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://ec.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mv.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ig.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vt.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://od.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://en.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cs.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://db.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://al.shxzukj.cn

[H03] 主动抛出异常
来源：http://pf.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://be.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dg.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://nk.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://as.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xn.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jd.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oh.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hw.panjiajie.cn

[H04] 自定义异常类型
来源：http://zw.asd995.cn

Py:   class MyError(Exception): pass
来源：http://sy.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ks.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://zm.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://ue.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://kb.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eh.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://aw.szsharing.cn

C#:   class MyException : Exception {}
来源：http://bx.huanxung.cn

[H05] 捕获特定类型
来源：http://ab.szxytkj.cn

Py:   except ValueError as e:
来源：http://wy.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qm.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://mg.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://yf.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://ob.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rd.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://oo.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gv.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://ys.szsharing.cn

Py:   value = d.get("k") or default
来源：http://br.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ua.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fc.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://si.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://du.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://du.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://ua.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://ny.szsharing.cn

[H07] 断言
来源：http://fs.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://dc.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://xg.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://hj.newstarts.cn

TS:   console.assert(x > 0);
来源：http://xf.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://hb.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fw.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eh.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://br.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://fo.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://rp.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hw.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://yc.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bv.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ai.panjiajie.cn

Go:   err.Error()
来源：http://jv.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://ua.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://pp.9csxet.cn

[H09] 带错误码的异常
来源：http://ls.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tv.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bo.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gv.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://on.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ta.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://es.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wj.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bq.wgjwhj.cn

[H10] 资源自动释放
来源：http://qq.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zk.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://td.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vm.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gz.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sg.huixiangedu.cn

Go:   defer f.Close()
来源：http://lo.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hk.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gj.hahajie.cn

================================================================================
来源：http://om.chemitech.net.cn

I. 正则表达式
来源：http://kg.chemitech.net.cn

================================================================================
来源：http://fw.wgjwhj.cn

[I01] 判断是否匹配
来源：http://cd.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kk.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sf.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://ir.newstarts.cn

TS:   /\d+/.test(s)
来源：http://gf.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tt.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mg.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://ac.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ju.shxzskj.cn

[I02] 提取所有匹配
来源：http://hc.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://uw.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pw.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sf.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://yk.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rv.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fc.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://fb.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yl.colortex.cn

[I03] 提取捕获分组
来源：http://kz.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wy.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tg.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://it.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kz.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yy.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ex.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cv.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://za.newstarts.cn

[I04] 正则替换
来源：http://mo.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wp.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lj.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://by.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ui.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wb.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lw.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ac.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ph.muxihuayi.cn

[I05] 按正则拆分
来源：http://cl.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hu.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://za.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://we.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://xh.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://jv.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ix.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://np.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ng.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vk.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ls.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dc.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zi.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jj.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xg.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mb.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pu.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wp.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://wc.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fa.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wv.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pc.huanxung.cn

TS:   /error/gim
来源：http://ls.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://js.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fy.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://yl.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fr.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://nf.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pl.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hy.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ph.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dp.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qd.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://in.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qr.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nq.newstarts.cn

================================================================================
来源：http://gd.muxihuayi.cn

J. 日期与时间
来源：http://wh.hahajie.cn

================================================================================
来源：http://ys.asd995.cn

[J01] 获取当前时间
来源：http://pr.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vf.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bq.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://mx.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://mr.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qn.asd995.cn

Go:   time.Now()
来源：http://ma.9csxet.cn

Ruby: Time.now
来源：http://mk.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pi.huixinmuqiang.cn

[J02] 格式化输出
来源：http://rr.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bf.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kz.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kr.shxzskj.cn

TS:   d.toISOString()
来源：http://kh.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wq.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ib.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bz.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jh.colortex.cn

[J03] 字符串解析为日期
来源：http://ys.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yt.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://go.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://ei.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://yx.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://do.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tz.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://yj.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wi.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://jd.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tk.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ps.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vw.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ph.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lz.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rw.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dp.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ne.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://wj.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://wp.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hm.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vt.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sv.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://uj.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://of.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://ll.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kj.chemitech.net.cn

[J06] 计算两时间之差
来源：http://pu.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://up.521024.cn

PHP:  $end->diff($start)->days;
来源：http://oq.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rw.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wz.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oe.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://ua.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://zl.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://bf.hnjuh.cn

[J07] 比较两个日期
来源：http://iy.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://eg.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lc.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://im.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://po.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nv.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ls.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gf.szxytkj.cn


<!-- 参考信息 -->