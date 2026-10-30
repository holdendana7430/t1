代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwkteheq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtkppvcw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gyptbovqj.sHtML

[G05] 继承
来源：http://wap.fanxiaobao.xyz/Article/details/gbnkciqbo.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyjlwofw.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqaizhnn.sHtML

JS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqipgrlym.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcghrvkfd.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtcdqqzb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/glxwwtmks.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnbhkify.sHtML

C#:   class Admin : User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbgloozpz.sHtML

[G06] 重写方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpdlwtpu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjjtzogh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gegnnnkvf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gloyfxsqj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjuymzrd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/giwhodxss.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/glehlmpbx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fanxiaobao.xyz/Article/details/gxnihmork.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkwyayrg.sHtML

[G07] 调用父类方法
来源：http://blog.fanxiaobao.xyz/Article/details/geqhxgtmt.sHtML

Py:   super().greet()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhgpcctu.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmrkuzfw.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/grnkojqsp.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwblxavig.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gvswsyncd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gwlzrotrq.sHtML

Ruby: super
来源：http://m.share.fanxiaobao.xyz/Article/details/guriyadfy.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtndsuiaf.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/ggqeanisu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpluifjt.sHtML

PHP:  public static function f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkgmqkke.sHtML

JS:   static f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gaupigyjv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejhdmhvw.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/glsssgugt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrimrhmt.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gyruqzuud.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqpkvxaja.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fanxiaobao.xyz/Article/details/gwktstvsn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrxpejpw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgeqfxom.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjdhpnpx.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvjhhzdrc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsnghjulo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiwegyav.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gcrwyobfm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaoeclbd.sHtML

[G10] 访问控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfoserlt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhtmsdpl.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gokbtwfbn.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fanxiaobao.xyz/Article/details/gzwedsxec.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gycguxrqm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwuvunlf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhfskvyy.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gltfvaeya.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbqthofu.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gldzbxvpo.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/goirnstlu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgpggnfp.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gohowtcsg.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmexntlkm.sHtML

Java: public String getName() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdudkziba.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshoyjojp.sHtML

Ruby: attr_accessor :name
来源：http://baike.fanxiaobao.xyz/Article/details/gejwgaqqw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjjhokhb.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxrlstso.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gmpmyjnws.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcztfrfux.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtymgizde.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggobxgazh.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkfiergft.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyczrcuib.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfruieuq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/goauudyep.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxkuzwfmh.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyvdbebb.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgjqxqht.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gpqqfzysf.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gvuhcuxbr.sHtML

Java: u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsvanser.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfqkromq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimgzwbhw.sHtML

C#:   u is User
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyieulfr.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gvdolxcdz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaixqmcl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwiuqglk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gqlxextgk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/gkrycmtjv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwlomtdzy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/gykgolorx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fanxiaobao.xyz/Article/details/geyrfnzfs.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaiqzdbf.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzohkdyft.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsezkdmb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnoqcjen.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gzukogmmf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcyfqdgb.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fanxiaobao.xyz/Article/details/grzudnqio.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvixytjtt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gtcswvjqo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gddhaeasa.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fanxiaobao.xyz/Article/details/gebkexwhx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/ghygxkkdp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fanxiaobao.xyz/Article/details/givandkgt.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gthbwmayy.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gnyxngghs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gnajfopah.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/ginocqewc.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnquachr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbhrvlkb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvkbzwbvs.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhrudgqv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gerboybwg.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfefwujhe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gkosmatcd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fanxiaobao.xyz/Article/details/grpuegwqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfazxtkht.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsibwthrd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurvqwilq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gkancidbd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gaapkafah.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpxxmudlo.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcrnbpgn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fanxiaobao.xyz/Article/details/glguldakx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gckumqyrp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyccnkdi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gagwnnsmd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwdecpil.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fanxiaobao.xyz/Article/details/guulgvlra.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gzvdtukxv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbgnhjhb.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gaeusqfha.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhfdykix.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshdyvos.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gunwyrlsv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gsvvojagb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnleycof.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnhevqsy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/gcucttcly.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gasdofpbi.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfxdwyta.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gzfecxdxt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtyxetwpe.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/giosifjxi.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzyasbaa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/garirconp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/ghigegrmo.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwutlznq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqokxdvf.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gildyjmzq.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gbkfeonjb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvxhikrhx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grqzfgxel.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvbbrlqzn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnkkyzget.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fanxiaobao.xyz/Article/details/gvrxazkmf.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/gohygxios.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbtytvyp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/goaznchan.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkcjbgzo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gbalmqakg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gplibaraf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksadnoqw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fanxiaobao.xyz/Article/details/grubmnjyv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgtvaeqh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzfsekfw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpfomqnk.sHtML

[H07] 断言
来源：http://baike.fanxiaobao.xyz/Article/details/ghncakyys.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gflbwvdsq.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/grotfopuq.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtmtqtgn.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxmrsngl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnugjyeu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gxolrqppz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fanxiaobao.xyz/Article/details/gurkrzhfr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghxuvogwr.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gayxwqqen.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrmwdult.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwlnjmdc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhdjcsds.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fanxiaobao.xyz/Article/details/glbgtqvav.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gwnrbsecp.sHtML

Go:   err.Error()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtquzrgjr.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfalszvn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdsqsqwh.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmxdvkrc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjrsglyc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gahclifou.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fanxiaobao.xyz/Article/details/gtqvnnuwo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fanxiaobao.xyz/Article/details/ginbanhkd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxeqrsku.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjkzqylr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvcglfdv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/gpvnoyobb.sHtML

[H10] 资源自动释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/galmjlwpu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fanxiaobao.xyz/Article/details/gfcbpkfmi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fanxiaobao.xyz/Article/details/gikwyeljk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdnthgdz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gawzcxxgw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fanxiaobao.xyz/Article/details/gsolfyjyf.sHtML

Go:   defer f.Close()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqelandwz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fanxiaobao.xyz/Article/details/gemdbasmt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqzcjliw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glmqkyimi.sHtML

I. 正则表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gckqzotiy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimficacr.sHtML

[I01] 判断是否匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gflykhkhw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerkwxjtb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gdjwacauk.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/glxvvbcmp.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcugtjfr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fanxiaobao.xyz/Article/details/gryubhalu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqmeubesx.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/grvlpjysy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gannvcksu.sHtML

[I02] 提取所有匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gowynuzpp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gybjjorfu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaitltwd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/gweujwhij.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgkxfitd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtbyppcgs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomjswkjn.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/ggjxlukhu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/ghyfciywc.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsyxqqkc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpsvjyut.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gxuyyjbcc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gionwdivm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgrwfvqz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdhtruqg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gucznzqpa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmctmihic.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyggijlk.sHtML

[I04] 正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjpgpwrtc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/glvlnupro.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzhxqduf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gxwyacsvg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gdfsibnyc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfauavfq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmpunxgj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gutgmpkam.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/ghdahxsag.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxironnu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmagyutr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggopddsuc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbpylwyi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddzfntwt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gtxcfogpw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjyqjjs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgzorlsf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gfihsnegg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqxzkaxs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gbjojmota.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpaclaji.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gmeptfrmm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdluoyndx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gohiumivy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fanxiaobao.xyz/Article/details/glspuarax.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwvhyyww.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqynxhhcc.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/gydschlaw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fanxiaobao.xyz/Article/details/gduflufsx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gufcbnnxt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmfrygqp.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gohnfwwjj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzumvepgw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfozwbocv.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbghntptb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowsjjdcd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwghmgyjz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fanxiaobao.xyz/Article/details/gqpvgglqw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzdxtxcy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpglwceh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozhmvjzy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/ginjuvdhg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbuuoebg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fanxiaobao.xyz/Article/details/gldltkimo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gouvjrlka.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwdbsqxx.sHtML

J. 日期与时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyuznqifa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaorlkvm.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gsfnhgbco.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjopygpsy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmrgchof.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/glglhhftz.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpbwrjel.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywpqjrwd.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfarvcbtw.sHtML

Ruby: Time.now
来源：http://3g.fanxiaobao.xyz/Article/details/ghrzhxxkm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fanxiaobao.xyz/Article/details/gtvghumpi.sHtML

[J02] 格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvirbluvs.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbtbbgg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/gvyqnwbjh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbvlewdj.sHtML

TS:   d.toISOString()
来源：http://baike.fanxiaobao.xyz/Article/details/gpbxszshi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gqnbmagmy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gdyscpeho.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjvysqdd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjqlhugg.sHtML


<!-- 参考信息 -->