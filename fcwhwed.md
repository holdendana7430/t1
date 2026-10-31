代发 wailian999

Py:   class Admin(User): pass
来源：http://if.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://pc.nicolike.cn

JS:   class Admin extends User {}
来源：http://xb.nszjky.cn

TS:   class Admin extends User {}
来源：http://zg.shtwfgs.cn

Java: class Admin extends User {}
来源：http://rg.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rn.panjiajie.cn

Ruby: class Admin < User; end
来源：http://ur.9csxet.cn

C#:   class Admin : User {}
来源：http://xb.521024.cn

[G06] 重写方法
来源：http://ax.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://bu.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cc.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://hu.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://fi.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://zn.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ci.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://wh.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://qk.huanxung.cn

[G07] 调用父类方法
来源：http://oa.yuexingan06.cn

Py:   super().greet()
来源：http://zv.jctech888.com.cn

PHP:  parent::greet();
来源：http://ze.bjjhwx.cn

JS:   super.greet();
来源：http://ft.wgjwhj.cn

TS:   super.greet();
来源：http://qb.jctech888.com.cn

Java: super.greet();
来源：http://iv.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zy.bookmarksfly.cn

Ruby: super
来源：http://fm.yuexingan06.cn

C#:   base.Greet();
来源：http://hj.huixiangedu.cn

[G08] 静态方法与属性
来源：http://dc.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mu.hnjuh.cn

PHP:  public static function f() {}
来源：http://xy.jctech888.com.cn

JS:   static f() {}
来源：http://mr.jctech888.com.cn

TS:   static f(): void {}
来源：http://od.yuntaijiaju.cn

Java: static void f() {}
来源：http://yz.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://co.huanxung.cn

Ruby: def self.f; end
来源：http://uc.yuexingan06.cn

C#:   public static void F() {}
来源：http://if.nicolike.cn

[G09] 接口 / 抽象类
来源：http://jh.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://eb.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yy.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ud.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://yk.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://fp.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://vo.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lt.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://iz.chemitech.net.cn

[G10] 访问控制
来源：http://eb.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://ub.huixiangedu.cn

PHP:  public / protected / private
来源：http://ec.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://cj.wgjwhj.cn

TS:   public / protected / private
来源：http://qw.asd995.cn

Java: public / protected / private / 默认包级
来源：http://ho.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hf.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://wg.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://xp.bjjhwx.cn

[G11] getter / setter
来源：http://ye.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://lt.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nz.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://rt.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://rc.nszjky.cn

Java: public String getName() { return name; }
来源：http://bh.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zt.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://nd.521024.cn

C#:   public string Name { get; set; }
来源：http://km.szxytkj.cn

[G12] 对象转字符串
来源：http://wt.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://gj.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xz.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://vm.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://vq.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ll.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vt.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://vg.colortex.cn

C#:   public override string ToString() => Name;
来源：http://gj.hahajie.cn

[G13] 判断对象类型
来源：http://xn.colortex.cn

Py:   isinstance(u, User)
来源：http://mv.asd995.cn

PHP:  $u instanceof User
来源：http://ee.asd995.cn

JS:   u instanceof User
来源：http://oh.shxzskj.cn

TS:   u instanceof User
来源：http://tr.shtwfgs.cn

Java: u instanceof User
来源：http://zf.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qf.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://vn.newstarts.cn

C#:   u is User
来源：http://nt.panjiajie.cn

[G14] 数据类 / record
来源：http://nx.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fr.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://lw.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://be.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://wh.huanxung.cn

Java: record User(String name, int age) {}
来源：http://yq.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://yl.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kn.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://fm.521024.cn

[G15] 枚举
来源：http://uq.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jt.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yz.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gt.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uz.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://jb.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nm.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://nm.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zm.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://sj.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pz.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://hw.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://vj.szxytkj.cn

TS:   Object.entries(obj)
来源：http://pd.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sa.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pj.szxytkj.cn

Ruby: obj.instance_variables
来源：http://az.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://cf.9csxet.cn

================================================================================
来源：http://jr.jctech888.com.cn

H. 异常与错误处理
来源：http://yx.521024.cn

================================================================================
来源：http://ph.chemitech.net.cn

[H01] try / catch 基础
来源：http://uk.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://he.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fo.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://py.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kk.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cz.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nf.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yu.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rv.newstarts.cn

[H02] finally / ensure 收尾
来源：http://ro.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yq.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://aw.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lz.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qz.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://in.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wc.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ut.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ai.hahajie.cn

[H03] 主动抛出异常
来源：http://hx.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://ja.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://go.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://bu.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://ca.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jy.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bo.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qw.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kp.colortex.cn

[H04] 自定义异常类型
来源：http://wq.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://lv.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tf.szsharing.cn

JS:   class MyError extends Error {}
来源：http://vi.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://vf.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://ps.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hj.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://td.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://qp.nicolike.cn

[H05] 捕获特定类型
来源：http://ar.shxzskj.cn

Py:   except ValueError as e:
来源：http://bq.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hh.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://ti.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://us.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://rp.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lx.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://qp.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mb.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://of.521024.cn

Py:   value = d.get("k") or default
来源：http://xe.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rh.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lf.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ib.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uf.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nf.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://fv.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://ov.jianghongdianzi.cn

[H07] 断言
来源：http://lh.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://ws.shxzskj.cn

PHP:  assert($x > 0);
来源：http://vc.nszjky.cn

JS:   console.assert(x > 0);
来源：http://lp.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://zr.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://cj.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dk.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ob.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://dp.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://uc.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://mq.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lg.nszjky.cn

JS:   e.message;  e.stack
来源：http://mi.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xk.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wv.yuexingan06.cn

Go:   err.Error()
来源：http://gl.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://fr.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://lj.shxzskj.cn

[H09] 带错误码的异常
来源：http://qw.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uz.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ic.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vd.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://po.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xl.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ia.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hq.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sy.panjiajie.cn

[H10] 资源自动释放
来源：http://ud.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bi.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fe.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xo.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rt.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ke.shxzskj.cn

Go:   defer f.Close()
来源：http://lv.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xb.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ak.9csxet.cn

================================================================================
来源：http://ev.521024.cn

I. 正则表达式
来源：http://mb.yuexingan06.cn

================================================================================
来源：http://qh.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://sx.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xf.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tl.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://nn.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://dt.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sk.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kf.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://fy.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ok.panjiajie.cn

[I02] 提取所有匹配
来源：http://hj.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://qg.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iq.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://br.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://xz.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bz.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pw.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://nl.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hq.wgjwhj.cn

[I03] 提取捕获分组
来源：http://fr.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ln.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eh.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://at.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qq.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tm.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lw.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fd.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rc.gzmigu.cn

[I04] 正则替换
来源：http://er.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gs.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sq.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cw.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://co.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gs.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vs.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hc.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mn.wgjwhj.cn

[I05] 按正则拆分
来源：http://dg.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://io.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://on.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://zc.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://sx.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://ue.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cw.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://et.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kc.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vs.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xm.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://im.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xe.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vl.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mi.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ss.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jf.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tt.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://cp.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kk.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sq.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ci.asd995.cn

TS:   /error/gim
来源：http://yc.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cs.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oc.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://dn.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qi.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://ko.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ty.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cx.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gr.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vl.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aq.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vx.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wc.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zt.shtwfgs.cn

================================================================================
来源：http://ql.yuexingan06.cn

J. 日期与时间
来源：http://um.nszjky.cn

================================================================================
来源：http://sx.shtwfgs.cn

[J01] 获取当前时间
来源：http://db.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://op.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pk.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://qo.newstarts.cn

TS:   new Date();  Date.now()
来源：http://qo.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zj.jctech888.com.cn

Go:   time.Now()
来源：http://xn.jctech888.com.cn

Ruby: Time.now
来源：http://cq.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hj.yuntaijiaju.cn

[J02] 格式化输出
来源：http://cy.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vi.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nu.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ar.521024.cn

TS:   d.toISOString()
来源：http://ei.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eg.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aa.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yn.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dy.521024.cn

[J03] 字符串解析为日期
来源：http://ec.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://je.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yi.asd995.cn

JS:   new Date("2024-01-02")
来源：http://yv.huanxung.cn


<!-- 参考信息 -->