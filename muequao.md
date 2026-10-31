代发 wailian999

Ruby: @name = "x"
来源：http://hv.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://hi.yuntaijiaju.cn

[G04] 定义方法
来源：http://bc.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://qz.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://te.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://wt.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://fi.521024.cn

Java: String greet() { return name; }
来源：http://my.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://no.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://fv.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://as.wgjwhj.cn

[G05] 继承
来源：http://ew.shxzukj.cn

Py:   class Admin(User): pass
来源：http://xk.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://vq.shxzukj.cn

JS:   class Admin extends User {}
来源：http://ac.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://pi.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://nv.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lj.nicolike.cn

Ruby: class Admin < User; end
来源：http://qd.hnjuh.cn

C#:   class Admin : User {}
来源：http://fr.szsharing.cn

[G06] 重写方法
来源：http://ri.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://cz.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mw.asd995.cn

JS:   greet() { return "admin"; }
来源：http://iw.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://vq.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://vd.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hv.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://rh.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://sj.panjiajie.cn

[G07] 调用父类方法
来源：http://qx.lnxyls.cn

Py:   super().greet()
来源：http://hb.lnxyls.cn

PHP:  parent::greet();
来源：http://ym.huanxung.cn

JS:   super.greet();
来源：http://li.wgjwhj.cn

TS:   super.greet();
来源：http://qc.bjjhwx.cn

Java: super.greet();
来源：http://rd.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ou.hnjuh.cn

Ruby: super
来源：http://dt.hnjuh.cn

C#:   base.Greet();
来源：http://nv.lnxyls.cn

[G08] 静态方法与属性
来源：http://to.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kg.jctech888.com.cn

PHP:  public static function f() {}
来源：http://or.jctech888.com.cn

JS:   static f() {}
来源：http://vp.colortex.cn

TS:   static f(): void {}
来源：http://pv.shxzskj.cn

Java: static void f() {}
来源：http://iu.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mu.huixiangedu.cn

Ruby: def self.f; end
来源：http://ex.nicolike.cn

C#:   public static void F() {}
来源：http://ba.521024.cn

[G09] 接口 / 抽象类
来源：http://tl.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://ym.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cl.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bc.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://jf.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://gc.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://ie.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qe.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://un.newstarts.cn

[G10] 访问控制
来源：http://pv.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://lu.wgjwhj.cn

PHP:  public / protected / private
来源：http://kj.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://kd.9csxet.cn

TS:   public / protected / private
来源：http://zv.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://kv.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lj.muxihuayi.cn

Ruby: public / protected / private
来源：http://pc.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://ay.yuntaijiaju.cn

[G11] getter / setter
来源：http://xo.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://cr.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ba.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://oh.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://jt.nszjky.cn

Java: public String getName() { return name; }
来源：http://dr.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://aw.colortex.cn

Ruby: attr_accessor :name
来源：http://tb.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://yv.huixiangedu.cn

[G12] 对象转字符串
来源：http://md.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://tr.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rz.521024.cn

JS:   toString() { return this.name; }
来源：http://ul.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://sf.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://gb.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jq.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://uj.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://pt.nszjky.cn

[G13] 判断对象类型
来源：http://tr.9csxet.cn

Py:   isinstance(u, User)
来源：http://ii.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://au.szsharing.cn

JS:   u instanceof User
来源：http://yx.521024.cn

TS:   u instanceof User
来源：http://bh.9csxet.cn

Java: u instanceof User
来源：http://hi.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ro.9csxet.cn

Ruby: u.is_a?(User)
来源：http://if.jianghongdianzi.cn

C#:   u is User
来源：http://vk.bjjhwx.cn

[G14] 数据类 / record
来源：http://hk.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zw.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://sd.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zk.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://wl.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://mv.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://hp.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cj.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://dy.shxzskj.cn

[G15] 枚举
来源：http://pe.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bt.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sa.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hg.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hx.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://xm.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cp.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://nv.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xs.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://yg.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vp.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://xu.hnjuh.cn

JS:   Object.entries(obj)
来源：http://qt.newstarts.cn

TS:   Object.entries(obj)
来源：http://br.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wd.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rc.521024.cn

Ruby: obj.instance_variables
来源：http://li.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://ql.shxzukj.cn

================================================================================
来源：http://eh.shxzukj.cn

H. 异常与错误处理
来源：http://xx.muxihuayi.cn

================================================================================
来源：http://cw.nicolike.cn

[H01] try / catch 基础
来源：http://qe.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gv.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qa.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ed.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zd.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uh.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pi.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qi.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://me.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://kf.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ll.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bo.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pv.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vf.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://if.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oo.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ut.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lm.521024.cn

[H03] 主动抛出异常
来源：http://kb.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://bm.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ua.521024.cn

JS:   throw new Error("错误信息");
来源：http://zq.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://sv.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vu.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ir.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://do.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tj.gzmigu.cn

[H04] 自定义异常类型
来源：http://zv.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://na.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sd.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://hm.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://jf.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://sz.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qv.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://ha.9csxet.cn

C#:   class MyException : Exception {}
来源：http://xa.shxzukj.cn

[H05] 捕获特定类型
来源：http://bi.huixiangedu.cn

Py:   except ValueError as e:
来源：http://xn.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cj.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://iq.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://ym.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://nh.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cc.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://bl.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pn.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://dm.9csxet.cn

Py:   value = d.get("k") or default
来源：http://rz.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mn.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ct.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ch.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yr.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zk.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://rk.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://ny.shxzukj.cn

[H07] 断言
来源：http://yk.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://ix.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://kd.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://bw.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://jw.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://fj.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xb.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xq.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://zw.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://ds.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://bg.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gq.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://km.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://if.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cb.nicolike.cn

Go:   err.Error()
来源：http://qx.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://hk.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://nl.szxytkj.cn

[H09] 带错误码的异常
来源：http://fn.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mz.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://go.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zo.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dp.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://td.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uf.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qe.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://up.shxzskj.cn

[H10] 资源自动释放
来源：http://xt.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ik.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xv.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yy.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tv.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gn.gzmigu.cn

Go:   defer f.Close()
来源：http://sg.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kd.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cb.yuntaijiaju.cn

================================================================================
来源：http://gk.asd995.cn

I. 正则表达式
来源：http://yr.521024.cn

================================================================================
来源：http://wi.huixiangedu.cn

[I01] 判断是否匹配
来源：http://fl.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bi.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kn.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://ec.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://nv.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eb.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://li.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://zh.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kt.lnxyls.cn

[I02] 提取所有匹配
来源：http://ma.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://wq.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mz.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qg.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://xz.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dk.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ft.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://ei.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xe.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://ur.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ne.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sj.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ao.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wq.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ps.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pk.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ln.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xv.jianghongdianzi.cn

[I04] 正则替换
来源：http://bd.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mq.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hp.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wq.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rl.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rr.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oa.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qn.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://he.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://sv.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gh.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vx.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://sj.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://my.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://ia.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nt.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qq.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qo.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nz.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vd.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kl.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lx.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tu.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dy.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kj.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jx.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lj.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://zc.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qh.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ll.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uc.shtwfgs.cn

TS:   /error/gim
来源：http://ps.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fu.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wy.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://zd.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yd.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://kf.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yv.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kl.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cs.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cd.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jn.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bj.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aw.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vm.bookmarksfly.cn

================================================================================
来源：http://nh.asd995.cn

J. 日期与时间
来源：http://jz.chemitech.net.cn

================================================================================
来源：http://ce.shxzukj.cn

[J01] 获取当前时间
来源：http://gh.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jv.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cz.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://kf.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://yv.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jb.asd995.cn

Go:   time.Now()
来源：http://dp.yuntaijiaju.cn

Ruby: Time.now
来源：http://tq.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sc.haigaiapp.cn

[J02] 格式化输出
来源：http://dy.wgjwhj.cn


<!-- 参考信息 -->