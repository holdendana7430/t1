代发 wailian999

Java: class Admin extends User {}
来源：http://zk.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bp.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://lq.colortex.cn

C#:   class Admin : User {}
来源：http://wz.wgjwhj.cn

[G06] 重写方法
来源：http://ph.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://hd.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bc.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://zr.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://rc.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://yq.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vj.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://do.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://wn.muxihuayi.cn

[G07] 调用父类方法
来源：http://ll.jctech888.com.cn

Py:   super().greet()
来源：http://tn.bjjhwx.cn

PHP:  parent::greet();
来源：http://mr.haigaiapp.cn

JS:   super.greet();
来源：http://cn.huanxung.cn

TS:   super.greet();
来源：http://yu.shtwfgs.cn

Java: super.greet();
来源：http://ro.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tz.nszjky.cn

Ruby: super
来源：http://jz.yuexingan06.cn

C#:   base.Greet();
来源：http://fd.9csxet.cn

[G08] 静态方法与属性
来源：http://hi.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jh.9csxet.cn

PHP:  public static function f() {}
来源：http://yx.wgjwhj.cn

JS:   static f() {}
来源：http://eq.nszjky.cn

TS:   static f(): void {}
来源：http://tp.szsharing.cn

Java: static void f() {}
来源：http://bv.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gk.szxytkj.cn

Ruby: def self.f; end
来源：http://cc.colortex.cn

C#:   public static void F() {}
来源：http://hj.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://rr.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://os.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oq.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gt.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://cb.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://yp.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://ro.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jr.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://kv.colortex.cn

[G10] 访问控制
来源：http://ca.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://ar.muxihuayi.cn

PHP:  public / protected / private
来源：http://wm.colortex.cn

JS:   #private 字段；其余公开
来源：http://ba.haigaiapp.cn

TS:   public / protected / private
来源：http://bx.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://jn.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ze.asd995.cn

Ruby: public / protected / private
来源：http://wy.9csxet.cn

C#:   public / protected / private / internal
来源：http://lx.asd995.cn

[G11] getter / setter
来源：http://rk.asd995.cn

Py:   @property 与 @x.setter
来源：http://ch.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jh.nicolike.cn

JS:   get name() { return this._name; }
来源：http://ry.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://pb.panjiajie.cn

Java: public String getName() { return name; }
来源：http://oe.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sx.hahajie.cn

Ruby: attr_accessor :name
来源：http://de.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://cz.shxzukj.cn

[G12] 对象转字符串
来源：http://jt.asd995.cn

Py:   def __str__(self): return self.name
来源：http://gv.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wp.asd995.cn

JS:   toString() { return this.name; }
来源：http://zt.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://ru.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://ii.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uz.newstarts.cn

Ruby: def to_s; @name; end
来源：http://kr.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://gi.panjiajie.cn

[G13] 判断对象类型
来源：http://ue.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://kh.hnjuh.cn

PHP:  $u instanceof User
来源：http://xm.hnjuh.cn

JS:   u instanceof User
来源：http://zy.bookmarksfly.cn

TS:   u instanceof User
来源：http://jy.lnxyls.cn

Java: u instanceof User
来源：http://kk.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ik.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://cn.asd995.cn

C#:   u is User
来源：http://ex.bjjhwx.cn

[G14] 数据类 / record
来源：http://gg.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cz.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://id.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lx.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://vz.9csxet.cn

Java: record User(String name, int age) {}
来源：http://ti.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://kh.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hh.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://az.shxzskj.cn

[G15] 枚举
来源：http://fd.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://en.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mm.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yz.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://se.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://by.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cl.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://wk.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sj.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://tp.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bf.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://il.szsharing.cn

JS:   Object.entries(obj)
来源：http://ga.lnxyls.cn

TS:   Object.entries(obj)
来源：http://xx.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://no.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fl.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://co.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://mn.szxytkj.cn

================================================================================
来源：http://rt.panjiajie.cn

H. 异常与错误处理
来源：http://na.nicolike.cn

================================================================================
来源：http://cg.yuexingan06.cn

[H01] try / catch 基础
来源：http://do.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ip.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qz.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hp.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tl.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bw.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yo.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://st.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nf.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://gt.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jz.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cu.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yp.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oz.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uq.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cg.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ze.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://tv.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://dg.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ti.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://zu.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://po.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lq.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kj.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://er.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gm.521024.cn

[H04] 自定义异常类型
来源：http://hu.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://ct.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fl.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://al.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://es.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://fy.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://az.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://ax.9csxet.cn

C#:   class MyException : Exception {}
来源：http://gu.shxzskj.cn

[H05] 捕获特定类型
来源：http://su.lnxyls.cn

Py:   except ValueError as e:
来源：http://jf.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ai.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://kr.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://df.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://nh.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://la.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://mz.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sg.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://ka.9csxet.cn

Py:   value = d.get("k") or default
来源：http://vm.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dd.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nn.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zq.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gz.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://na.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ih.521024.cn

C#:   obj?.A?.B ?? default
来源：http://ul.shxzskj.cn

[H07] 断言
来源：http://af.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://uk.yuexingan06.cn

PHP:  assert($x > 0);
来源：http://mh.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://ta.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://dm.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://ve.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://it.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uh.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ri.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://tl.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://hy.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hq.newstarts.cn

JS:   e.message;  e.stack
来源：http://bl.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nx.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dn.asd995.cn

Go:   err.Error()
来源：http://tl.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://kn.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://im.asd995.cn

[H09] 带错误码的异常
来源：http://vk.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://up.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gk.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ig.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ta.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ta.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ii.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ys.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xh.huanxung.cn

[H10] 资源自动释放
来源：http://ws.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://li.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://av.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bg.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ol.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nz.chemitech.net.cn

Go:   defer f.Close()
来源：http://ai.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dl.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mq.hnjuh.cn

================================================================================
来源：http://fz.colortex.cn

I. 正则表达式
来源：http://wl.chemitech.net.cn

================================================================================
来源：http://cu.asd995.cn

[I01] 判断是否匹配
来源：http://ol.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ss.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xq.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://if.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://vw.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://md.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dq.521024.cn

Ruby: s.match?(/\d+/)
来源：http://tp.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wy.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://ka.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://je.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ae.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://do.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://bz.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jb.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kx.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://bv.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://or.haigaiapp.cn

[I03] 提取捕获分组
来源：http://hr.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hp.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ud.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gr.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oc.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pu.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kl.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xo.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://so.muxihuayi.cn

[I04] 正则替换
来源：http://la.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xx.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xy.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://au.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nc.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fq.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xj.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vr.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ur.szxytkj.cn

[I05] 按正则拆分
来源：http://ve.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yp.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uv.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://xb.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://da.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://jn.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ov.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sl.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jq.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yh.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zu.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oj.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yx.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xh.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ou.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bx.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lx.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vu.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://gv.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ld.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rq.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xo.colortex.cn

TS:   /error/gim
来源：http://hy.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rc.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ca.colortex.cn

Ruby: s.scan(/error/i)
来源：http://mg.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ul.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://zm.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://td.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sp.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://po.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nh.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ht.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zf.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yr.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eb.asd995.cn

================================================================================
来源：http://lj.haigaiapp.cn

J. 日期与时间
来源：http://pn.shtwfgs.cn

================================================================================
来源：http://cm.chemitech.net.cn

[J01] 获取当前时间
来源：http://eg.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ps.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fq.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://uw.huanxung.cn

TS:   new Date();  Date.now()
来源：http://xq.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hq.haigaiapp.cn

Go:   time.Now()
来源：http://zp.huixiangedu.cn

Ruby: Time.now
来源：http://vd.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vk.muxihuayi.cn

[J02] 格式化输出
来源：http://nn.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cw.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nk.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wi.muxihuayi.cn

TS:   d.toISOString()
来源：http://qo.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sh.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ea.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gv.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://al.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://ir.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mo.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ah.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://tm.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://sx.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jh.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rs.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://hr.huixiangedu.cn


<!-- 参考信息 -->