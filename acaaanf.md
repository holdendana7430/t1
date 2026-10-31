代发 wailian999

Ruby: @name = "x"
来源：http://bg.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://ap.9csxet.cn

[G04] 定义方法
来源：http://db.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://wj.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kp.9csxet.cn

JS:   greet() { return this.name; }
来源：http://ao.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://no.chemitech.net.cn

Java: String greet() { return name; }
来源：http://rc.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gs.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://iy.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://wv.colortex.cn

[G05] 继承
来源：http://by.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://qa.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://ec.nszjky.cn

JS:   class Admin extends User {}
来源：http://vr.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://gm.nicolike.cn

Java: class Admin extends User {}
来源：http://st.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ag.asd995.cn

Ruby: class Admin < User; end
来源：http://yz.jctech888.com.cn

C#:   class Admin : User {}
来源：http://pa.bookmarksfly.cn

[G06] 重写方法
来源：http://mq.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://gl.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bz.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://bn.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://fl.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://nr.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jq.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://vk.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://wx.shxzukj.cn

[G07] 调用父类方法
来源：http://kp.asd995.cn

Py:   super().greet()
来源：http://be.shtwfgs.cn

PHP:  parent::greet();
来源：http://hj.lnxyls.cn

JS:   super.greet();
来源：http://ce.shxzskj.cn

TS:   super.greet();
来源：http://gb.shxzskj.cn

Java: super.greet();
来源：http://ty.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uh.9csxet.cn

Ruby: super
来源：http://ek.muxihuayi.cn

C#:   base.Greet();
来源：http://hn.lnxyls.cn

[G08] 静态方法与属性
来源：http://gd.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vu.hahajie.cn

PHP:  public static function f() {}
来源：http://et.huixinmuqiang.cn

JS:   static f() {}
来源：http://yk.nszjky.cn

TS:   static f(): void {}
来源：http://ue.shxzskj.cn

Java: static void f() {}
来源：http://ph.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ro.lnxyls.cn

Ruby: def self.f; end
来源：http://ge.nicolike.cn

C#:   public static void F() {}
来源：http://io.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://xq.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://js.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://by.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jd.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://vf.szsharing.cn

Java: interface Shape { double area(); }
来源：http://al.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://dl.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dn.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://fm.shxzskj.cn

[G10] 访问控制
来源：http://kq.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://vo.newstarts.cn

PHP:  public / protected / private
来源：http://af.nicolike.cn

JS:   #private 字段；其余公开
来源：http://vm.szxytkj.cn

TS:   public / protected / private
来源：http://jo.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://pq.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ev.shtwfgs.cn

Ruby: public / protected / private
来源：http://oi.shxzukj.cn

C#:   public / protected / private / internal
来源：http://ls.huixiangedu.cn

[G11] getter / setter
来源：http://fu.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://fl.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jj.nszjky.cn

JS:   get name() { return this._name; }
来源：http://xk.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://yb.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://ru.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ci.szsharing.cn

Ruby: attr_accessor :name
来源：http://vl.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://cz.muxihuayi.cn

[G12] 对象转字符串
来源：http://qw.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://lh.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ca.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://tz.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://gd.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://bv.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vz.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://dx.colortex.cn

C#:   public override string ToString() => Name;
来源：http://pb.9csxet.cn

[G13] 判断对象类型
来源：http://ec.521024.cn

Py:   isinstance(u, User)
来源：http://it.jctech888.com.cn

PHP:  $u instanceof User
来源：http://bq.shxzskj.cn

JS:   u instanceof User
来源：http://ma.panjiajie.cn

TS:   u instanceof User
来源：http://za.gzmigu.cn

Java: u instanceof User
来源：http://gs.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jl.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://mw.yuntaijiaju.cn

C#:   u is User
来源：http://je.9csxet.cn

[G14] 数据类 / record
来源：http://ip.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ll.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://fv.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fp.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://jg.9csxet.cn

Java: record User(String name, int age) {}
来源：http://xh.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://hr.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fd.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://iv.huanxung.cn

[G15] 枚举
来源：http://ls.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tv.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ba.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nl.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uj.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://qq.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jt.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://ac.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gq.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://gy.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yk.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://yl.hnjuh.cn

JS:   Object.entries(obj)
来源：http://yl.521024.cn

TS:   Object.entries(obj)
来源：http://gw.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nn.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lf.shxzskj.cn

Ruby: obj.instance_variables
来源：http://ln.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://an.newstarts.cn

================================================================================
来源：http://jn.wgjwhj.cn

H. 异常与错误处理
来源：http://np.shxzukj.cn

================================================================================
来源：http://hz.521024.cn

[H01] try / catch 基础
来源：http://lc.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vc.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jc.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rf.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ov.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fg.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wp.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ix.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ms.newstarts.cn

[H02] finally / ensure 收尾
来源：http://mz.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wa.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pq.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lr.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rs.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vr.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lq.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kw.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sh.haigaiapp.cn

[H03] 主动抛出异常
来源：http://ej.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://xu.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qe.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://cm.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://xf.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tp.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pu.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vp.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oq.521024.cn

[H04] 自定义异常类型
来源：http://xe.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://zj.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fo.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://zo.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://dt.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://rc.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ln.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://fj.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://pe.haigaiapp.cn

[H05] 捕获特定类型
来源：http://qn.newstarts.cn

Py:   except ValueError as e:
来源：http://gf.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rr.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://lx.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://jb.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://kk.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oi.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://uu.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gh.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://lr.asd995.cn

Py:   value = d.get("k") or default
来源：http://ka.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ex.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://np.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vl.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://od.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cq.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://dl.521024.cn

C#:   obj?.A?.B ?? default
来源：http://ym.wgjwhj.cn

[H07] 断言
来源：http://rj.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://ck.panjiajie.cn

PHP:  assert($x > 0);
来源：http://jp.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://bv.huanxung.cn

TS:   console.assert(x > 0);
来源：http://uq.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://po.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hf.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pj.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://pt.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://ob.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://qf.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mf.hnjuh.cn

JS:   e.message;  e.stack
来源：http://cz.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yt.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://na.colortex.cn

Go:   err.Error()
来源：http://pw.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://zb.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://gk.bjjhwx.cn

[H09] 带错误码的异常
来源：http://oj.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gy.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hk.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bp.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://up.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vy.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bs.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://os.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lm.haigaiapp.cn

[H10] 资源自动释放
来源：http://dy.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ox.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ge.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jj.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://et.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hh.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://mu.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jr.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ws.haigaiapp.cn

================================================================================
来源：http://rk.gzmigu.cn

I. 正则表达式
来源：http://cl.huanxung.cn

================================================================================
来源：http://js.nszjky.cn

[I01] 判断是否匹配
来源：http://dv.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bm.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wt.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://ya.521024.cn

TS:   /\d+/.test(s)
来源：http://ol.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nj.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vd.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://ki.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ey.hahajie.cn

[I02] 提取所有匹配
来源：http://ki.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://qy.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zo.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dy.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://il.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ul.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://as.nicolike.cn

Ruby: s.scan(/\d+/)
来源：http://if.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kk.nicolike.cn

[I03] 提取捕获分组
来源：http://dm.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lg.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rc.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zm.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kp.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qm.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yg.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fx.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ak.colortex.cn

[I04] 正则替换
来源：http://iy.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ud.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jl.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xo.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fn.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vf.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mv.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wj.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fe.nszjky.cn

[I05] 按正则拆分
来源：http://vb.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vk.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pr.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://pt.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ir.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://jx.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fh.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ug.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ze.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lw.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qv.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ou.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tz.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yj.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wi.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jy.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nu.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zn.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://cc.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gz.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fr.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nu.shxzskj.cn

TS:   /error/gim
来源：http://kx.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nw.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hw.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://dt.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cs.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://xu.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uf.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uh.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sl.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tk.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ek.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xb.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ap.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nl.asd995.cn

================================================================================
来源：http://ci.nszjky.cn

J. 日期与时间
来源：http://og.bjjhwx.cn

================================================================================
来源：http://ss.shxzskj.cn

[J01] 获取当前时间
来源：http://ev.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ym.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oe.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://dt.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://zr.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://do.haigaiapp.cn

Go:   time.Now()
来源：http://sh.jctech888.com.cn

Ruby: Time.now
来源：http://qx.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ju.nszjky.cn

[J02] 格式化输出
来源：http://gv.haigaiapp.cn


<!-- 参考信息 -->