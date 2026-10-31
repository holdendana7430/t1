代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://lq.nszjky.cn

JS:   greet() { return this.name; }
来源：http://yu.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://mj.newstarts.cn

Java: String greet() { return name; }
来源：http://do.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fb.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://te.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://sc.9csxet.cn

[G05] 继承
来源：http://sa.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://dq.nicolike.cn

PHP:  class Admin extends User {}
来源：http://pn.newstarts.cn

JS:   class Admin extends User {}
来源：http://yo.521024.cn

TS:   class Admin extends User {}
来源：http://qz.asd995.cn

Java: class Admin extends User {}
来源：http://hl.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dm.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://sf.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://vd.yuntaijiaju.cn

[G06] 重写方法
来源：http://mw.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://tc.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ui.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://hq.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://pm.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://rp.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nd.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://gw.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://ne.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://mu.gzmigu.cn

Py:   super().greet()
来源：http://kh.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://jb.hnjuh.cn

JS:   super.greet();
来源：http://cj.colortex.cn

TS:   super.greet();
来源：http://xw.muxihuayi.cn

Java: super.greet();
来源：http://rh.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zc.chemitech.net.cn

Ruby: super
来源：http://qw.huixinmuqiang.cn

C#:   base.Greet();
来源：http://nc.hahajie.cn

[G08] 静态方法与属性
来源：http://lm.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://da.muxihuayi.cn

PHP:  public static function f() {}
来源：http://ad.9csxet.cn

JS:   static f() {}
来源：http://id.nszjky.cn

TS:   static f(): void {}
来源：http://dz.panjiajie.cn

Java: static void f() {}
来源：http://ka.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://be.colortex.cn

Ruby: def self.f; end
来源：http://ev.yuexingan06.cn

C#:   public static void F() {}
来源：http://lo.nicolike.cn

[G09] 接口 / 抽象类
来源：http://mw.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://dc.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bu.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gs.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://xa.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://lr.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://oe.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://el.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://go.wgjwhj.cn

[G10] 访问控制
来源：http://xi.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://qh.bjjhwx.cn

PHP:  public / protected / private
来源：http://sn.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://yq.yuntaijiaju.cn

TS:   public / protected / private
来源：http://ju.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://ny.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dv.jctech888.com.cn

Ruby: public / protected / private
来源：http://et.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://zw.huanxung.cn

[G11] getter / setter
来源：http://vt.huanxung.cn

Py:   @property 与 @x.setter
来源：http://xi.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dn.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://wh.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://ji.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://pp.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zj.colortex.cn

Ruby: attr_accessor :name
来源：http://dw.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://bp.colortex.cn

[G12] 对象转字符串
来源：http://hd.colortex.cn

Py:   def __str__(self): return self.name
来源：http://ro.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bo.newstarts.cn

JS:   toString() { return this.name; }
来源：http://kj.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://xp.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://yp.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wf.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://sa.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://rc.colortex.cn

[G13] 判断对象类型
来源：http://xw.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://tn.jctech888.com.cn

PHP:  $u instanceof User
来源：http://qf.wgjwhj.cn

JS:   u instanceof User
来源：http://uk.panjiajie.cn

TS:   u instanceof User
来源：http://ui.bookmarksfly.cn

Java: u instanceof User
来源：http://ll.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aq.nszjky.cn

Ruby: u.is_a?(User)
来源：http://ll.lnxyls.cn

C#:   u is User
来源：http://eh.jctech888.com.cn

[G14] 数据类 / record
来源：http://it.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pv.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://fo.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zg.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://tg.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://vz.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://io.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kt.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://by.hnjuh.cn

[G15] 枚举
来源：http://xz.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ts.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qf.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mh.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yi.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://vp.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://si.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://ea.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dt.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://ni.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wi.colortex.cn

PHP:  get_object_vars($obj);
来源：http://is.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://ic.newstarts.cn

TS:   Object.entries(obj)
来源：http://bl.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xc.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zs.hnjuh.cn

Ruby: obj.instance_variables
来源：http://sx.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://xy.hnjuh.cn

================================================================================
来源：http://il.yuntaijiaju.cn

H. 异常与错误处理
来源：http://dw.huixiangedu.cn

================================================================================
来源：http://cs.chemitech.net.cn

[H01] try / catch 基础
来源：http://hx.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bi.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nb.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hc.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ax.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dn.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tl.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zt.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mm.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://ki.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ua.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cx.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sn.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lw.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ys.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mf.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ni.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ln.nicolike.cn

[H03] 主动抛出异常
来源：http://vj.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://ua.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ia.colortex.cn

JS:   throw new Error("错误信息");
来源：http://ht.colortex.cn

TS:   throw new Error("错误信息");
来源：http://zy.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fe.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nq.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://to.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zu.haigaiapp.cn

[H04] 自定义异常类型
来源：http://zk.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://sq.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wd.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://jt.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://cx.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ej.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jh.521024.cn

Ruby: class MyError < StandardError; end
来源：http://em.nszjky.cn

C#:   class MyException : Exception {}
来源：http://rc.521024.cn

[H05] 捕获特定类型
来源：http://ta.shxzskj.cn

Py:   except ValueError as e:
来源：http://xv.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rf.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://it.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://xj.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://wx.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ok.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://ou.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ac.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://gs.newstarts.cn

Py:   value = d.get("k") or default
来源：http://js.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gq.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ou.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://il.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lz.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yh.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://wy.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://dw.chemitech.net.cn

[H07] 断言
来源：http://ta.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://tx.nicolike.cn

PHP:  assert($x > 0);
来源：http://rw.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://jz.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://fu.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://bd.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jr.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xu.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://fu.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://el.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://el.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://td.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://nu.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xj.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cl.muxihuayi.cn

Go:   err.Error()
来源：http://ij.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://bn.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://ki.yuexingan06.cn

[H09] 带错误码的异常
来源：http://lb.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tj.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fu.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ox.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ll.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lk.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bt.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ea.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bu.shxzukj.cn

[H10] 资源自动释放
来源：http://pa.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ue.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iv.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ud.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fd.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xa.hahajie.cn

Go:   defer f.Close()
来源：http://ur.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ii.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tb.nicolike.cn

================================================================================
来源：http://js.lnxyls.cn

I. 正则表达式
来源：http://dq.muxihuayi.cn

================================================================================
来源：http://re.chemitech.net.cn

[I01] 判断是否匹配
来源：http://qc.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ku.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kq.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://sd.hahajie.cn

TS:   /\d+/.test(s)
来源：http://al.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uc.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yx.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://en.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rm.szsharing.cn

[I02] 提取所有匹配
来源：http://tj.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://or.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lo.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kf.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://sw.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wn.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://am.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://cg.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pd.panjiajie.cn

[I03] 提取捕获分组
来源：http://xw.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pf.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mn.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rh.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hr.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pa.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lm.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ev.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ij.shtwfgs.cn

[I04] 正则替换
来源：http://so.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nc.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bl.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nn.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gv.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iy.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ji.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lf.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fo.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://zk.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wj.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ls.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://kx.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://nw.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://rb.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iw.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yq.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://my.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://we.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wn.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mg.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sv.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://br.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bw.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://po.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://el.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gn.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://jl.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pc.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jp.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://am.521024.cn

TS:   /error/gim
来源：http://vl.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bs.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xo.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://om.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ka.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://zs.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ld.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lt.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vs.colortex.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cw.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fo.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ai.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tx.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ol.chemitech.net.cn

================================================================================
来源：http://yt.shxzukj.cn

J. 日期与时间
来源：http://ri.shxzskj.cn

================================================================================
来源：http://hc.jctech888.com.cn

[J01] 获取当前时间
来源：http://xo.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rv.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uk.colortex.cn

JS:   new Date();  Date.now()
来源：http://un.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://qq.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://og.panjiajie.cn

Go:   time.Now()
来源：http://rp.9csxet.cn

Ruby: Time.now
来源：http://vr.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wz.jianghongdianzi.cn

[J02] 格式化输出
来源：http://av.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lt.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oq.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://en.lnxyls.cn

TS:   d.toISOString()
来源：http://lr.shtwfgs.cn


<!-- 参考信息 -->