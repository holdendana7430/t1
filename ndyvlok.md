代发 wailian999

TS:   public / protected / private
来源：http://rm.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://il.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gs.haigaiapp.cn

Ruby: public / protected / private
来源：http://qg.shxzskj.cn

C#:   public / protected / private / internal
来源：http://zy.newstarts.cn

[G11] getter / setter
来源：http://rf.hahajie.cn

Py:   @property 与 @x.setter
来源：http://jq.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ji.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://zg.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://ns.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://xr.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://le.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://ag.colortex.cn

C#:   public string Name { get; set; }
来源：http://md.colortex.cn

[G12] 对象转字符串
来源：http://co.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://ok.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ys.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://na.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://dn.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://vg.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://re.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://qq.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://dc.asd995.cn

[G13] 判断对象类型
来源：http://vc.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://uu.jctech888.com.cn

PHP:  $u instanceof User
来源：http://im.chemitech.net.cn

JS:   u instanceof User
来源：http://pn.wgjwhj.cn

TS:   u instanceof User
来源：http://fp.chemitech.net.cn

Java: u instanceof User
来源：http://da.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dx.newstarts.cn

Ruby: u.is_a?(User)
来源：http://gf.nszjky.cn

C#:   u is User
来源：http://tk.panjiajie.cn

[G14] 数据类 / record
来源：http://sd.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ei.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://wy.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ed.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ym.9csxet.cn

Java: record User(String name, int age) {}
来源：http://lf.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://iv.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lz.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://xz.nszjky.cn

[G15] 枚举
来源：http://rf.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pf.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gt.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ey.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wx.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://ym.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hy.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://lx.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ka.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://iv.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://be.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://ku.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://xc.521024.cn

TS:   Object.entries(obj)
来源：http://ki.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iv.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xu.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://ic.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://sk.huanxung.cn

================================================================================
来源：http://jk.nszjky.cn

H. 异常与错误处理
来源：http://ug.huixinmuqiang.cn

================================================================================
来源：http://zk.panjiajie.cn

[H01] try / catch 基础
来源：http://fj.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hg.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hv.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tk.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tf.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gg.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bf.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sg.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ae.szsharing.cn

[H02] finally / ensure 收尾
来源：http://el.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rg.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ml.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ip.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mc.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uq.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hq.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fb.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hy.bjjhwx.cn

[H03] 主动抛出异常
来源：http://vk.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://ps.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dn.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://tm.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://xb.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yn.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yt.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gi.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lg.panjiajie.cn

[H04] 自定义异常类型
来源：http://dg.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://ub.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bt.nszjky.cn

JS:   class MyError extends Error {}
来源：http://zz.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://tl.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://lt.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lv.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://uz.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://vs.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://zb.yuexingan06.cn

Py:   except ValueError as e:
来源：http://np.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mi.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://ee.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://jg.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://ka.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cc.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://gv.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lq.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://cm.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://rv.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://aa.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ow.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://od.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fv.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://md.huanxung.cn

Ruby: d&.dig(:a, :b)
来源：http://au.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://wx.panjiajie.cn

[H07] 断言
来源：http://vu.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://iq.huanxung.cn

PHP:  assert($x > 0);
来源：http://ou.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://bj.hahajie.cn

TS:   console.assert(x > 0);
来源：http://sy.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://nj.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://df.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wy.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://gw.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ri.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://mp.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mx.hnjuh.cn

JS:   e.message;  e.stack
来源：http://sd.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ui.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mx.nicolike.cn

Go:   err.Error()
来源：http://ws.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://it.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://xq.shxzskj.cn

[H09] 带错误码的异常
来源：http://ds.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oi.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mk.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wi.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jw.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qz.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yq.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xv.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bs.hahajie.cn

[H10] 资源自动释放
来源：http://co.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zh.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bp.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pn.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mo.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mr.yuexingan06.cn

Go:   defer f.Close()
来源：http://wf.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ei.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zy.szsharing.cn

================================================================================
来源：http://hf.hnjuh.cn

I. 正则表达式
来源：http://rw.lnxyls.cn

================================================================================
来源：http://ff.huixiangedu.cn

[I01] 判断是否匹配
来源：http://ei.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cg.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mp.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://dp.szsharing.cn

TS:   /\d+/.test(s)
来源：http://ky.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dt.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ej.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://zr.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lt.wgjwhj.cn

[I02] 提取所有匹配
来源：http://pu.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://mo.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uv.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ng.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://rw.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oj.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lt.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://fh.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ll.shtwfgs.cn

[I03] 提取捕获分组
来源：http://vl.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hv.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yg.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cf.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://od.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bb.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mq.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rd.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ci.shxzukj.cn

[I04] 正则替换
来源：http://uq.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://te.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://br.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ml.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xb.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uu.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dd.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zk.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ro.asd995.cn

[I05] 按正则拆分
来源：http://ba.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oe.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dw.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://gk.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://ut.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://lg.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uo.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lz.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zu.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jx.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wp.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pz.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hk.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gg.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nt.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ru.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eu.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ii.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://zu.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xy.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zk.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ku.colortex.cn

TS:   /error/gim
来源：http://yb.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dk.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cf.asd995.cn

Ruby: s.scan(/error/i)
来源：http://zj.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nc.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://wh.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pg.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vo.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://id.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mj.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mk.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qc.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gk.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chemitech.net.cn

================================================================================
来源：http://iw.lnxyls.cn

J. 日期与时间
来源：http://si.shxzukj.cn

================================================================================
来源：http://js.panjiajie.cn

[J01] 获取当前时间
来源：http://jm.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ct.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eg.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://vi.huanxung.cn

TS:   new Date();  Date.now()
来源：http://oq.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yz.nszjky.cn

Go:   time.Now()
来源：http://pa.huixiangedu.cn

Ruby: Time.now
来源：http://ju.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zi.chemitech.net.cn

[J02] 格式化输出
来源：http://rn.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ur.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cn.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kn.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://gj.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://py.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bt.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hh.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aj.panjiajie.cn

[J03] 字符串解析为日期
来源：http://bp.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yy.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tf.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ux.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://qy.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sm.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://af.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://ge.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vs.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://jd.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://te.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vm.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hk.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fp.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xq.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ez.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ld.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oe.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://iz.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://ax.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://na.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wd.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fe.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ks.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://um.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://zo.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ol.shxzukj.cn

[J06] 计算两时间之差
来源：http://qb.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://dc.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://gd.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fb.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vn.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gd.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://vo.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://xh.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://ne.huanxung.cn

[J07] 比较两个日期
来源：http://ky.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://rr.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yo.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wh.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ky.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://li.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sa.hahajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ez.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://kb.szsharing.cn

[J08] 提取年月日与星期
来源：http://xv.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mi.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ba.asd995.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yk.hahajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lt.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lz.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kr.jctech888.com.cn


<!-- 参考信息 -->