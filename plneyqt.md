代发 wailian999

[G10] 访问控制
来源：http://vs.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://qn.521024.cn

PHP:  public / protected / private
来源：http://ir.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ej.bookmarksfly.cn

TS:   public / protected / private
来源：http://dv.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://ju.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ks.muxihuayi.cn

Ruby: public / protected / private
来源：http://av.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://pu.szxytkj.cn

[G11] getter / setter
来源：http://rr.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://yq.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qd.colortex.cn

JS:   get name() { return this._name; }
来源：http://um.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://ft.asd995.cn

Java: public String getName() { return name; }
来源：http://se.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bt.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://sy.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://wi.asd995.cn

[G12] 对象转字符串
来源：http://wb.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://jh.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fk.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://zq.521024.cn

TS:   toString(): string { return this.name; }
来源：http://il.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://ay.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vk.nicolike.cn

Ruby: def to_s; @name; end
来源：http://zl.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://gz.shxzukj.cn

[G13] 判断对象类型
来源：http://uc.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://xe.hnjuh.cn

PHP:  $u instanceof User
来源：http://hd.hahajie.cn

JS:   u instanceof User
来源：http://gh.szsharing.cn

TS:   u instanceof User
来源：http://ax.muxihuayi.cn

Java: u instanceof User
来源：http://rq.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mi.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://rn.jctech888.com.cn

C#:   u is User
来源：http://lp.9csxet.cn

[G14] 数据类 / record
来源：http://ng.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kb.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://rw.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tf.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://nv.asd995.cn

Java: record User(String name, int age) {}
来源：http://rj.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://js.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://td.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://yd.yuntaijiaju.cn

[G15] 枚举
来源：http://gu.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rv.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wi.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://km.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lh.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://jh.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lo.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://be.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hi.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://ud.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nr.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ch.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://xb.shxzskj.cn

TS:   Object.entries(obj)
来源：http://bw.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ck.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xk.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://og.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://gh.huanxung.cn

================================================================================
来源：http://or.colortex.cn

H. 异常与错误处理
来源：http://na.wgjwhj.cn

================================================================================
来源：http://fo.jctech888.com.cn

[H01] try / catch 基础
来源：http://jt.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ob.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ei.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sv.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://br.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dw.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://it.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dx.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ip.szsharing.cn

[H02] finally / ensure 收尾
来源：http://sp.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xk.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oa.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wx.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rf.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eu.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qs.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xt.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xz.nicolike.cn

[H03] 主动抛出异常
来源：http://li.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://mu.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dr.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://am.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://jn.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://re.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vo.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oa.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nw.newstarts.cn

[H04] 自定义异常类型
来源：http://hk.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ey.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pf.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://qc.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://zt.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://qq.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wg.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ux.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://mn.newstarts.cn

[H05] 捕获特定类型
来源：http://gf.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://ss.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sm.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://lg.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://tn.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ih.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://er.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://cj.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pz.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://yy.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://bo.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ub.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mb.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rk.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zf.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jh.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://ys.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://rx.haigaiapp.cn

[H07] 断言
来源：http://hi.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://rg.shxzukj.cn

PHP:  assert($x > 0);
来源：http://vu.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://za.szsharing.cn

TS:   console.assert(x > 0);
来源：http://dy.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://wg.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vb.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bv.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://zb.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://cn.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://vq.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gv.newstarts.cn

JS:   e.message;  e.stack
来源：http://je.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mb.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pr.gzmigu.cn

Go:   err.Error()
来源：http://pf.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://yj.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://ux.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://lg.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oj.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rh.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ot.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://on.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vw.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jg.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zx.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ig.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://pu.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hw.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ll.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sh.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ep.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uy.shxzukj.cn

Go:   defer f.Close()
来源：http://fn.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uc.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mb.huanxung.cn

================================================================================
来源：http://fw.hahajie.cn

I. 正则表达式
来源：http://zo.chemitech.net.cn

================================================================================
来源：http://yn.huanxung.cn

[I01] 判断是否匹配
来源：http://ww.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://di.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qv.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://iw.asd995.cn

TS:   /\d+/.test(s)
来源：http://ni.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://df.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rb.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://at.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cd.gzmigu.cn

[I02] 提取所有匹配
来源：http://dt.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://df.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hl.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ci.asd995.cn

TS:   s.match(/\d+/g)
来源：http://aa.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nx.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bc.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://em.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eq.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://po.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xr.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jf.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xe.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sg.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fr.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cw.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gj.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cc.szsharing.cn

[I04] 正则替换
来源：http://gg.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jd.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zg.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://st.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mz.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rd.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ep.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nx.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tw.gzmigu.cn

[I05] 按正则拆分
来源：http://yv.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://os.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eb.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://kb.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://as.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://zl.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wg.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zu.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aw.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hr.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zs.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wv.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ht.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bo.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mi.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ci.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ee.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ng.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://ws.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qe.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tp.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dd.colortex.cn

TS:   /error/gim
来源：http://va.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yo.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rq.521024.cn

Ruby: s.scan(/error/i)
来源：http://wo.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eo.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://xx.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eo.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mz.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ok.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bv.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kf.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rv.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gn.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hm.gzmigu.cn

================================================================================
来源：http://ft.hnjuh.cn

J. 日期与时间
来源：http://gb.haigaiapp.cn

================================================================================
来源：http://vr.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://ry.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qw.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bg.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://we.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://ob.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ql.gzmigu.cn

Go:   time.Now()
来源：http://gi.shxzskj.cn

Ruby: Time.now
来源：http://wx.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fa.521024.cn

[J02] 格式化输出
来源：http://av.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fm.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://er.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yx.szsharing.cn

TS:   d.toISOString()
来源：http://zh.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://il.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bx.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pt.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wy.huanxung.cn

[J03] 字符串解析为日期
来源：http://br.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wh.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lu.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://vl.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://ua.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qf.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cu.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://gy.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uo.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://qj.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wk.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ge.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zj.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ii.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://po.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yu.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ah.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dm.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://nd.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ce.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jy.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qo.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pr.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://gs.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yp.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://gb.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://js.nszjky.cn

[J06] 计算两时间之差
来源：http://as.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://hq.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://yn.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sf.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://np.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://va.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://bv.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://mq.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://xm.shxzskj.cn

[J07] 比较两个日期
来源：http://es.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://ea.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gd.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cj.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gb.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fx.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lk.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fa.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://sh.nicolike.cn

[J08] 提取年月日与星期
来源：http://ri.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vc.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dl.hahajie.cn


<!-- 参考信息 -->