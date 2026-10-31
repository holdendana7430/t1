代发 wailian999

[G10] 访问控制
来源：http://we.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://ly.521024.cn

PHP:  public / protected / private
来源：http://pd.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://jv.gzmigu.cn

TS:   public / protected / private
来源：http://ux.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://ps.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ll.szxytkj.cn

Ruby: public / protected / private
来源：http://zz.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://zs.szsharing.cn

[G11] getter / setter
来源：http://ke.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://sx.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://re.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://tp.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://mq.shxzskj.cn

Java: public String getName() { return name; }
来源：http://fq.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xa.hahajie.cn

Ruby: attr_accessor :name
来源：http://rr.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://ip.panjiajie.cn

[G12] 对象转字符串
来源：http://qf.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://lq.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jr.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://bp.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://xb.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://kk.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ym.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://ki.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://zv.colortex.cn

[G13] 判断对象类型
来源：http://gt.huanxung.cn

Py:   isinstance(u, User)
来源：http://uk.muxihuayi.cn

PHP:  $u instanceof User
来源：http://vq.521024.cn

JS:   u instanceof User
来源：http://mi.panjiajie.cn

TS:   u instanceof User
来源：http://px.chemitech.net.cn

Java: u instanceof User
来源：http://gt.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://li.hahajie.cn

Ruby: u.is_a?(User)
来源：http://rz.lnxyls.cn

C#:   u is User
来源：http://ry.shtwfgs.cn

[G14] 数据类 / record
来源：http://nx.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yz.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://kw.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lx.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://lc.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://qu.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://zl.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eo.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://zb.jctech888.com.cn

[G15] 枚举
来源：http://ih.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sa.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bt.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cu.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xt.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://sq.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vw.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://bv.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://go.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://sf.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://up.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://oz.panjiajie.cn

JS:   Object.entries(obj)
来源：http://yh.nszjky.cn

TS:   Object.entries(obj)
来源：http://li.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://be.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ka.szsharing.cn

Ruby: obj.instance_variables
来源：http://bv.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://up.nszjky.cn

================================================================================
来源：http://ue.bjjhwx.cn

H. 异常与错误处理
来源：http://lb.wgjwhj.cn

================================================================================
来源：http://wd.bookmarksfly.cn

[H01] try / catch 基础
来源：http://sz.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uk.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ea.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wr.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://li.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://js.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dl.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nj.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xz.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://pz.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gg.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://et.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fl.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fx.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zi.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bq.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rh.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://di.chemitech.net.cn

[H03] 主动抛出异常
来源：http://rt.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://hd.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ig.521024.cn

JS:   throw new Error("错误信息");
来源：http://hr.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://vj.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://es.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nv.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://su.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ah.shtwfgs.cn

[H04] 自定义异常类型
来源：http://nx.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://dz.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tm.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://ug.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ec.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://gg.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hr.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://nd.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://wg.yuexingan06.cn

[H05] 捕获特定类型
来源：http://at.chemitech.net.cn

Py:   except ValueError as e:
来源：http://zy.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gb.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ri.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://mc.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://ud.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pt.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://ip.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oe.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://xt.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://ve.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yq.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://id.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wz.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bx.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yo.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://jf.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://ba.chemitech.net.cn

[H07] 断言
来源：http://rd.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://mi.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://rr.9csxet.cn

JS:   console.assert(x > 0);
来源：http://tl.9csxet.cn

TS:   console.assert(x > 0);
来源：http://hs.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://ph.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yc.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ug.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://aa.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://ju.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://gg.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jy.nszjky.cn

JS:   e.message;  e.stack
来源：http://ps.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qz.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nl.panjiajie.cn

Go:   err.Error()
来源：http://lh.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://tr.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://qg.bjjhwx.cn

[H09] 带错误码的异常
来源：http://el.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sg.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://za.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ul.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uk.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iw.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://te.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pj.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sz.bjjhwx.cn

[H10] 资源自动释放
来源：http://jp.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cj.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pa.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zz.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nk.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://or.szxytkj.cn

Go:   defer f.Close()
来源：http://mr.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qd.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hk.huixinmuqiang.cn

================================================================================
来源：http://eo.huixiangedu.cn

I. 正则表达式
来源：http://wp.shtwfgs.cn

================================================================================
来源：http://zh.huixiangedu.cn

[I01] 判断是否匹配
来源：http://oc.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sk.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ks.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://nl.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://zg.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zo.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://di.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://mr.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ky.asd995.cn

[I02] 提取所有匹配
来源：http://qd.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://lp.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hu.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zj.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://nl.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fq.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mw.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://qt.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vd.jctech888.com.cn

[I03] 提取捕获分组
来源：http://rj.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uz.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://is.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://up.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://it.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xi.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mv.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zx.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ms.shtwfgs.cn

[I04] 正则替换
来源：http://en.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fu.huanxung.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://on.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jh.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lo.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hd.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gl.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fp.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zk.asd995.cn

[I05] 按正则拆分
来源：http://pi.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jt.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fn.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://ut.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://sy.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://db.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://te.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lk.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xz.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ow.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ce.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lb.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pz.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bn.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vq.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bw.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gv.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cf.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://fe.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://af.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jd.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rh.hahajie.cn

TS:   /error/gim
来源：http://lw.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lq.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ed.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://cg.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mt.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://js.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hg.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://le.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ar.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tl.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xb.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iy.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wb.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rb.hahajie.cn

================================================================================
来源：http://qp.panjiajie.cn

J. 日期与时间
来源：http://fn.chemitech.net.cn

================================================================================
来源：http://zn.huanxung.cn

[J01] 获取当前时间
来源：http://zz.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jq.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xq.szsharing.cn

JS:   new Date();  Date.now()
来源：http://og.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://by.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vx.shxzskj.cn

Go:   time.Now()
来源：http://vw.9csxet.cn

Ruby: Time.now
来源：http://tl.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rv.huanxung.cn

[J02] 格式化输出
来源：http://zu.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://no.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oh.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vh.asd995.cn

TS:   d.toISOString()
来源：http://va.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yo.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rd.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dg.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zl.newstarts.cn

[J03] 字符串解析为日期
来源：http://jg.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mb.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tc.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://ib.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://kn.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://op.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dn.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://kg.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hl.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ns.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://io.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wg.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ox.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wy.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rt.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jl.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nc.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wb.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://ho.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://fy.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://my.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://se.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rd.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://dr.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qt.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://ga.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mq.wgjwhj.cn

[J06] 计算两时间之差
来源：http://xz.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://dw.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://dx.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kp.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gg.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nv.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://og.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://kq.521024.cn

C#:   (end - start).TotalSeconds
来源：http://ev.huixiangedu.cn

[J07] 比较两个日期
来源：http://ll.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://nt.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gi.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rj.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ht.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fi.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gd.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hd.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://tj.521024.cn

[J08] 提取年月日与星期
来源：http://fr.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mb.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dh.bjjhwx.cn


<!-- 参考信息 -->