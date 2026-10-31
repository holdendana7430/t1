代发 wailian999

[G10] 访问控制
来源：http://sf.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ll.newstarts.cn

PHP:  public / protected / private
来源：http://lx.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://je.nszjky.cn

TS:   public / protected / private
来源：http://jd.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://fg.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xu.muxihuayi.cn

Ruby: public / protected / private
来源：http://lp.asd995.cn

C#:   public / protected / private / internal
来源：http://od.nicolike.cn

[G11] getter / setter
来源：http://qz.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://er.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dc.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://rz.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://dw.9csxet.cn

Java: public String getName() { return name; }
来源：http://qy.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zw.hnjuh.cn

Ruby: attr_accessor :name
来源：http://ip.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://hx.nicolike.cn

[G12] 对象转字符串
来源：http://qu.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://qi.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://em.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://dv.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://ca.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://dp.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sc.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://mz.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://oj.shxzukj.cn

[G13] 判断对象类型
来源：http://rs.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://ep.szxytkj.cn

PHP:  $u instanceof User
来源：http://lk.hnjuh.cn

JS:   u instanceof User
来源：http://wx.bjjhwx.cn

TS:   u instanceof User
来源：http://lq.jianghongdianzi.cn

Java: u instanceof User
来源：http://ct.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ur.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://po.shtwfgs.cn

C#:   u is User
来源：http://ef.huixiangedu.cn

[G14] 数据类 / record
来源：http://wr.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bn.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://lq.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://td.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://th.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://bv.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://az.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sr.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://ff.shtwfgs.cn

[G15] 枚举
来源：http://cc.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vm.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gb.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://br.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yt.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://qy.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gq.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://zd.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vm.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://sr.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ct.521024.cn

PHP:  get_object_vars($obj);
来源：http://bx.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://ia.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://cg.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vf.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gs.newstarts.cn

Ruby: obj.instance_variables
来源：http://db.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://qz.nicolike.cn

================================================================================
来源：http://xf.huanxung.cn

H. 异常与错误处理
来源：http://wg.jianghongdianzi.cn

================================================================================
来源：http://vy.lnxyls.cn

[H01] try / catch 基础
来源：http://cs.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aw.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iy.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hq.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ct.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ge.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zt.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aw.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rk.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://li.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xn.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bo.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iy.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bo.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vn.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://td.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ro.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uz.hnjuh.cn

[H03] 主动抛出异常
来源：http://ne.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://xh.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kd.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://zh.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://ib.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vq.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hj.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mk.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yx.shtwfgs.cn

[H04] 自定义异常类型
来源：http://nn.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://bh.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yd.newstarts.cn

JS:   class MyError extends Error {}
来源：http://jg.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://sr.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://xw.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://al.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://hl.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://yk.szxytkj.cn

[H05] 捕获特定类型
来源：http://he.lnxyls.cn

Py:   except ValueError as e:
来源：http://pi.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uq.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://hn.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://ci.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://kd.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qn.521024.cn

Ruby: rescue ArgumentError => e
来源：http://gh.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jn.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://wf.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://ly.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xa.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lw.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jp.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ga.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://va.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://ry.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://wq.szsharing.cn

[H07] 断言
来源：http://lr.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://yy.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://ze.nicolike.cn

JS:   console.assert(x > 0);
来源：http://vu.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://tq.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://cc.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kz.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jo.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://kp.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://gs.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://an.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ck.szsharing.cn

JS:   e.message;  e.stack
来源：http://pb.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://io.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://or.yuexingan06.cn

Go:   err.Error()
来源：http://zu.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://ic.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ay.9csxet.cn

[H09] 带错误码的异常
来源：http://xy.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kk.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ni.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hw.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://td.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ek.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yi.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jb.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://os.gzmigu.cn

[H10] 资源自动释放
来源：http://cq.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ym.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ht.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ly.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://na.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hp.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://xj.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xf.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yh.gzmigu.cn

================================================================================
来源：http://hu.asd995.cn

I. 正则表达式
来源：http://hl.shtwfgs.cn

================================================================================
来源：http://xh.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://bh.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vl.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hl.nszjky.cn

JS:   /\d+/.test(s)
来源：http://nf.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://kl.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tp.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yg.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://kj.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bi.newstarts.cn

[I02] 提取所有匹配
来源：http://jl.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://kf.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://df.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://js.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://hr.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pd.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uc.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://ll.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nk.hahajie.cn

[I03] 提取捕获分组
来源：http://az.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lx.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://el.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bw.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://um.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yi.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fy.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ej.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tw.nicolike.cn

[I04] 正则替换
来源：http://ow.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jr.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mv.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gy.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pb.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yl.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ot.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://om.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ea.shxzukj.cn

[I05] 按正则拆分
来源：http://ld.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hd.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yw.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://vq.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://og.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://dw.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rc.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://du.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jv.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xq.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gi.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kp.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vq.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jv.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ab.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ni.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://al.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ex.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://op.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wj.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yy.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kn.wgjwhj.cn

TS:   /error/gim
来源：http://op.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kw.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xd.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://yf.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ox.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://rx.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ic.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wu.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ma.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sg.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://px.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sa.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qo.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oi.yuexingan06.cn

================================================================================
来源：http://ow.colortex.cn

J. 日期与时间
来源：http://qf.bjjhwx.cn

================================================================================
来源：http://as.gzmigu.cn

[J01] 获取当前时间
来源：http://hb.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mp.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oz.nszjky.cn

JS:   new Date();  Date.now()
来源：http://ev.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://kj.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wy.asd995.cn

Go:   time.Now()
来源：http://ug.colortex.cn

Ruby: Time.now
来源：http://xc.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ho.shxzskj.cn

[J02] 格式化输出
来源：http://id.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xa.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qx.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cv.huixiangedu.cn

TS:   d.toISOString()
来源：http://cx.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://at.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://to.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lp.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zg.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://mb.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bi.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tx.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://iy.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://nk.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bo.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ox.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://oy.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ck.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://pa.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ov.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xs.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://np.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cs.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nu.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gn.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ps.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rd.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://av.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://do.newstarts.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pj.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ei.bjjhwx.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sc.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://ul.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rm.bjjhwx.cn

Ruby: Time.now + 7 * 86400
来源：http://oc.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xb.wgjwhj.cn

[J06] 计算两时间之差
来源：http://sv.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://qj.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://ok.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rx.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uo.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rg.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://px.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://pv.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://fs.gzmigu.cn

[J07] 比较两个日期
来源：http://dj.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://vs.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yo.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ph.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gp.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lt.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lr.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sr.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://ze.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://au.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bt.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ho.bjjhwx.cn


<!-- 参考信息 -->