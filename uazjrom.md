代发 wailian999

TS:   public / protected / private
来源：http://sx.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://ow.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kn.chemitech.net.cn

Ruby: public / protected / private
来源：http://en.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://xy.huixinmuqiang.cn

[G11] getter / setter
来源：http://it.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://xm.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yh.521024.cn

JS:   get name() { return this._name; }
来源：http://hz.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://xi.shxzukj.cn

Java: public String getName() { return name; }
来源：http://wb.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hd.shxzukj.cn

Ruby: attr_accessor :name
来源：http://rd.521024.cn

C#:   public string Name { get; set; }
来源：http://zt.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://fd.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://ag.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sg.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://vy.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://xw.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://tm.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dj.szsharing.cn

Ruby: def to_s; @name; end
来源：http://tl.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://pr.szxytkj.cn

[G13] 判断对象类型
来源：http://br.9csxet.cn

Py:   isinstance(u, User)
来源：http://xl.newstarts.cn

PHP:  $u instanceof User
来源：http://lb.hnjuh.cn

JS:   u instanceof User
来源：http://im.chemitech.net.cn

TS:   u instanceof User
来源：http://pi.shxzukj.cn

Java: u instanceof User
来源：http://uj.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oz.nicolike.cn

Ruby: u.is_a?(User)
来源：http://bx.szsharing.cn

C#:   u is User
来源：http://kl.hnjuh.cn

[G14] 数据类 / record
来源：http://wc.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cc.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://pa.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bd.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://yr.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://qe.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://bz.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wc.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://xo.yuntaijiaju.cn

[G15] 枚举
来源：http://by.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://td.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mi.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jc.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qq.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://se.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ww.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://li.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tq.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://su.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ss.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://zf.huanxung.cn

JS:   Object.entries(obj)
来源：http://re.gzmigu.cn

TS:   Object.entries(obj)
来源：http://nb.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fr.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ie.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://mc.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://ws.colortex.cn

================================================================================
来源：http://gz.bjjhwx.cn

H. 异常与错误处理
来源：http://sm.shtwfgs.cn

================================================================================
来源：http://sy.newstarts.cn

[H01] try / catch 基础
来源：http://fl.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wr.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://af.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hv.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qp.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rs.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dw.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gk.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wg.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://qm.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://df.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tw.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gt.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://it.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://la.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lq.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hq.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ti.hnjuh.cn

[H03] 主动抛出异常
来源：http://os.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://wy.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tf.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://sk.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://uo.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ls.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zn.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ie.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sx.wgjwhj.cn

[H04] 自定义异常类型
来源：http://gv.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://ln.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ov.huanxung.cn

JS:   class MyError extends Error {}
来源：http://ga.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://ll.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://wl.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ts.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://ep.newstarts.cn

C#:   class MyException : Exception {}
来源：http://dh.muxihuayi.cn

[H05] 捕获特定类型
来源：http://ig.wgjwhj.cn

Py:   except ValueError as e:
来源：http://tv.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uu.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://lq.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://fk.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://df.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yw.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://ly.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ni.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://oi.9csxet.cn

Py:   value = d.get("k") or default
来源：http://hu.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ow.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wa.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yh.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kd.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://la.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://sv.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://ht.colortex.cn

[H07] 断言
来源：http://oo.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ur.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://rh.nicolike.cn

JS:   console.assert(x > 0);
来源：http://mf.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://zv.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://zm.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yg.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hj.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://he.521024.cn

[H08] 获取错误信息与堆栈
来源：http://vb.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://sf.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mx.nicolike.cn

JS:   e.message;  e.stack
来源：http://yo.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ie.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sm.bookmarksfly.cn

Go:   err.Error()
来源：http://hz.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://xz.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://vn.nicolike.cn

[H09] 带错误码的异常
来源：http://ur.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sm.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rj.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ix.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yn.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bg.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zi.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sz.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mh.yuexingan06.cn

[H10] 资源自动释放
来源：http://vf.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mc.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xj.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hn.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nl.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cj.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://zn.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bp.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xv.jctech888.com.cn

================================================================================
来源：http://ga.nicolike.cn

I. 正则表达式
来源：http://xi.muxihuayi.cn

================================================================================
来源：http://zw.nicolike.cn

[I01] 判断是否匹配
来源：http://tp.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://na.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dz.nicolike.cn

JS:   /\d+/.test(s)
来源：http://wb.asd995.cn

TS:   /\d+/.test(s)
来源：http://al.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vu.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ji.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://pa.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bq.shxzukj.cn

[I02] 提取所有匹配
来源：http://yn.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://ds.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zg.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jv.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://kp.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rf.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dy.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://ss.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iw.hahajie.cn

[I03] 提取捕获分组
来源：http://oq.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hb.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mm.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ri.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pm.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jd.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zt.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://en.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://he.bjjhwx.cn

[I04] 正则替换
来源：http://ln.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://on.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qr.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://px.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://af.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://os.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tg.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://so.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rm.bjjhwx.cn

[I05] 按正则拆分
来源：http://xs.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ay.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uc.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://wg.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://uw.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://gk.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bx.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yx.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rz.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xg.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nv.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rh.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://up.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zo.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ij.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jg.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iw.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xq.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://kj.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tv.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://by.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nh.huixinmuqiang.cn

TS:   /error/gim
来源：http://gq.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yy.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fh.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://xp.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oe.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://dm.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hq.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ft.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yf.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oh.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uy.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ws.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ok.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pm.yuexingan06.cn

================================================================================
来源：http://yz.shtwfgs.cn

J. 日期与时间
来源：http://gb.haigaiapp.cn

================================================================================
来源：http://sw.nicolike.cn

[J01] 获取当前时间
来源：http://lk.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rx.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qk.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://ij.newstarts.cn

TS:   new Date();  Date.now()
来源：http://ts.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cc.9csxet.cn

Go:   time.Now()
来源：http://qz.shtwfgs.cn

Ruby: Time.now
来源：http://au.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kt.huixiangedu.cn

[J02] 格式化输出
来源：http://nc.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nt.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wt.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wv.wgjwhj.cn

TS:   d.toISOString()
来源：http://ka.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zv.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://av.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rd.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hq.newstarts.cn

[J03] 字符串解析为日期
来源：http://qc.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ns.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ab.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://ww.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://ql.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gr.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aa.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://et.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vk.9csxet.cn

[J04] 时间戳与日期互转
来源：http://lf.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aj.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ib.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://co.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xx.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vf.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qm.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jl.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nb.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://fj.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://rz.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wb.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oe.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kj.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://mx.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zy.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://ww.gzmigu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xh.szxytkj.cn

[J06] 计算两时间之差
来源：http://hk.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://pq.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://ft.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kd.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fh.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ss.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://md.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://zd.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://bi.yuexingan06.cn

[J07] 比较两个日期
来源：http://xw.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://wc.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bk.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nf.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fa.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uy.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dl.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://it.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ob.shxzukj.cn

[J08] 提取年月日与星期
来源：http://qa.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xt.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bm.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://my.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ub.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ck.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pa.yuexingan06.cn


<!-- 参考信息 -->