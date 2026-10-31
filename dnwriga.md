代发 wailian999

TS:   public / protected / private
来源：http://vw.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://ar.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://az.wgjwhj.cn

Ruby: public / protected / private
来源：http://dq.521024.cn

C#:   public / protected / private / internal
来源：http://vq.panjiajie.cn

[G11] getter / setter
来源：http://je.521024.cn

Py:   @property 与 @x.setter
来源：http://qa.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bd.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://kg.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://kh.nicolike.cn

Java: public String getName() { return name; }
来源：http://zp.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vo.huanxung.cn

Ruby: attr_accessor :name
来源：http://lo.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://zm.muxihuayi.cn

[G12] 对象转字符串
来源：http://mx.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://ix.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lw.nicolike.cn

JS:   toString() { return this.name; }
来源：http://po.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://ef.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://tp.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ra.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://lc.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://uh.shtwfgs.cn

[G13] 判断对象类型
来源：http://ix.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://dv.nszjky.cn

PHP:  $u instanceof User
来源：http://fk.nicolike.cn

JS:   u instanceof User
来源：http://id.wgjwhj.cn

TS:   u instanceof User
来源：http://am.chemitech.net.cn

Java: u instanceof User
来源：http://kz.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qu.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://sa.521024.cn

C#:   u is User
来源：http://tv.nicolike.cn

[G14] 数据类 / record
来源：http://bj.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gi.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ej.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fh.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://ij.521024.cn

Java: record User(String name, int age) {}
来源：http://ts.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://gh.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gl.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://gw.newstarts.cn

[G15] 枚举
来源：http://tp.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ya.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://db.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cj.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jo.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://ll.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fc.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://xt.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ne.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://wn.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yu.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://hf.szsharing.cn

JS:   Object.entries(obj)
来源：http://hq.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://vx.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uv.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yx.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://oe.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://wt.jianghongdianzi.cn

================================================================================
来源：http://lg.shtwfgs.cn

H. 异常与错误处理
来源：http://mc.hahajie.cn

================================================================================
来源：http://bi.gzmigu.cn

[H01] try / catch 基础
来源：http://qb.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vo.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rz.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pb.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lh.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://va.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rv.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dc.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://df.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://qv.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://no.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tl.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mo.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vy.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sy.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hq.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ky.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fl.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://es.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://hi.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tp.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://fe.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://pa.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ae.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rs.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yo.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://av.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://tz.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://uk.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bg.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://mb.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://vl.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://wh.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wg.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://uf.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://wt.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://eb.shtwfgs.cn

Py:   except ValueError as e:
来源：http://yn.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cb.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://wu.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://pm.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://qq.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sf.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://bx.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uy.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://cj.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://fv.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kn.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ug.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pb.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ry.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ja.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://sh.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://ii.huixinmuqiang.cn

[H07] 断言
来源：http://ow.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://qc.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://cd.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ug.521024.cn

TS:   console.assert(x > 0);
来源：http://vg.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://dy.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sx.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wc.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://ei.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://jt.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://gy.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ya.shxzskj.cn

JS:   e.message;  e.stack
来源：http://fe.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jg.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://co.bjjhwx.cn

Go:   err.Error()
来源：http://pz.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://pn.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://ih.bjjhwx.cn

[H09] 带错误码的异常
来源：http://kh.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fr.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gm.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qc.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vp.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uo.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jf.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xw.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zp.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://oi.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fe.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vl.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pv.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ly.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qo.asd995.cn

Go:   defer f.Close()
来源：http://ul.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ry.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bj.huixiangedu.cn

================================================================================
来源：http://rn.shxzskj.cn

I. 正则表达式
来源：http://cp.jctech888.com.cn

================================================================================
来源：http://ei.lnxyls.cn

[I01] 判断是否匹配
来源：http://xy.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nk.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jn.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://mu.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://oz.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oq.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xn.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://xx.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nt.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://zu.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://he.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://do.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eg.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://ae.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ul.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ze.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://ez.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xc.wgjwhj.cn

[I03] 提取捕获分组
来源：http://vk.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ak.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://um.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rb.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uo.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cd.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gq.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pt.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zw.nszjky.cn

[I04] 正则替换
来源：http://mr.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ar.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ql.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lc.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://os.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jv.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rd.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yi.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nr.bookmarksfly.cn

[I05] 按正则拆分
来源：http://df.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vs.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qo.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://bh.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://mk.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://nl.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ul.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ry.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ah.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ni.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qn.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xs.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sm.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ud.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rv.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ni.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ed.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uc.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://ib.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wh.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fg.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oh.colortex.cn

TS:   /error/gim
来源：http://iq.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vx.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ph.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://az.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ch.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ra.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wv.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mw.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ib.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ay.yuntaijiaju.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aa.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rc.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pp.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ea.9csxet.cn

================================================================================
来源：http://tf.newstarts.cn

J. 日期与时间
来源：http://vg.yuexingan06.cn

================================================================================
来源：http://rq.shxzskj.cn

[J01] 获取当前时间
来源：http://ih.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wf.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gx.huanxung.cn

JS:   new Date();  Date.now()
来源：http://if.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ao.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vh.jctech888.com.cn

Go:   time.Now()
来源：http://ow.jianghongdianzi.cn

Ruby: Time.now
来源：http://em.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wy.nicolike.cn

[J02] 格式化输出
来源：http://zw.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sx.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zz.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gz.bjjhwx.cn

TS:   d.toISOString()
来源：http://od.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iu.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://og.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yd.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wg.shxzukj.cn

[J03] 字符串解析为日期
来源：http://ir.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sh.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uu.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://xz.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://ao.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qi.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ku.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://fd.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sx.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://bo.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qd.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tf.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rl.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fr.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pc.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ci.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pq.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ih.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://vz.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://wg.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yg.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yf.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gx.521024.cn

Java: LocalDate.now().plusDays(7)
来源：http://pd.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://st.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://ta.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ak.chemitech.net.cn

[J06] 计算两时间之差
来源：http://qd.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://jd.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://qq.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bd.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fd.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tc.521024.cn

Go:   end.Sub(start).Hours()
来源：http://fj.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://ih.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://uh.9csxet.cn

[J07] 比较两个日期
来源：http://vf.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ok.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://we.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mz.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lk.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gn.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rk.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zp.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://ec.huanxung.cn

[J08] 提取年月日与星期
来源：http://if.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yq.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vp.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gd.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qt.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ye.shxzukj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pz.bookmarksfly.cn


<!-- 参考信息 -->