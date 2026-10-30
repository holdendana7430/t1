代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghiitjmah.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmbauwmob.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmedfqvhb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsxmkfji.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghtkraijo.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gwiqunbow.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gqemvqhnx.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gfxyzkjre.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/ghliulbzy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gpyfhqsoh.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdqtbgkor.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gofyeuerp.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkqwixaxp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gmsfgkjdn.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gdqgmhoqb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnxqagwqd.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/grsuhkmvb.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gcuklayuz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvgonqyfg.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gulswjbvl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gstjrpppv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbkegunlz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/grirvkrqs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gxysxoapn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gxjocrjvt.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/glbhltzqr.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gawlpiutq.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gcuvqiiiu.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwtrehayr.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcmujllww.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gdfykslze.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gflimakmh.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gbtghbbkc.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gtqcifedq.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gqvhrikgw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gbigqsqtm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfgnvxobi.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gntoxoops.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gucsktzxq.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gsslgbfdh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gylwampwg.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gmvmjzrnx.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gydyirgae.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gvrtxqpyf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gqwtmxzcx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwximpdi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gtexvpfds.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/geugitvtl.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/goeymmxtb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gpeevyftu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gqlydvmqj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gqlsalqhx.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gzjykfvbp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gdteyutrx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gkbdvgrap.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gyyeyjolk.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gonzroyon.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gblaycwgp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gzvzzzqjo.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gdnvoonkd.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/ggqklecem.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gnaxmdage.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gbdeqlvtb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqormfpwf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gcavnhqll.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/goujztfbr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ginmkbzwo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grrahzzbn.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gucnwlhti.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gamvrqhre.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcsuidupg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gfebcesmd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gjtcvjmcx.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjorjbgzw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gsqleqcod.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gpxyxxlln.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gpclzrmes.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gvsktlwkm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gfpvbvzrq.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gsvdfrdqk.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gflqkpjfq.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/giwvtfxbe.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/grxomeivt.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmcohyybe.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gcctqsvdv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gwqdoznqg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gbgagxewy.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gqxrxpjsc.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gblridpmw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/ggoxfcwqw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gzezwjwvf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gysvfntrs.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gbmhttegq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/grdwhgwnq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gzfylgcvu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gvzdketor.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gfwksdqbu.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gqxcmnhis.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gabjeghcc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gddvlyvmr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gsmnmrkeo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gdpxdrxgo.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gsqfeuhed.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/goqjxblwv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gkehjfrpn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gkzmmnvlq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/genktjhyn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gsaeheivo.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gsfzswhvs.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/giyqlfphz.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gowngpkjn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gcxhkeogx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gqpqhgvrn.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gvfybsypt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gpxabfkep.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjhvnsaql.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gzkcpkhmc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmljilwet.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/ggijbuzkz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gthpvxzgc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gtuvivrkp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gwshnkhmn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/ghagzuqgp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggezjlydc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gqesyiczy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gmagtcwqk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gmhukoovc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/goheejsmw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gmsrlsxbi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbelpqboa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ggkpejwjq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwhvemoeu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gpqsrzzid.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gtkrrifyv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gxuvkcgyw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gtkwmrxtj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/ggcufykrz.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gtujchypv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzddybueq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gacpntrpe.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/grojguorf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/guefiyqgu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gmoapzvgf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gehjtncrp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gkykzbuhr.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gsocyeltp.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gxlenttym.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gyazujahh.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/goyrjcwug.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gdcjmbrmd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gspvziyrz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/genqmgedo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gcolbajhz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/glnxtcfep.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gyzfpbcbb.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gjefotxjg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gmbfpoqev.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gglloklha.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gvepkrdqv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gjqcrgenn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/grfutlgmn.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gxsforduy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gsnlvpulg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gcblyovha.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gjdblbhbh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gjcsrvqhb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/ggaarrwlo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gmsrjhyju.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gqfhpwqed.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gexhruwnt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gjloriedb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gtudxucea.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gubmwfrqd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gdgtezawz.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gjlnwdozk.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxqvdlwoe.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqwyiyrsh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gyrndbtpo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gtvvrsvmv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gdkuyapqt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/grwbrlumv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gqkpnarmr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gcowfjihh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gejwyacvq.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gcxgpaitd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/guupdnlcl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/glisqpkzj.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gonleynhq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gzxprpmpo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gfcsjncma.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/grfzgzbuj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gyhtpsvmi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gfdkxunuk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gqimwlzgn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/ggfexfxfi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/grwqsybbr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gzuxfkdrv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gfxpnxwnn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gnyremqpp.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gnsftbkve.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/ghgyktkie.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gtqwgkput.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gdwgrseal.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gwymvwoin.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gfkwryqcx.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gfaeaaugu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/glkylswel.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gymdbnorp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glzojlaxg.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gnnhuetuz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guyttchxz.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gmkksobyb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gytwuntwr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/grirzyplb.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gditwsqgl.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gvevsmmbt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gtahhoeta.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gmixgzyav.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gqlokmngw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gzepoavmp.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gxswidaxg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/ghonebexg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gnlwampco.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gouuyzsix.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gefhklygq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/ggznhtaxm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gmmcfvbwb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/ghuxsuzyz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gxyryszxy.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gtjdnojtm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gahfjoiil.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/grcslnwlr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/guzpgwzkh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gxlwmswno.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gwdnyjhqk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gncvzzzhn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gklbgpcak.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/glcdipkyd.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gkepxtlxs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gwsfquwnu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gygsxmwvb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gnxhcclcr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/ggycofzlf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gldeidwcs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gsokxoott.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gxkrszuma.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gayrsjebn.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gwiylttuu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gmdjwhnby.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsdlzpnvp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gmydwsdrk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gdatcnbba.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gchxdytcx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/geajmewdt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gbzmztnby.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gfmxuiuws.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gzqmubtqs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gmnojwibn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gbrtjxokv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gipzhrpxk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gasnrcgfm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gzpkdivsy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gpbfmxoif.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gzehaknmm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gishqtqks.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/ggtwaxyym.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gfyjplorq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gvioizari.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/ggcsobgau.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gckgebvds.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gauiogadb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gcksrdsmz.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gogqlbyke.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gdmwswxxg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gtmgnkymw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/glwzjonnb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gneyxmvur.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/ggevkjbxr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gclsmfzoj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gbjbbdorr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/glgrdhbrq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gsyypvtru.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/glzhoyshd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giagzgoeg.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gfvrtufql.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzmqsuohy.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/ggfvwftma.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gazmdtjrd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gjdcswget.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gpnmzubvp.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gpdpjiilh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/glzzauwrz.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gpyqbfkyn.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gbnanbizf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gixuxxppv.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gxqffzurq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gdlzbtxpg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/geyqtihsr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gxqnlxmcz.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/gajnevgzn.sHtML


<!-- 参考信息 -->