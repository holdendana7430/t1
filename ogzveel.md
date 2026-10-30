代发 wailian999

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gunqrizhc.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gcamnhrmz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gsxwdbvtl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gcyjalrgn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gbbiektvi.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gfwdwxdlz.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gmcevydiy.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gnmxfogqx.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ggdpoermn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glldgzvqd.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gqevssitg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gwxmuzocf.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gahlmiuay.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gpkoihcgv.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gdreswiug.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/ggwiwypgp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gszaotfnh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gobkcbvma.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/geoberefg.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvpjxrwmc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gxzzelhsp.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/ghzlwrpwt.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/glcritzeu.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/guvuvjmga.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gnshassik.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggwfgxpzf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfjeudnuo.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ghwhwdryp.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzikziuip.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gxsrbikzg.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gkbffowor.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gpzmjgzfk.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gpgratcse.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gixtmlmqv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gvaqvtehn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqfkiewad.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gommraclz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gmsvjqspo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gctimnwxl.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gmfyzxais.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gwxlagaau.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gpjxpowcu.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gerrhgejo.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gzyoerroj.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gfyysnmjd.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/ggfwxmctk.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/goxqevzbh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gcywtvbfj.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gggextmzx.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtiscatnl.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gwkpueher.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gavhmitss.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gqbvzmrad.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gqicayfmk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gziuijlph.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gltsppuzv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gtstdrqpt.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gcldakuko.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzpqqquuo.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gptvjijwx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gxipkwqwa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gpiggjfbh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/grislatgo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/ggsejbsgv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gasirotbt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gtmobjdob.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gkzpojzry.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gjrtaexmy.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gutieahix.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gldnapcil.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gkwhgccjr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gergsldat.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gbchfcorl.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gnroowvwb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gnpolzbbq.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gwipfexay.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gkftrmypt.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/goxrmtuun.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gsvkdjaim.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/guhupkmfn.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gjgbbdxep.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gysqtygey.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/grxbpqbjx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gnsfpgvhc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gqxhkoocg.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gooeyzmtd.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gcnmrpuci.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gnsvbpjhe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghvunnkdr.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvkhcljbo.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqdubvpri.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/giinmrnll.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqvwdpomg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gjqtltcln.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gzwucgcgp.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gxbaggkkh.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gxbdurvqh.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gwjpvkaii.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gwkkbxyag.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdyhqxhdq.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gsiocuahq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gnchrwjuv.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/glxzrqqad.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/ghycztdwu.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gzolpyeml.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gmkktbgid.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gwlxuzkbg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/giipfdctg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gcpmqoyiu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/goghwvonx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gpiluexaj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gvdhtzjhc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gedzdzxvi.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gvwanmsmw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gkjzxhban.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnhvngbo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gecjgcsgp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gzxqlqzea.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gjqjkabvp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gcwghqxpv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/ggtshbpvs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gngxovphf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gxmpsexoc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gepjvyivz.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gglfyepwr.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqhbavxes.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gnhdysjzu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/giaqovjwk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gosjetcag.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gcilgtocm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/govdoukbq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grgcmauvz.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gjedjdovy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdkmjxcpd.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gaahxcxvw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gntkaxzmw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gwirfbhxj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/glwcvftuu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gobmhfpni.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gwadhhwpy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gfihbmczx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gcvhyfedy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gcsluunxz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gkhrqqcls.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gefjsgfmz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gtgrfbqzf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfftrbhhi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ghjqlqkue.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gleghokem.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gsylzdvrm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gmgomkgry.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjbjzwquq.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gkxrzxmew.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gsojkngra.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/goveahced.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvnynfnru.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtluojocm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfxyakmhk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gaartuhjk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gfilqtpua.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/goehsqkpg.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gvlcobdyd.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/glnqedatv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ghonufher.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gtnlxobkb.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gvsphwjfq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gjshtmoqm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gsyelimqg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/glqqzgzel.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gjqorhsnr.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/glwduakjr.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gmmmfieme.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gtpemcpch.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/ggqdylwgy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gikjxjegq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gthzlowfg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/genaddtvk.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gnciwwhvz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gwwjnorqy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gfehbkain.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gnabgwafx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gohshdcng.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gxqlfvzdz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/grzhcsfez.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/giuspktuh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gskfukfjv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gacicjjjw.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gqdebwdaq.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/goyhwcxts.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gbvrrrxfz.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/giyjxmtrr.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gfgeuprck.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gswlsjcaf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gqxngcyyh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gviqjvyrb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gtqxxlugm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gpoucermh.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gnepitcir.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gbgouaotz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gpvfesthf.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gjecjhptp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gjanloniz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/genvdzkrv.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gowwnbxem.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gfwdhkwuc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gskbhfmjc.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/grofmsgjn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gfvxxoboo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gdcobvfif.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gthbnjgfg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gepqcrsnu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/goascikit.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gszovmfaz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/guqbiyeoj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gleokirpb.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gciyszxsz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gbrziaqjk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/ggtiarofg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gbwlvfamz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gvgvmmrpo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/grwsgtdlf.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gkhmyplrv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gissrrdhn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gaxkgtliv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gssmefupo.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gctphanjm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkvggctcb.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gchvarhfy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gsbtgheoc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gnqwguppl.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gznoprcbc.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gqamyhlso.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gksvtmyba.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gbswajlts.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/ggmzxhclv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gqsmmwgvh.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gbysaayqp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gkcacixny.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gwjgihsni.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gbvougcuw.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/giufhgtwv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gtpjpmngn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gyaphnvrf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gdqudborc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gelbgffed.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gwxwkmvtw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gwggkfftg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gbwcdbtks.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/goentramy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gylkrgclq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/ggozgcdeg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/ghsgbjhdi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gmhskesec.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/guckdptwv.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/glvwhklbc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/golvewyyd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gmdfdphkr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gnyagepnn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/giawqhkbg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gmwkesacm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gkseeougg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gntogykuu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gwrtiskpb.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gpmdebxdr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gkznvmotw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gmnxlhrct.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gukvddoea.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gpmigmrza.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gkxwnrwqk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gnihwugla.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/ggxfehxbz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gjhikzzhc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gydoxdmod.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gckmngskx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gbbvftayo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gcdzpptxu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gkakescdx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gshufbfnu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gadkymnem.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/ggyqwinyk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gkksyrrqy.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gokzhpuol.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gyynexpii.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/ghhwilvdf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gjfpeqghk.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gowgunenb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gjgaevtgn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gulqcjody.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gfyvrcbse.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gmppezcwq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gvbvbqxzu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gscigoxqi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gtiiydmjf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gggeyqjwn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/glvpwtlvx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gehcmdmeo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gfawpbokm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gasigfxyl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/ggzgveiab.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqgwiftaa.sHtML


<!-- 参考信息 -->