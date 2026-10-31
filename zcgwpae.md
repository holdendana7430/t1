代发 wailian999

Java: class Admin extends User {}
来源：http://vq.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hj.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://co.asd995.cn

C#:   class Admin : User {}
来源：http://qn.bookmarksfly.cn

[G06] 重写方法
来源：http://ey.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://mz.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rh.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://sf.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://td.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://uf.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yg.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ez.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://kl.nszjky.cn

[G07] 调用父类方法
来源：http://ty.hnjuh.cn

Py:   super().greet()
来源：http://xg.newstarts.cn

PHP:  parent::greet();
来源：http://wm.9csxet.cn

JS:   super.greet();
来源：http://ik.huixiangedu.cn

TS:   super.greet();
来源：http://et.szsharing.cn

Java: super.greet();
来源：http://vj.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ju.jctech888.com.cn

Ruby: super
来源：http://pc.nszjky.cn

C#:   base.Greet();
来源：http://je.huanxung.cn

[G08] 静态方法与属性
来源：http://or.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fb.huanxung.cn

PHP:  public static function f() {}
来源：http://mt.gzmigu.cn

JS:   static f() {}
来源：http://ru.haigaiapp.cn

TS:   static f(): void {}
来源：http://wb.521024.cn

Java: static void f() {}
来源：http://fh.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qh.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://ou.hnjuh.cn

C#:   public static void F() {}
来源：http://fr.hahajie.cn

[G09] 接口 / 抽象类
来源：http://od.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://at.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mc.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cs.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://mv.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://la.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://re.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rn.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://cf.lnxyls.cn

[G10] 访问控制
来源：http://eg.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://wp.panjiajie.cn

PHP:  public / protected / private
来源：http://lu.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://ts.colortex.cn

TS:   public / protected / private
来源：http://ts.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://yq.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mw.yuexingan06.cn

Ruby: public / protected / private
来源：http://do.gzmigu.cn

C#:   public / protected / private / internal
来源：http://fs.shxzskj.cn

[G11] getter / setter
来源：http://kw.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://nn.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gu.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://cy.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://ze.gzmigu.cn

Java: public String getName() { return name; }
来源：http://fd.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kg.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://ht.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://no.shxzukj.cn

[G12] 对象转字符串
来源：http://my.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://vj.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ou.nicolike.cn

JS:   toString() { return this.name; }
来源：http://kx.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://ue.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://bg.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cr.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://xv.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://lt.newstarts.cn

[G13] 判断对象类型
来源：http://dk.szsharing.cn

Py:   isinstance(u, User)
来源：http://oj.colortex.cn

PHP:  $u instanceof User
来源：http://iv.shxzskj.cn

JS:   u instanceof User
来源：http://kl.szxytkj.cn

TS:   u instanceof User
来源：http://je.nicolike.cn

Java: u instanceof User
来源：http://vf.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pn.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://mm.wgjwhj.cn

C#:   u is User
来源：http://zn.asd995.cn

[G14] 数据类 / record
来源：http://uy.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ks.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://kd.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://as.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://xm.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://tj.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://oh.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qf.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://am.muxihuayi.cn

[G15] 枚举
来源：http://sk.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zh.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yi.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ch.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pa.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://kb.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nu.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://hd.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jc.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://bt.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rt.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://zq.szxytkj.cn

JS:   Object.entries(obj)
来源：http://ur.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://hm.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xd.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vk.hnjuh.cn

Ruby: obj.instance_variables
来源：http://fs.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://ft.nszjky.cn

================================================================================
来源：http://zh.huanxung.cn

H. 异常与错误处理
来源：http://nc.bjjhwx.cn

================================================================================
来源：http://fi.hnjuh.cn

[H01] try / catch 基础
来源：http://pu.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zk.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bs.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fq.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cs.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://on.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ba.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gm.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ta.huanxung.cn

[H02] finally / ensure 收尾
来源：http://ms.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ml.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yh.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fd.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cv.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wj.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jx.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hg.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rl.gzmigu.cn

[H03] 主动抛出异常
来源：http://tz.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://oq.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://as.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://vl.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://nd.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zm.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rm.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ko.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://in.szxytkj.cn

[H04] 自定义异常类型
来源：http://ew.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://zy.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mc.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://rc.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://ba.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://rs.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://om.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://fn.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://kg.newstarts.cn

[H05] 捕获特定类型
来源：http://xp.jctech888.com.cn

Py:   except ValueError as e:
来源：http://wq.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mq.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://ms.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://bx.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://ah.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ko.521024.cn

Ruby: rescue ArgumentError => e
来源：http://ml.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ac.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://ti.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://il.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yw.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://di.nszjky.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vi.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://da.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eg.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://cr.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://fl.jianghongdianzi.cn

[H07] 断言
来源：http://jm.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://pd.panjiajie.cn

PHP:  assert($x > 0);
来源：http://ip.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://sp.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://zj.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://ym.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hd.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://va.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://zl.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://hr.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://vg.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://op.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://yd.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ct.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://it.panjiajie.cn

Go:   err.Error()
来源：http://qs.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://vr.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://fn.muxihuayi.cn

[H09] 带错误码的异常
来源：http://ta.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bs.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jb.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jw.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://na.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kn.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bp.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://av.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dz.newstarts.cn

[H10] 资源自动释放
来源：http://oi.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qk.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ii.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kk.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wd.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sz.szsharing.cn

Go:   defer f.Close()
来源：http://ib.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cm.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tl.gzmigu.cn

================================================================================
来源：http://ur.szxytkj.cn

I. 正则表达式
来源：http://pa.szxytkj.cn

================================================================================
来源：http://uo.newstarts.cn

[I01] 判断是否匹配
来源：http://at.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xh.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qv.9csxet.cn

JS:   /\d+/.test(s)
来源：http://ha.huanxung.cn

TS:   /\d+/.test(s)
来源：http://fm.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kr.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rj.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://so.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ht.hahajie.cn

[I02] 提取所有匹配
来源：http://ev.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://cw.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hd.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://im.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://yc.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lz.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dv.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://ei.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://er.szxytkj.cn

[I03] 提取捕获分组
来源：http://qn.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ls.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://au.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hn.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yp.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xe.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jf.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dx.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hf.jianghongdianzi.cn

[I04] 正则替换
来源：http://kx.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mp.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ox.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qd.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kv.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sy.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://re.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gu.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dp.huanxung.cn

[I05] 按正则拆分
来源：http://sn.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dc.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://so.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://hj.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://gx.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://yc.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xg.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://on.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://un.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ln.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://so.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zx.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ul.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zi.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://re.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vj.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nt.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zw.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://wn.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sm.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rn.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jr.huixinmuqiang.cn

TS:   /error/gim
来源：http://af.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bg.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bx.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://jy.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bk.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://yw.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fc.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ga.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ot.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ck.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ni.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ik.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ec.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xz.szxytkj.cn

================================================================================
来源：http://kk.wgjwhj.cn

J. 日期与时间
来源：http://uc.yuntaijiaju.cn

================================================================================
来源：http://gl.panjiajie.cn

[J01] 获取当前时间
来源：http://ht.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vh.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lg.szsharing.cn

JS:   new Date();  Date.now()
来源：http://ep.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://np.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qw.lnxyls.cn

Go:   time.Now()
来源：http://ln.hnjuh.cn

Ruby: Time.now
来源：http://rp.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kg.hnjuh.cn

[J02] 格式化输出
来源：http://za.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lz.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vz.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fq.shtwfgs.cn

TS:   d.toISOString()
来源：http://ac.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fy.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gy.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xi.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gq.panjiajie.cn

[J03] 字符串解析为日期
来源：http://ju.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wl.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tr.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://nd.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://pa.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jk.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mt.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://ao.wgjwhj.cn


<!-- 参考信息 -->