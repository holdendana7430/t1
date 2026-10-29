代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtcfedoxd.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/ghtnebbib.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gibbddlgd.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gnwzutmmc.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gabamkcle.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gsthndoku.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/ggevflbks.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gwkyzvequ.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gfpdmyytn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gasiguecq.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gisfmgndw.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gqjtfqckj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnvezhjtr.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gatkzygff.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gayflknyh.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gyotjdomd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gjxphvecq.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gvcvndgnf.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gyemfdemy.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gouxlinaa.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gaecoozql.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwnyaiizb.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqcnmdyku.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmxnfcpwk.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/grqelfsgj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/ghoitwyzu.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gfznhhgco.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/ggxhehdfb.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gtkxljfyk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gekxgvpzt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gehskmfmx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvsesgipe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gzcfbhfwe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gijmrgppi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gafheiuwh.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/guijtnvoy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/ginaaffic.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gnqkxzifh.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gkrkljiha.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gsgbvferw.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gsafscnho.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gatfkpzyd.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/guexmkaai.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gjoupwghx.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gpfggipiw.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/ggparjsns.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gszynlggm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/guzkyppxf.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gqdrhwznq.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gwjemlpvz.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gimapscbq.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gisgdoici.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/geuarlpld.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gxmtisnpv.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gzqwyrgin.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gmnrpcvym.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gjxyxnpxf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gjlpclmmr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/girhlcaol.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/guodozzee.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/glbjduhym.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gokiuwsog.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gjsmmsggl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gkheebfni.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gybbkpulu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gzvalrxre.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbdqcozry.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/guqkelfqw.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gsaxcyvde.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gerqkktir.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gmiotxxiv.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/godrmjxle.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gpjtxowyp.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/guyevkzbo.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gqemotohg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbcuuvgsb.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gattkthbg.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/glhkcxjfg.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpbpktzpw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gqqhzwkdf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gnjrbdfml.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gtagewvql.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/glusygisa.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gonizskzi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gijhbpxpx.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbqoeqnay.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gowvmypki.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/giutfymrq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gkgkqhzha.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gcwmlxhbo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/ghxlzsjfx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gppzxcwtr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/ghqwawpln.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/grlhomjxy.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gmkxujglt.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpbxbawcx.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/glicflhsu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gnynkpyxa.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gleplhchj.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gdgjgfybf.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gmgsjjqke.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/grnsuqosf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gvguwxewn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gbuwtuhre.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/grrculyhm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/ghwodoiae.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gpmuhrnsp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gpvzjdqru.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gjperuolc.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gxlrkltrg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gdxtxqclb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gqhennxwy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gnbdzqbfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gmshqtigf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gvtcwjtjd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gfdapdtvw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/givyiumwh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/graatejyw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gkrupubhl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gpetmousr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gmchqtuum.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/giwudbxpt.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gibwysqsv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gpqtnduhv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/ggksvkjhx.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gxkoulzid.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gfkpxsork.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gppzxwvbg.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gtnitzpqc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbsdnzo.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gjwuatyxq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gqwmidxab.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gdexxzzju.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzbossbuj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gaclagdfp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gnlwoctir.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/guuvxoiwa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gvrvfqges.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gnmymlkfc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gywuokceo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gocpgksyd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gbikeohxc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghbhotshm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gymrmfcpk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqepclvra.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gpvquming.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gvyokyskx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gacxlthsw.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwcfkjyjt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gpwiroqbc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gweaidkah.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gegmwwjky.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxzbwhpvl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gedkltmpv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gaiupnmbq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gqkiosnys.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsiirjobe.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/giafvyxod.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gwkimtjvc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gdapkmjli.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/ggnohnvsu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gjzjsydlw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/grygkymvx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gneklerso.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gxndzflch.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gpbacrkvl.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gulgmlula.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gqfffudsh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gmvdqdyui.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/girqrvmbi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gnfvrrcvc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/glwodfufy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gavtstgtb.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gdzwxonlx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/givxqjweq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gcapmzzbz.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gialeyftp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gfhnijsjh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gtojpbpqe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gixaqcwpk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/ggpxymaga.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gdzyvmaqq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzdnivem.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gbrgkjkrm.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gwyrmoldk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gzarpuwkv.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gbnfceaxz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grfmcqeyz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gpxvrcllo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gijtikqdb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gqzbxnlnd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/glkxfngjb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ggsihgyex.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gwnczgszo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gzznlknjz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gnkjxbxau.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gvongsnna.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gaczgsisk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gnmhckfes.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gmrkcnwrx.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gvhhpvmdh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gluasuqrh.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/glvwoihob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gaoujmnqv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/glvnlulmt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gteqhokor.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gpitnbvdl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/glcdmrkmq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gsofxlvqj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gwhikiafe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gdaetjqcg.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gjhylrfvc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gwykovmpx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gbqurlxgw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/grjbacgij.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gzjgzzmts.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/guqsbheiu.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gisupaopw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gwfzrdify.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsmzywnnx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsmdxzesd.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gxowxosvw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfwkofmep.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gwtyctazw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gderblrkg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gonyjxepe.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gvnftclwj.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gggsbodmr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gipmnoqoj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gsaqlxauq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/ghsinjihl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gblxhvcqo.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gfubhnrse.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gbpusocvn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gukcdwvrw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gbgmcpjrc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gxhhstjjb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gyclvichs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gqldjpurp.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gihckygsg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/geauhrkzf.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gmacjwqhv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gygdzebgv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/grnkuxwpk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gugdmhdtp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gcjxbvybt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gkfevgsbc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gkytvdtwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/ghjpveaad.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/ggckgofpc.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gktnxuulv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gkvyuvaxw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gtopjutuu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gnortnjwm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gbzpwhqzc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gjgrjmgdv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gyhhirpeo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gvzhqrhwz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/giquzjbqp.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gqqfhtval.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/grwouqdil.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/ghaposwfh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gwkpuaozl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gwxvlqdli.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gzdeyqvin.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gixobiqkd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gpsepivpk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gjllpilke.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gwgwfcusc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/grdyciczw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsxbhce.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gujxdlubd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gpkxausvd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gljnupzgt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gbobqpgqt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gpzwupiso.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/ggzffaopf.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/garcrdhlb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gedgznotd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gaedpbuzo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gbuqlwcqn.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gbtimbwgl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gwxzgufrw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/geicumdza.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gicqmouag.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gkjwlqvnv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gmssnmsnq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gaksdtxgd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gohczzogn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gfqraibdp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gxoufgmne.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gngzmtaet.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gdoofdenc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gomqehsfr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gedznmpsp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvufivyfk.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/gjeaduots.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpzuuwcwm.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gwllvetho.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gepvnslrb.sHtML


<!-- 参考信息 -->