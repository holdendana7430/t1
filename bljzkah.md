代发 wailian999

TS:   public / protected / private
来源：http://tm.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://hf.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tk.asd995.cn

Ruby: public / protected / private
来源：http://kt.huanxung.cn

C#:   public / protected / private / internal
来源：http://jc.shxzskj.cn

[G11] getter / setter
来源：http://ka.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://vd.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pg.hahajie.cn

JS:   get name() { return this._name; }
来源：http://nq.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://ii.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://qy.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zz.szsharing.cn

Ruby: attr_accessor :name
来源：http://th.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://oq.hahajie.cn

[G12] 对象转字符串
来源：http://cs.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://mq.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gu.colortex.cn

JS:   toString() { return this.name; }
来源：http://ok.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://zu.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://uc.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rp.521024.cn

Ruby: def to_s; @name; end
来源：http://fq.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://dt.colortex.cn

[G13] 判断对象类型
来源：http://bq.newstarts.cn

Py:   isinstance(u, User)
来源：http://tl.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://rx.newstarts.cn

JS:   u instanceof User
来源：http://cx.hahajie.cn

TS:   u instanceof User
来源：http://bw.szsharing.cn

Java: u instanceof User
来源：http://un.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ue.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://yk.hnjuh.cn

C#:   u is User
来源：http://ab.hnjuh.cn

[G14] 数据类 / record
来源：http://di.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cd.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://bf.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uf.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://xt.521024.cn

Java: record User(String name, int age) {}
来源：http://kc.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://ge.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://df.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://ei.asd995.cn

[G15] 枚举
来源：http://rc.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sq.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xd.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rl.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vu.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://mr.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hs.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://rr.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hu.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://ex.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cf.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://mk.lnxyls.cn

JS:   Object.entries(obj)
来源：http://rp.shxzskj.cn

TS:   Object.entries(obj)
来源：http://dm.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ok.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bg.lnxyls.cn

Ruby: obj.instance_variables
来源：http://on.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://eq.bjjhwx.cn

================================================================================
来源：http://qj.hahajie.cn

H. 异常与错误处理
来源：http://eq.hnjuh.cn

================================================================================
来源：http://ad.colortex.cn

[H01] try / catch 基础
来源：http://ns.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kv.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nt.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kh.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xd.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eo.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rh.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bx.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rn.nszjky.cn

[H02] finally / ensure 收尾
来源：http://qx.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://az.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ce.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mu.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ku.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ox.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sa.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eb.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://om.shxzskj.cn

[H03] 主动抛出异常
来源：http://fh.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://mx.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rg.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://yk.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://pd.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hq.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qz.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sp.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dj.bjjhwx.cn

[H04] 自定义异常类型
来源：http://mc.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://hc.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xt.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://cf.newstarts.cn

TS:   class MyError extends Error {}
来源：http://gi.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://dg.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aq.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://pe.hahajie.cn

C#:   class MyException : Exception {}
来源：http://xb.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://me.panjiajie.cn

Py:   except ValueError as e:
来源：http://ex.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ei.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://kj.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://ab.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://lh.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ke.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://yx.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://me.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://ln.nicolike.cn

Py:   value = d.get("k") or default
来源：http://nz.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ug.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ro.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bc.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bv.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fy.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://yd.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://or.newstarts.cn

[H07] 断言
来源：http://ip.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://fq.nszjky.cn

PHP:  assert($x > 0);
来源：http://vq.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://qq.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://dx.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://oq.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fi.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ok.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://rx.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://cv.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://vz.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fu.nicolike.cn

JS:   e.message;  e.stack
来源：http://om.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ml.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mu.huanxung.cn

Go:   err.Error()
来源：http://ow.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://hg.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://vo.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://li.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ve.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nq.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zl.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vz.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ae.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dd.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wv.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oe.haigaiapp.cn

[H10] 资源自动释放
来源：http://ic.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bm.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ep.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oj.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ox.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://th.shxzskj.cn

Go:   defer f.Close()
来源：http://be.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xm.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://js.nicolike.cn

================================================================================
来源：http://bs.newstarts.cn

I. 正则表达式
来源：http://qr.nszjky.cn

================================================================================
来源：http://uz.jctech888.com.cn

[I01] 判断是否匹配
来源：http://gd.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fr.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://df.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://kh.newstarts.cn

TS:   /\d+/.test(s)
来源：http://wk.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ux.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mn.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://vs.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ol.jctech888.com.cn

[I02] 提取所有匹配
来源：http://lb.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://vb.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ym.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fj.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://wk.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oo.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yq.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://yz.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://st.shxzukj.cn

[I03] 提取捕获分组
来源：http://gu.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kl.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ov.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://el.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ck.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ld.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eh.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pc.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dr.newstarts.cn

[I04] 正则替换
来源：http://cm.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ho.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vv.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xs.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gz.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kl.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vx.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://le.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.jctech888.com.cn

[I05] 按正则拆分
来源：http://il.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hr.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sk.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ui.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://tr.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://vq.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://do.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jp.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oj.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://um.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eh.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yn.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kp.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://la.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ff.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tq.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iq.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ld.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://tb.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ci.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pl.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jg.haigaiapp.cn

TS:   /error/gim
来源：http://dj.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vl.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sd.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://yq.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ro.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://hs.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fe.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mt.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qi.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yp.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pf.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ib.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sz.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://if.hahajie.cn

================================================================================
来源：http://sw.haigaiapp.cn

J. 日期与时间
来源：http://sq.bjjhwx.cn

================================================================================
来源：http://iv.nicolike.cn

[J01] 获取当前时间
来源：http://ak.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vt.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gx.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://ji.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://hu.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bm.wgjwhj.cn

Go:   time.Now()
来源：http://ju.shxzskj.cn

Ruby: Time.now
来源：http://qf.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oe.jctech888.com.cn

[J02] 格式化输出
来源：http://zq.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://in.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qa.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pw.huixiangedu.cn

TS:   d.toISOString()
来源：http://ua.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qg.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cd.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ae.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hh.gzmigu.cn

[J03] 字符串解析为日期
来源：http://ur.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qo.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://el.521024.cn

JS:   new Date("2024-01-02")
来源：http://ko.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://qh.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oy.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ro.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://pr.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ht.gzmigu.cn

[J04] 时间戳与日期互转
来源：http://ko.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ow.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ce.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ui.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ig.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vl.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yn.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yu.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://er.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://mi.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://ni.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sz.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nf.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nr.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://ow.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jm.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://di.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xj.bjjhwx.cn

[J06] 计算两时间之差
来源：http://fs.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://vf.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://lh.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yp.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cl.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zm.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://pm.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://je.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://qd.muxihuayi.cn

[J07] 比较两个日期
来源：http://ho.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://bl.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pv.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qf.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bf.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zg.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://br.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://al.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://ms.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://vk.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fr.yuexingan06.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hd.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bo.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vi.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pe.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rx.huanxung.cn


<!-- 参考信息 -->