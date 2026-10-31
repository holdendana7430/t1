代发 wailian999

[G06] 重写方法
来源：http://dz.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://jc.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nw.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://cf.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://bw.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://po.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sp.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://xl.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://ya.szsharing.cn

[G07] 调用父类方法
来源：http://wy.shxzskj.cn

Py:   super().greet()
来源：http://tv.lnxyls.cn

PHP:  parent::greet();
来源：http://cw.521024.cn

JS:   super.greet();
来源：http://xf.bjjhwx.cn

TS:   super.greet();
来源：http://rm.bookmarksfly.cn

Java: super.greet();
来源：http://go.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oh.szsharing.cn

Ruby: super
来源：http://ny.shxzukj.cn

C#:   base.Greet();
来源：http://sq.newstarts.cn

[G08] 静态方法与属性
来源：http://wy.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cm.521024.cn

PHP:  public static function f() {}
来源：http://ax.szxytkj.cn

JS:   static f() {}
来源：http://gi.nicolike.cn

TS:   static f(): void {}
来源：http://of.newstarts.cn

Java: static void f() {}
来源：http://us.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ln.9csxet.cn

Ruby: def self.f; end
来源：http://pd.shxzukj.cn

C#:   public static void F() {}
来源：http://to.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://uv.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://yw.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://af.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ut.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://mj.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://hb.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://ui.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qq.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://ld.shxzskj.cn

[G10] 访问控制
来源：http://rw.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ew.hnjuh.cn

PHP:  public / protected / private
来源：http://ok.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://lw.huixinmuqiang.cn

TS:   public / protected / private
来源：http://zc.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://lk.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jh.nszjky.cn

Ruby: public / protected / private
来源：http://kk.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://vf.panjiajie.cn

[G11] getter / setter
来源：http://lp.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://bo.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zv.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://rh.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://zl.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://en.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ij.521024.cn

Ruby: attr_accessor :name
来源：http://br.521024.cn

C#:   public string Name { get; set; }
来源：http://eo.szsharing.cn

[G12] 对象转字符串
来源：http://wp.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://nl.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://it.szsharing.cn

JS:   toString() { return this.name; }
来源：http://ry.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://te.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://sn.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ha.colortex.cn

Ruby: def to_s; @name; end
来源：http://ad.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ll.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://ws.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://mx.newstarts.cn

PHP:  $u instanceof User
来源：http://vz.muxihuayi.cn

JS:   u instanceof User
来源：http://rc.hnjuh.cn

TS:   u instanceof User
来源：http://wk.szsharing.cn

Java: u instanceof User
来源：http://xh.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://no.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://tc.nszjky.cn

C#:   u is User
来源：http://yz.chemitech.net.cn

[G14] 数据类 / record
来源：http://oz.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://od.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://eb.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qk.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://iu.szsharing.cn

Java: record User(String name, int age) {}
来源：http://zo.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://zq.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ki.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://kd.huixinmuqiang.cn

[G15] 枚举
来源：http://cz.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wr.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pq.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ob.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lu.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://dd.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://em.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://oy.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xd.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://fk.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rz.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://qu.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://uu.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://hy.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wi.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ux.shxzukj.cn

Ruby: obj.instance_variables
来源：http://fl.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://kk.colortex.cn

================================================================================
来源：http://bm.bookmarksfly.cn

H. 异常与错误处理
来源：http://vf.nszjky.cn

================================================================================
来源：http://jc.yuexingan06.cn

[H01] try / catch 基础
来源：http://ks.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://un.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fu.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sn.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iq.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sl.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://el.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fq.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jk.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ke.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ep.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tt.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cb.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yp.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wk.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xs.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qs.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xp.huixiangedu.cn

[H03] 主动抛出异常
来源：http://mz.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://zc.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xv.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://gj.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://qd.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rm.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fz.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pd.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://og.nszjky.cn

[H04] 自定义异常类型
来源：http://rh.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://dv.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qy.9csxet.cn

JS:   class MyError extends Error {}
来源：http://jf.asd995.cn

TS:   class MyError extends Error {}
来源：http://uu.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://qm.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ij.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://gn.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://yi.nicolike.cn

[H05] 捕获特定类型
来源：http://gp.hahajie.cn

Py:   except ValueError as e:
来源：http://kf.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lc.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://vm.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://rz.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://iy.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tm.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://jp.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zn.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://nw.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://jy.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ej.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ja.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fj.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ex.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://it.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://st.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://yn.hahajie.cn

[H07] 断言
来源：http://ie.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://xv.shxzskj.cn

PHP:  assert($x > 0);
来源：http://zu.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://jn.newstarts.cn

TS:   console.assert(x > 0);
来源：http://bp.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://kv.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sr.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ju.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://yq.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://zc.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://gb.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qg.szsharing.cn

JS:   e.message;  e.stack
来源：http://ei.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jl.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bo.nicolike.cn

Go:   err.Error()
来源：http://uv.521024.cn

Ruby: e.message;  e.backtrace
来源：http://bb.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://ee.shxzskj.cn

[H09] 带错误码的异常
来源：http://ai.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lf.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yt.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uf.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bh.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rp.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ey.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://td.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fb.chemitech.net.cn

[H10] 资源自动释放
来源：http://zi.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mb.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ug.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://om.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gj.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://br.haigaiapp.cn

Go:   defer f.Close()
来源：http://lv.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lu.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qe.huanxung.cn

================================================================================
来源：http://ah.hnjuh.cn

I. 正则表达式
来源：http://iq.szsharing.cn

================================================================================
来源：http://ma.jctech888.com.cn

[I01] 判断是否匹配
来源：http://ge.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vp.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pw.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://jj.newstarts.cn

TS:   /\d+/.test(s)
来源：http://jt.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ak.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ay.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://xn.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qo.nicolike.cn

[I02] 提取所有匹配
来源：http://wf.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://xo.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fh.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ig.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://xv.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mp.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eu.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://cg.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ob.chemitech.net.cn

[I03] 提取捕获分组
来源：http://tw.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lf.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cj.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hy.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wf.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://az.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hn.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wu.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lc.hahajie.cn

[I04] 正则替换
来源：http://vr.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sk.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pa.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qr.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ue.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ib.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ei.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rl.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kn.colortex.cn

[I05] 按正则拆分
来源：http://hz.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xy.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ql.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://kd.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://ld.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://zn.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jx.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://or.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sy.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iy.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ti.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qe.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bd.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jz.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pz.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://te.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pj.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zv.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://bk.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jv.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ts.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://me.haigaiapp.cn

TS:   /error/gim
来源：http://hi.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wa.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mm.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://nj.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://va.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://fm.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gu.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://en.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mx.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ji.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nr.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ln.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yh.jctech888.com.cn

================================================================================
来源：http://gt.bjjhwx.cn

J. 日期与时间
来源：http://sm.9csxet.cn

================================================================================
来源：http://wa.colortex.cn

[J01] 获取当前时间
来源：http://bp.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://by.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lg.9csxet.cn

JS:   new Date();  Date.now()
来源：http://zw.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://np.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pa.shtwfgs.cn

Go:   time.Now()
来源：http://kl.jctech888.com.cn

Ruby: Time.now
来源：http://dq.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cx.nicolike.cn

[J02] 格式化输出
来源：http://rv.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://es.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eo.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pb.hahajie.cn

TS:   d.toISOString()
来源：http://nn.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tf.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://np.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aa.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wj.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://lk.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xz.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iv.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://hv.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://yl.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ke.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://li.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://kt.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jy.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://ti.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zm.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kw.jctech888.com.cn


<!-- 参考信息 -->