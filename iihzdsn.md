代发 wailian999

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gosevuquv.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gakjhdcgf.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gcjjiwlen.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gpvsdhvuh.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gdmurjsza.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gwrrveulk.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gtzuskhed.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gjugobuak.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grzztvfhk.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbiqopyxq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwyhpxjlx.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guasywfpk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gtcofxsks.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gfrvxqykd.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gdtsmlqjc.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gafdrkmpa.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gcrgemtmi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpxtoenvn.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gehuggdaw.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwenbpvph.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gaayjxiwi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/glkwlzndx.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gykhmlrev.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkfposswb.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gomnahvcm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gzrogxblm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/guoafaaun.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnjgksnrv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grpcwdxpv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbjwdhkun.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gpmcjdmsy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gsntdbacw.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/ghgmreeux.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/grrkmioir.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gwtpkgmeq.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gfheadyph.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ggujsbzdc.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/grefmslfg.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/goeztixlh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gidpoijch.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gxmikhdjj.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ggecjkdyg.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gujvimcgg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gwhwuqxon.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gnwijpnkp.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/glnudaxbq.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gxuzsauhs.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gzersscfi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gjncjfprn.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/grsbzyoig.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gopjbxhwt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gyhdxnqna.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gdgclzbup.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gyimuhoob.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gagiimnpi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gjypnckwm.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gbaxijzhq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/goyfkntgw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gogxtzkmx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gkjtgdeob.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gooffllcw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gkqqzteks.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gdauxidfj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gsndfabja.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gczifiptf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gzjokxtmb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gtwxkkptp.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/geymcqzko.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/geuvguwoq.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gmxlzjzte.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gxzcomjhl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gcnzotvba.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/grvwnzfiy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzpfgvmkh.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjmlpccds.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gehgwkrue.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gevoccycj.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gorqjmgzb.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gpmkhlgla.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gxovbheqk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ghgyzgaiw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggsymxfyx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ghlryyuuj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnbucqeaf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gmjmhlamm.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gapagibdp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/ggzntauki.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gohukhegl.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gtrubtaua.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gskmcmwzn.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gttfhtmwl.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gmhgycxco.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gwmkuidex.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gpfpeitsk.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gmrvssrom.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/ghkytstcx.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gxcinzqux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gpiftauci.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gvwggjjnd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/ghcgrxyqq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gqazkyjzf.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gshtohjvf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gjkhcfmdn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/glejehhru.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gdbkunucx.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gprltstkd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gddrcppkn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gauyujfhb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gbimlngif.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gefunefqk.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gbpbxxsxo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gvghvsloj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gctattrvz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gpzoguatc.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gicbgbfsw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gufrukcbw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gehxmbiuo.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghwtzwxzw.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gbszhwjjc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/glvnyxcii.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gqfnflvxj.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gnllztaax.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/ghkdlthrf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjqlhnmxa.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/galjreymt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvorcqluf.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gvyiesruo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gydqpclbj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gsmfgnqry.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/guqdjpbvq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gkowwvmir.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gvhohofoc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gjovnobpd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/glyhvfrmt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gpmthdyis.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gkbpsugno.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/guzmmkxfe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gdlmmqsrn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/glbdnzkam.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ggyweffls.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gxrinnqcc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/grgtwafky.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gmxwlvkof.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/grggikmqu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/ggoiytdbs.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gprboiuew.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/geyeqiyqt.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gjjuwpavo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gadwvxcuc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gixgfezzj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gnxatrvxh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gjicieneu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gsfgivisv.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gqvltjaje.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/grdsdjciy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gtpgoehpj.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gtezpxyvt.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gkvbatgxw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gwujfwzdf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gxatwudue.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gygierfzl.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gzqbdwthq.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gtkvzrhur.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gqetjjrff.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gdhvrngwg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gmizeiamq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gisanxucm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gvfjiibrk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/goinpbjsi.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/grqtouwfl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gyumlnamx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gqehjtspr.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/geqeklyyi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gyhxxxboo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gfvhymzit.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gzbtwuahj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gcpdhiabg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gwhlplldz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/ghzfyxjir.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gxngcyneq.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gazcxqvku.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gaqwhilxp.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/giuxiiinc.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvqarkipx.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gyflododb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gbqtgjxhd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gnwmowfii.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gxrtbryts.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/grjrnucof.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gwdaboepq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gqkzghroa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gjmlfpbsj.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gcgpzkzkx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gefcfgrbw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/guziluxva.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gizhgvdan.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gyendgbpi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gjndobubl.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/geitmwpcz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gfnbwqjht.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gqoxvqnqg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gbzjcojto.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gyvxvpvlm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gxbbjfavg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gzkfatrmv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/geazlgxdr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/grpmimemd.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gyowzybsi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gxfvugzfd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gkyrszacv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gkawjozkx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gxeelmtyu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/ggbgirfyt.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gvuggssim.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gopnzkhdj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gugdylygt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwrncnzap.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/grwcunbdp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grcqqaxxo.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gikyggmut.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gkjwicpzn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gmktufbgo.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/glhehpqrf.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghguyncif.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/goxlmqcnv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gmflyyigx.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/glrbjbmav.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gdncvsike.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gxwounaez.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gmbtxlrgw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gsjjwrlqb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gsqnfcgww.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/glnxuavrr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/giunxobjs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gyletizct.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gocqpnats.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gqtacjjld.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gsafuxzdx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gauudlquq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/grxadpqov.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gejlupbjj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gevipgpss.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gtgilqijj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/ggvwyrpyb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gfulddpes.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gyupkgpxz.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gawfhdiqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gdzajmmjs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghivhjzyl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gpehxcrdv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/ghikipavv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghphnhvxz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gehbvauvp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/guriehjra.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gaocatmem.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gytdvrwpy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gjxiawfpx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwwiwiman.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/ghqybcudq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/glmjpcvii.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gvmbeskhl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gtzpijqhc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gwniitrvc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gqmrifulb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gtujpgmvu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gpmqhirar.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gnsqwdcat.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/glxpfzsaw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gcseafggo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gholcbnsi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/grjyrnyhl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gltpsizjp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gbtytzopy.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gxycqmnme.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/glthaqxmo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/grxujtlki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gkrnmdxpc.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gavahgkhb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gltzuwwki.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gngxscuvx.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gyxpkldkr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gtaujfnwd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gvbgnsncy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.zdbjq.cn/Article/details/gdcfcpgpr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gjmlerrtr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gerfhnvfo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqyxupus.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/girzxnohm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gocjhrhhx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/ghnfmziyz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gudixvemx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcpbvtjxr.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gesmadggy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbyvmwvir.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/ggasbpcvl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gkkssrkzp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gttxrptks.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gxqpacenh.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gaxdyxybs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gkasjhfvs.sHtML


<!-- 参考信息 -->