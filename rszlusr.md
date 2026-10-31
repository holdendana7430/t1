代发 wailian999

TS:   public / protected / private
来源：http://vw.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://ih.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ar.shtwfgs.cn

Ruby: public / protected / private
来源：http://sn.szsharing.cn

C#:   public / protected / private / internal
来源：http://xt.huixiangedu.cn

[G11] getter / setter
来源：http://nb.521024.cn

Py:   @property 与 @x.setter
来源：http://iv.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ju.colortex.cn

JS:   get name() { return this._name; }
来源：http://hw.521024.cn

TS:   get name(): string { return this._name; }
来源：http://pr.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://zx.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sh.shxzskj.cn

Ruby: attr_accessor :name
来源：http://ii.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://ds.hahajie.cn

[G12] 对象转字符串
来源：http://ql.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://xr.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mw.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://wt.521024.cn

TS:   toString(): string { return this.name; }
来源：http://mu.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://mv.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sw.hahajie.cn

Ruby: def to_s; @name; end
来源：http://le.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://fx.chemitech.net.cn

[G13] 判断对象类型
来源：http://ps.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://pf.chemitech.net.cn

PHP:  $u instanceof User
来源：http://ns.jctech888.com.cn

JS:   u instanceof User
来源：http://eb.huixiangedu.cn

TS:   u instanceof User
来源：http://ro.shtwfgs.cn

Java: u instanceof User
来源：http://gq.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uf.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://zv.hnjuh.cn

C#:   u is User
来源：http://ax.szxytkj.cn

[G14] 数据类 / record
来源：http://kt.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ge.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://le.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ke.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://kj.asd995.cn

Java: record User(String name, int age) {}
来源：http://xk.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://qb.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xw.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://tg.jctech888.com.cn

[G15] 枚举
来源：http://dn.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wm.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fd.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mj.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gb.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://hc.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jj.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://xt.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sx.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://ws.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vz.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://kn.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://vc.asd995.cn

TS:   Object.entries(obj)
来源：http://lc.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ul.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://df.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://et.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://qr.lnxyls.cn

================================================================================
来源：http://sc.newstarts.cn

H. 异常与错误处理
来源：http://gt.hnjuh.cn

================================================================================
来源：http://mp.chemitech.net.cn

[H01] try / catch 基础
来源：http://wz.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://di.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kz.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ee.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ju.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lj.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fd.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zx.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pm.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://aa.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dw.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sa.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yw.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gl.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kn.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pi.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tt.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rw.panjiajie.cn

[H03] 主动抛出异常
来源：http://sm.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://sn.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xq.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://bc.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://bc.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://na.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pw.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mh.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sc.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://mu.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://gv.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vh.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://gt.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://dn.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://hm.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ig.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://ix.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://dl.wgjwhj.cn

[H05] 捕获特定类型
来源：http://ad.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://ja.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ux.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://ed.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://vy.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://xz.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qf.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://jc.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yt.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://ah.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://ym.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tv.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://km.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nc.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pb.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yz.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://sk.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://yb.shxzskj.cn

[H07] 断言
来源：http://by.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://zn.hnjuh.cn

PHP:  assert($x > 0);
来源：http://yg.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://hd.szsharing.cn

TS:   console.assert(x > 0);
来源：http://es.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://fw.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uu.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tp.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://tn.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://bv.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://yj.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mk.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://ld.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ee.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kh.yuntaijiaju.cn

Go:   err.Error()
来源：http://hn.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://wp.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://jx.521024.cn

[H09] 带错误码的异常
来源：http://rm.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rj.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pm.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yk.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zy.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iy.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tk.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tm.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://up.521024.cn

[H10] 资源自动释放
来源：http://ya.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ab.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kx.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sc.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zr.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bz.panjiajie.cn

Go:   defer f.Close()
来源：http://mp.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pl.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://va.gzmigu.cn

================================================================================
来源：http://sy.haigaiapp.cn

I. 正则表达式
来源：http://st.bookmarksfly.cn

================================================================================
来源：http://ej.9csxet.cn

[I01] 判断是否匹配
来源：http://mb.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nj.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://db.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://oo.asd995.cn

TS:   /\d+/.test(s)
来源：http://rq.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vo.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gl.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://ob.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lx.nicolike.cn

[I02] 提取所有匹配
来源：http://vf.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://zm.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vh.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pf.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://bc.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oc.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ad.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://yw.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sd.shxzskj.cn

[I03] 提取捕获分组
来源：http://ir.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wc.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://if.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xf.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://en.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ap.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lc.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mq.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://js.muxihuayi.cn

[I04] 正则替换
来源：http://xb.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uu.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://al.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jf.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ar.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ad.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wg.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tv.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pz.szxytkj.cn

[I05] 按正则拆分
来源：http://ay.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ox.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dy.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://xq.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://gk.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://hv.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://df.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bm.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xa.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vb.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gv.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://of.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lh.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qb.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vu.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://on.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zy.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://po.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://id.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kn.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jv.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kk.lnxyls.cn

TS:   /error/gim
来源：http://rq.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mv.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xb.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://nf.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://af.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ys.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://df.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pp.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hi.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mj.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qr.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://me.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kx.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uw.9csxet.cn

================================================================================
来源：http://zv.huanxung.cn

J. 日期与时间
来源：http://tz.colortex.cn

================================================================================
来源：http://pp.panjiajie.cn

[J01] 获取当前时间
来源：http://xl.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ox.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pi.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://et.szsharing.cn

TS:   new Date();  Date.now()
来源：http://ah.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zy.521024.cn

Go:   time.Now()
来源：http://np.shtwfgs.cn

Ruby: Time.now
来源：http://ao.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jp.nszjky.cn

[J02] 格式化输出
来源：http://yt.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://co.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cf.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zk.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://sq.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ls.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bi.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lt.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uw.hahajie.cn

[J03] 字符串解析为日期
来源：http://ut.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yb.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mc.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://za.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://md.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://et.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cg.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://vn.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zg.huanxung.cn

[J04] 时间戳与日期互转
来源：http://mc.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pa.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sf.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ni.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fj.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jv.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fb.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://my.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hs.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://gq.asd995.cn

Py:   now + timedelta(days=7)
来源：http://fi.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ny.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qg.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bu.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://la.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pp.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://rq.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ml.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://oy.asd995.cn

Py:   (end - start).total_seconds()
来源：http://pz.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://vu.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vx.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xe.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://un.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://qk.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://oy.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://qb.nicolike.cn

[J07] 比较两个日期
来源：http://xr.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://cc.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://to.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yj.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jl.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ky.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://am.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bg.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://zc.hahajie.cn

[J08] 提取年月日与星期
来源：http://iu.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jw.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fk.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oo.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mi.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mb.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hx.colortex.cn


<!-- 参考信息 -->