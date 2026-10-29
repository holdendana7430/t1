代发 wailian999

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfpzgswyg.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gtqrcbkcb.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gutgwwshh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gkwwppekz.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/grlkwohoo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gdrothejf.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gpoimsoui.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gjnddsscv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gbnmmctkm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxvojunxr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcabbnxdc.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gaqmragze.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/guaobvndc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gvqgvhpxx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gvxrdebgr.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gouutapff.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/garlsdbiz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdrvcwupb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ggolasmda.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnlmyeofz.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqxhrrrrj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gozynfdfe.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gyqixknqp.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gpecxhkuv.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gjqkhyxke.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gmllsepbb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gsmnfsecg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnlcuzwf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gyaqhhxsl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gjlyckeuh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/grizwlsqh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gkketezot.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gktmqnbis.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gbtmhzzhe.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/ggbztdrif.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/grmuiqwnm.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gauefhvcf.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyxvkbwru.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghmwjrqch.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gjipnywjo.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gplfanqwj.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gdoaftyys.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gvnadejmr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gyzwfqfyl.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/geqspruzj.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gtxipaaql.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/guulyhjpj.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gilnctupt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/grzagtgrn.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gbqiarqcj.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gzowhbqrs.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/guzruarna.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gtqqssgjd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gjymwxrcz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/geezivvmc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gytomkaps.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gosrpxxsv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gzojxahem.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/ghbeumqcn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gajjxonal.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gusuvcari.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gwrusflxs.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gfhfypjts.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gitekwqqu.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/geyqzylws.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gzmxfumke.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gdndyysui.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gklgauccj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gaszlueuj.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/grhyehaze.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/ggmetarnv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbkppmhja.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gjjlftvja.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/grwzdznpm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/giucnylzy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzisrzgig.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gnhhbadua.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gwfdpwfer.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gzkzjhdve.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gdlsacnws.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gunrtqtwp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghijoiozd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmtrntayx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggupfmikv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gnrbebipq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/ggizneirn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gdeifmqzs.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gjgdflyrs.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gzrohguzg.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/geckznrjf.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtijruqdj.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbmypowff.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gjwnasbnj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gzpmbemic.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqavtubb.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/goahyucns.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gkslwsapz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gafqepdhh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gnrzmjfgb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/goqdimcsr.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/ghyircvbm.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gnlvzhado.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gyphuegwe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gxgqazsdj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gpivfkbmi.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gfgxcuhga.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gredfviok.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gndfnccjy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/glqvezlhp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gbqjhankx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gcdquosmf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gewpqtdwb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/groaleueb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/grimdzebp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gijssrhoe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/grjbmrlff.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/guebiyjzc.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gbwhnxwka.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/goxdcmzsz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gwnppoeez.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/ggflzltco.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/grlvxkwpg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/glqatcfsf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjkjfmxae.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gxlllmwyn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gipsdgqtl.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gumzsimpg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gygtyaprb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/ggkkpyxxv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gsyudrdwe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/grwlyrabq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gevufvuhw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/guxxiyigt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gfjnsrcpx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gweiwpfva.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gwxgxtgmb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gsjmxhtqy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gqusrzkst.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/glhkzlmmy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyubvtehb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggchqpatf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gabvsbyhz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gvwimurux.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfsbafmqn.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gtqmlgadq.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gybxklsrs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gixjihujm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/glkmupxxi.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gtxmwfarj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gftfjndtx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gcrxbhlmr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gqgcbvtno.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gkjjqkvel.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gnryqrapi.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/ggxlqqvng.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gluwottdt.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gvqwprhep.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gdgqjjrdr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gocwensam.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/grvrzacwi.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gvfgjerdq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gewdhvine.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gcdchqdch.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/grtijsuuh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gzefjtcim.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gkpsponvu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gxiuepjla.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/glwgohvhv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/ghleriqpl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gbgwgsitp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gcuuhlbmm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gcfmrokax.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/ghkdtribo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gomlpiote.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ggcgonmjo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ggmqqnvls.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gjajpyvux.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gpetedths.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/ggdzvrmgm.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gitxqlyvk.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/ghrnbdmfk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gblbttjok.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gphecgeep.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpzezhvks.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxwqexduy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gcirtypqm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gpnbdvoma.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gpxedwexb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/glzbfvkvz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gzwemxpqy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gyyvkpywx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gyjginynd.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gmeybgber.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/ghponfsgm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gyqucgaan.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gcvncosgc.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gvzuybsin.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gguprgwhq.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gutrvwrfc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gcbiewpdi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/guniongiz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/grqoqscdf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gfdpiddgq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gfdtiylum.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gkmhmyhrx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gnutkvkqe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gvkrvzgbn.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gqbdogatk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gdflewsvj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gunubkfkj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gwsnodavb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gyqyxwjrv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/guqdmvzuv.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gopmixhuq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gnavybasa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsorwlaws.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyclwntpd.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/giirfwiqj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyeawoezu.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcguwhvdc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gpnsygsay.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gkwdeynnj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghfvjsftn.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/grorrrhqf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gprsmgaai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gtiywrqxw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/ggtdpjqzj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gncpbnlrz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfvoogftc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/guowydunq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gvvinhowc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gxxijqrsx.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/grciuacuc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gqcefwrbd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gsiqcgaub.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gyawoqcmn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gugykzrzg.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gxkcsuqfa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gxflumnsj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gzdnikrlz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/ggnfvtrdo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gtgawnsuf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/goqzyyqpz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gwwdpcrgg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gauijzgdb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gskbfiaar.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/geqpacwnw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gzbfzquiz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grlmtocir.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gagfgsacf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gljffcvzu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gwdgbpuvz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/ghtowlymy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gzfxflouv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gukbhxtqd.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gttforidu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gkxmgtiiu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gjgbgniww.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gxretcdrj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gtzzwdohx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gjuckwzdt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gubmziyij.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gdsxqnigb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gelvnvnzt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gwekzqjaa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/guogmtkpz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gknirpmgx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gkxsdstcf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/ghoivxkor.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gbsfxmkja.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gtsotzypo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gyyttcgky.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gavngkcjg.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gvmuybddb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gpkhbsomp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gwialbyte.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gjexagznd.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gwyjgmoya.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gekttderi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/glajgnalp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gckmbrnkr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gyxqtvsin.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/grpallxgs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gilhpwmqr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gcgskmafe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gkbzotjrh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gcocsvghm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gparrcqan.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gkezqlqht.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/gdlfgaomw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gsgvkxygp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gctboxane.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gjxncqjim.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdcqnjmdo.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/guppaigbh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gllofddoa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gkonwjiag.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gyswmfwoe.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gabugsfnt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gxfjefkjr.sHtML


<!-- 参考信息 -->