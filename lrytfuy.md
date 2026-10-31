代发 wailian999

[G10] 访问控制
来源：http://dj.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://ux.newstarts.cn

PHP:  public / protected / private
来源：http://zv.szsharing.cn

JS:   #private 字段；其余公开
来源：http://ey.lnxyls.cn

TS:   public / protected / private
来源：http://cm.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://vz.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lf.asd995.cn

Ruby: public / protected / private
来源：http://si.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://mp.wgjwhj.cn

[G11] getter / setter
来源：http://tg.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ed.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qe.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://sy.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://qq.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://yr.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yx.nszjky.cn

Ruby: attr_accessor :name
来源：http://oe.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://uk.szxytkj.cn

[G12] 对象转字符串
来源：http://uw.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://xn.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dr.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://tg.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://cn.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://wp.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eg.hahajie.cn

Ruby: def to_s; @name; end
来源：http://mk.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://kt.gzmigu.cn

[G13] 判断对象类型
来源：http://nl.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://la.newstarts.cn

PHP:  $u instanceof User
来源：http://ax.nszjky.cn

JS:   u instanceof User
来源：http://hd.huixinmuqiang.cn

TS:   u instanceof User
来源：http://jc.521024.cn

Java: u instanceof User
来源：http://fe.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ai.521024.cn

Ruby: u.is_a?(User)
来源：http://kp.chemitech.net.cn

C#:   u is User
来源：http://le.bjjhwx.cn

[G14] 数据类 / record
来源：http://oh.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fi.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://gb.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zp.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://xd.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://om.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://th.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fc.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://xi.haigaiapp.cn

[G15] 枚举
来源：http://zd.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cv.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://he.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ee.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rc.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://cy.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ks.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://wn.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://li.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://vj.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ij.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://bg.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://qp.9csxet.cn

TS:   Object.entries(obj)
来源：http://yj.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://et.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tg.colortex.cn

Ruby: obj.instance_variables
来源：http://st.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ew.bjjhwx.cn

================================================================================
来源：http://rr.yuexingan06.cn

H. 异常与错误处理
来源：http://zh.huixiangedu.cn

================================================================================
来源：http://qt.hnjuh.cn

[H01] try / catch 基础
来源：http://tp.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ok.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wc.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ax.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ct.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ea.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ua.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ou.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kg.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://le.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ml.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pu.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nc.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fu.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xz.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ui.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tl.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rp.asd995.cn

[H03] 主动抛出异常
来源：http://dh.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://pj.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cp.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://nj.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://ga.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zl.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fu.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://er.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gj.asd995.cn

[H04] 自定义异常类型
来源：http://lw.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://jd.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vs.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://uu.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ju.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://ub.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ez.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://de.nszjky.cn

C#:   class MyException : Exception {}
来源：http://au.gzmigu.cn

[H05] 捕获特定类型
来源：http://mo.wgjwhj.cn

Py:   except ValueError as e:
来源：http://ya.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xu.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://or.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://qq.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://bs.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mr.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://nl.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ax.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://vi.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://rd.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sb.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vj.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xa.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fk.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bb.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://tj.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://nb.lnxyls.cn

[H07] 断言
来源：http://ib.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://ws.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://ru.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://pp.szsharing.cn

TS:   console.assert(x > 0);
来源：http://fc.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://hw.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jm.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ea.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://bq.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://dn.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://ac.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ku.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ni.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zs.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ht.shxzukj.cn

Go:   err.Error()
来源：http://ir.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://uo.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://rc.asd995.cn

[H09] 带错误码的异常
来源：http://zy.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ln.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dn.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kx.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wk.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mn.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yf.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://st.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kh.nicolike.cn

[H10] 资源自动释放
来源：http://cx.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dq.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wo.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xn.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sc.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uu.huanxung.cn

Go:   defer f.Close()
来源：http://uy.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bs.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nr.wgjwhj.cn

================================================================================
来源：http://ym.bjjhwx.cn

I. 正则表达式
来源：http://xv.wgjwhj.cn

================================================================================
来源：http://nv.jctech888.com.cn

[I01] 判断是否匹配
来源：http://be.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lx.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mo.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://op.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://ow.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gm.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lc.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://os.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://be.nicolike.cn

[I02] 提取所有匹配
来源：http://wu.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://mt.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wl.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zw.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://tu.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cy.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ze.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://vh.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wz.szsharing.cn

[I03] 提取捕获分组
来源：http://pv.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vp.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uf.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xs.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aa.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lh.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kg.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hj.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oe.521024.cn

[I04] 正则替换
来源：http://tp.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uv.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mb.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cj.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uc.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zc.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hq.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uw.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://uu.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dw.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fe.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://uy.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://tj.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://cs.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nt.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hj.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gj.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ik.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uv.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hg.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rn.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://us.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yq.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nq.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qu.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pz.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://ww.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bu.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pm.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ta.muxihuayi.cn

TS:   /error/gim
来源：http://dt.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qq.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nj.521024.cn

Ruby: s.scan(/error/i)
来源：http://us.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xq.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://rr.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://da.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ag.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://js.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bj.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rs.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lo.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mn.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fs.szsharing.cn

================================================================================
来源：http://ef.huixiangedu.cn

J. 日期与时间
来源：http://xp.asd995.cn

================================================================================
来源：http://rh.9csxet.cn

[J01] 获取当前时间
来源：http://xe.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zg.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kk.hahajie.cn

JS:   new Date();  Date.now()
来源：http://dg.huanxung.cn

TS:   new Date();  Date.now()
来源：http://jh.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ft.huixinmuqiang.cn

Go:   time.Now()
来源：http://xw.hnjuh.cn

Ruby: Time.now
来源：http://zf.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gg.panjiajie.cn

[J02] 格式化输出
来源：http://mc.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qn.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://je.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nb.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://te.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qp.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vt.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jb.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dr.nicolike.cn

[J03] 字符串解析为日期
来源：http://sn.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fp.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jw.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://jw.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://mq.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pt.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sk.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://sl.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ow.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://ep.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ot.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tv.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gd.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ma.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://py.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mw.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oh.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xt.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://gj.asd995.cn

Py:   now + timedelta(days=7)
来源：http://mx.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hg.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vf.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xf.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://pk.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lx.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://wf.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jr.szsharing.cn

[J06] 计算两时间之差
来源：http://hz.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://wo.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://hz.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://re.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lg.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oe.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://ek.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://zq.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://kk.bjjhwx.cn

[J07] 比较两个日期
来源：http://kk.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://gw.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bo.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jx.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zn.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qf.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uq.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ll.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://pv.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://ms.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rh.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ho.lnxyls.cn


<!-- 参考信息 -->