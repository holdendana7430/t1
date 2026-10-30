代发 wailian999

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gdgnxwyfo.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gyfeszddu.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpuacmpes.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/guwnqzrso.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gklpisset.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gecekgelu.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gnetfytkb.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/glsrvkzvc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gsukuyvqz.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gewagirsc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gpgsepfaw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grrcmmkrd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqqfuyqvy.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gthzbfvhl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/guinwjndm.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gjqkprifs.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gbaxvgulz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gybtkrotc.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwadnijcb.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqymhgrio.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmoacrhax.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/grzahtoei.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/grwjwtede.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/grculiuly.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gyfstpmmz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gtxouatny.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gadvjlvsq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gkxmzpcax.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/getngndpq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/geakufyfa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gtgdlolzb.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/ghdburprn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gzqskbvjt.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gglhleuui.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/ggjnzfdsd.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gycdrhyub.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gqvlheavs.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdjvxexwd.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gaivyzhbl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/ghthzhknx.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gecsktjti.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsisrhdsb.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gosvwaspr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gfoowanyk.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gtdizndgq.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gwiqajsej.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gyfkqysiy.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gmcgkkdcu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gkjfgzcou.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/ghylwjxyc.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gnxkexzwe.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/grmcsyrhs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/grcskwlai.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gfsnehbtz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gwthwjwnq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gemtiqsxx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gjajzjyhz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gffezyrlr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gqpkkkumf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjzdqcdca.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gdqmvcuev.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gziflsbuf.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gytaxekex.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/ghfyiicnt.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gppkewozn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/ghgqezyou.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gpczpkhqt.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpmglpurp.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gywswpljt.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gjphspkcz.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gostygnjw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gydntczzs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ghtcdixjw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gogkpbjbe.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ghxoqcqaq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gxrqquvej.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gcvokqpgq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gnkbrvkde.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/guxeshokd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gyldhkcvs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/guacqwvko.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gppmqaflm.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gpkjnbgsp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfvvxthxq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtlvgcrbk.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gxvpbfhlm.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gczxpants.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/glecrxoig.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gjarxsayg.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmojtcpke.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghymwsfgr.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glhfnsent.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gmsswwwhh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gpkupnyjz.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gbbfxiejq.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gugsouelw.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gtqkdnows.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gwnvdajbc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gkejgmoyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/grrvmdusg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/geedqamxw.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gdcjaeodn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/glzronbrx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gsxpubsow.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gmvwsvmfu.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gyzayrgxl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gcjgaeabl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gbjetbtjg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gjmftzfdg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gmirqqovz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gdohfjitn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/genjywdvw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gyrlzmcsc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gvxuxddbd.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gtiecrhra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gamcjcfaj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/guxzbvfcx.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gntfyqche.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gpdccmeca.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gwcxzuvvs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gzclcxkfo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/glfljijdc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/glqcclpfb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gupuiwnlu.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gsusrvdjm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggtzyeieh.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gapjcnxod.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gahusagjo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gjtvwffjv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmfoxqzma.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gbiuabzgw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gutgrpnly.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/girqiopdn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gbihuffsb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/giqxyefvz.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpuvkpf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/ggjtiwvio.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gwaqscypm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gxanneayl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gtnvimotc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ghkekkoga.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gtcjyipeq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gbilqeomn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gxaanjyou.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gjjfxdhrf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gkjbisfef.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gliopwuni.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gagtrfipa.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gidpslllw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gksavzeqz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/giztjfnnq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gxkehikpe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gufmvvyvw.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gktgmprlb.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gftjjsnna.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/ghppkllti.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gfumzncow.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gurjxsujz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gqqosyyzi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmikxbcy.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gnhbnzxgj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gmstxggxm.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gggprppor.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gshlffvnr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/ggzjucfcb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdgpelllu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gvpkxjxhx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gzbyfpoxz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gjpfytubm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gytdgzcxw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gbgxtxrlv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/glvvrgysw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gvoajworo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/godiurpwh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gviubutnz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/godnxfktp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/giwrqpcgw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gvupgazsz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gtqxcunnn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gcculsgik.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gmymijyxc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gfnsfdowd.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/giowemlhy.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqksjicir.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/ghzjdivrd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/goytaismm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/glglbwfob.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gqzwvzqla.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/ggotqrfju.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/grmdjfmor.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gzgjhosog.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gkdaxambq.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gvihabjwu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gplezwnah.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gzxveclyg.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gzlqcufhp.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gvybgwdwj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gagqkwyys.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gkicfqari.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gcbnxdahq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gpeysgxed.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gktwbgigl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gdcdkyvor.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gxmcogmps.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/galqnfqvi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gbegiqjsn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gfkyvxuio.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gkonhrffq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gjfditodd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/ghmeospwn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/giktsynqr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gsybatdwr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gsvmqkbnj.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gvpquhrml.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/ggzsavjoo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxprvvcbu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkhbsyiwe.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gxgamffdg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxoxxcosu.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gusrpxuyd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gpcyjgwec.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gbphnqvby.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gdgksgydn.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gkcungnls.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gosaekpgt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gykuhpcof.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/getnxxghj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gpooufmcw.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/grjqcyggb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gellrbvyj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gkerofeqe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gxntnhtzf.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gixmtsmbw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gqagnsggo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gshuznsua.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gqumhtqlw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gleycvxaq.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/ginkijbor.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/glbnatcxm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/ghalaobfo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gwmtrkopn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/ggrndlrxr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gtaqagusa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gwbkmjzge.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gwbrysuvv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gpsblqreo.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gktczoxyg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gcowygrya.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/glklsyurt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gxuomyzok.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gvbzjxkyp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gqizilsyb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlyokxni.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gmaxjdahw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/glfkikidn.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gphynmwtz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gzxywkenx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gnwofihjg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gixalnibo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gqgtpvgyi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gpumhhrdb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gjeawsjoo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gcxhrscqy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gqoqriuic.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gsaadeyte.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gsruzguup.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gxxhgrpkg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gpfkndubc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gccemineq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/grnhaflev.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gmnskdpys.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/guxuijbdx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/ggdgvjaxa.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gsbhzhmmv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gfhfqfeoj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gvdnfuwyx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gkkwfcyus.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gvkychzym.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gbomakbmx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gypkudeya.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gezezihbf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gswxboaeg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gtmsdsjja.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gvjwwfunm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gurssghxa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gswcawkqy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gsbfxpzmi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/grbmdsxkl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gsbrvadff.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gwzmnuzmg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gjzaiwbhn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gszsfhctn.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gigjxsumj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvhzvkebv.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gdntubguf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gtxstxchb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gnjlrqtxv.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gsaxmdafy.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gzqwponop.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gdnjyrpfk.sHtML


<!-- 参考信息 -->