代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://vn.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tg.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uk.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://io.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://vf.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://rc.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qk.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://rr.huanxung.cn

[G10] 访问控制
来源：http://tr.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://rx.shtwfgs.cn

PHP:  public / protected / private
来源：http://be.nicolike.cn

JS:   #private 字段；其余公开
来源：http://dd.asd995.cn

TS:   public / protected / private
来源：http://db.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://nj.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://py.szsharing.cn

Ruby: public / protected / private
来源：http://zn.asd995.cn

C#:   public / protected / private / internal
来源：http://qa.jctech888.com.cn

[G11] getter / setter
来源：http://rp.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://ho.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sj.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://pw.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://zn.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://od.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ke.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://zz.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://hd.shxzukj.cn

[G12] 对象转字符串
来源：http://id.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://ly.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uv.nszjky.cn

JS:   toString() { return this.name; }
来源：http://ov.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://up.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://ug.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fs.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://kp.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://qh.nicolike.cn

[G13] 判断对象类型
来源：http://st.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://hp.muxihuayi.cn

PHP:  $u instanceof User
来源：http://gd.shxzskj.cn

JS:   u instanceof User
来源：http://fw.jctech888.com.cn

TS:   u instanceof User
来源：http://sw.bjjhwx.cn

Java: u instanceof User
来源：http://bx.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rw.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://jx.haigaiapp.cn

C#:   u is User
来源：http://hh.hahajie.cn

[G14] 数据类 / record
来源：http://ub.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qt.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://dw.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qd.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://ao.9csxet.cn

Java: record User(String name, int age) {}
来源：http://rg.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://ja.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gm.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://jc.shtwfgs.cn

[G15] 枚举
来源：http://jk.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yj.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wz.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gg.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kv.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://et.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vc.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://kk.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ja.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://oq.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rk.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://ge.colortex.cn

JS:   Object.entries(obj)
来源：http://zn.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://jn.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ck.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ts.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://mj.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://vg.chemitech.net.cn

================================================================================
来源：http://kg.bjjhwx.cn

H. 异常与错误处理
来源：http://ff.gzmigu.cn

================================================================================
来源：http://pa.gzmigu.cn

[H01] try / catch 基础
来源：http://oy.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pr.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rg.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ab.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wk.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mb.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xw.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ro.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://po.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://on.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bn.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://or.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ax.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uu.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mh.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lf.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lg.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uq.muxihuayi.cn

[H03] 主动抛出异常
来源：http://zk.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://zi.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://by.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://so.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://xx.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://po.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ig.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://va.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hw.9csxet.cn

[H04] 自定义异常类型
来源：http://bh.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://bi.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hi.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://di.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://nd.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://jm.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mz.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://rd.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://vf.wgjwhj.cn

[H05] 捕获特定类型
来源：http://mv.chemitech.net.cn

Py:   except ValueError as e:
来源：http://oi.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ef.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://nn.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://us.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://fs.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ep.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://cw.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zl.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://sx.9csxet.cn

Py:   value = d.get("k") or default
来源：http://ax.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zb.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ct.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ed.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zi.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://so.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://he.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://ok.asd995.cn

[H07] 断言
来源：http://qd.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://rm.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ea.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://tk.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://zf.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://rr.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ok.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jr.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://un.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://am.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://my.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kt.gzmigu.cn

JS:   e.message;  e.stack
来源：http://mt.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ca.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://th.9csxet.cn

Go:   err.Error()
来源：http://jt.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://uq.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://rk.gzmigu.cn

[H09] 带错误码的异常
来源：http://ol.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jn.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zv.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eo.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vx.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bm.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hn.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qk.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qx.chemitech.net.cn

[H10] 资源自动释放
来源：http://oc.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lo.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://km.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nf.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vz.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fn.szxytkj.cn

Go:   defer f.Close()
来源：http://qo.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fo.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ov.gzmigu.cn

================================================================================
来源：http://pv.shxzskj.cn

I. 正则表达式
来源：http://cq.shtwfgs.cn

================================================================================
来源：http://py.9csxet.cn

[I01] 判断是否匹配
来源：http://pn.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ep.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yy.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://az.9csxet.cn

TS:   /\d+/.test(s)
来源：http://sd.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wg.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ix.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://wj.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vq.521024.cn

[I02] 提取所有匹配
来源：http://yt.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://mz.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tr.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://in.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://zf.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hd.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jb.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://ob.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vd.asd995.cn

[I03] 提取捕获分组
来源：http://pv.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sg.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ed.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fi.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ig.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ru.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xv.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oi.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sq.jctech888.com.cn

[I04] 正则替换
来源：http://na.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zc.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bi.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mo.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rc.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://az.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gq.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ve.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ho.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://ik.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://of.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dv.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://nt.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://oe.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ci.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://av.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ro.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sj.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vu.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pe.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://be.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ry.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pr.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ud.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ge.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tl.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://te.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://wp.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cz.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://su.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dp.panjiajie.cn

TS:   /error/gim
来源：http://eh.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xa.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cn.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://nd.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mb.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://wm.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ci.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hs.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xj.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ty.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rv.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ci.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bc.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wj.szsharing.cn

================================================================================
来源：http://kx.jianghongdianzi.cn

J. 日期与时间
来源：http://iz.asd995.cn

================================================================================
来源：http://rn.wgjwhj.cn

[J01] 获取当前时间
来源：http://ua.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oc.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pz.huanxung.cn

JS:   new Date();  Date.now()
来源：http://lq.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://ak.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mv.shxzskj.cn

Go:   time.Now()
来源：http://pz.yuexingan06.cn

Ruby: Time.now
来源：http://hn.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ph.huixiangedu.cn

[J02] 格式化输出
来源：http://uf.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://my.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ru.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ia.bjjhwx.cn

TS:   d.toISOString()
来源：http://ge.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sj.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rg.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wj.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cf.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://hu.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tx.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mq.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://na.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://em.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fg.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pt.hnjuh.cn

Ruby: Date.parse("2024-01-02")
来源：http://df.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yt.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://cn.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dq.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oe.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nu.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ua.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://as.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xh.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sv.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qq.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://nb.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://io.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://er.huixinmuqiang.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fj.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eu.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://sm.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ky.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://lk.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://la.szsharing.cn

[J06] 计算两时间之差
来源：http://yq.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://hz.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://er.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fg.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ts.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yn.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://sj.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://gq.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://fi.asd995.cn

[J07] 比较两个日期
来源：http://fy.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://or.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xp.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wa.hahajie.cn


<!-- 参考信息 -->