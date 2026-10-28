代发 wailian999

JS:   this.name = "x";
来源：http://hz.tianlin.xyz/gtzvjwjniy.html

TS:   name: string = "x";
来源：http://hz.zhengqikj.top/gtbrswzvrs.html

Java: private String name;
来源：http://hz.haohaochexian.top/gthgmhnfeg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangtech.top/gtkjfirzho.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtzjxppfzp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gtkeaearha.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtpwzgjerv.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtwpsxhmly.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sweek.top/gtpftcjmoc.html

JS:   greet() { return this.name; }
来源：http://hz.52xcode.cn/gtmyvggals.html

TS:   greet(): string { return this.name; }
来源：http://hz.smart0.xyz/gtdhjycrvk.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gtvzvcsxqs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtcukaenkh.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtnenzffjl.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtfrzoztcb.html

[G05] 继承
来源：http://hz.hfpthk.cn/gtaxypdsac.html

Py:   class Admin(User): pass
来源：http://hz.snrcjt.cn/gtyukdsjvt.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtcewnpcsr.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtuknxsoeo.html

TS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtsfqcjcca.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtxvresgjn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtlmfqnher.html

Ruby: class Admin < User; end
来源：http://hz.chenzaomai.com/gtpjjptqtb.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtpbbzaddn.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gtraptohma.html

Py:   def greet(self): return "admin"
来源：http://hz.shzxlz.cn/gtsjxcxqzq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtoxbbgcfq.html

JS:   greet() { return "admin"; }
来源：http://hz.daxiang520.top/gthynyjreu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtbitwratf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtcqqnrfpt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gtvltoaueb.html

Ruby: def greet; "admin"; end
来源：http://hz.yuxming.cn/gtmqhrrqcg.html

C#:   public override string Greet() => "admin";
来源：http://hz.ybcxt.top/gtrriectwf.html

[G07] 调用父类方法
来源：http://hz.jqgfzy.top/gthluyjqmv.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtmitvyigg.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gtpifkxpoj.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtaqoxzzgk.html

TS:   super.greet();
来源：http://hz.zycfv.cn/gtigjanmeg.html

Java: super.greet();
来源：http://hz.cucudq.cn/gtswsveeqs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtoilgkfcv.html

Ruby: super
来源：http://hz.jqgfzy.top/gtspucfqwb.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtzpxddjta.html

[G08] 静态方法与属性
来源：http://hz.daria6918.cn/gthygtkcet.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nwbrower.top/gtpkunkszw.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gtvavgihlp.html

JS:   static f() {}
来源：http://hz.hammf.cn/gtcffyyalp.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtqhwesark.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gtlchdgqcf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.mhx1999.top/gtgovdvtyf.html

Ruby: def self.f; end
来源：http://hz.wangshuangyany.cn/gtxwryqrve.html

C#:   public static void F() {}
来源：http://hz.sweek.top/gtohmdbzdg.html

[G09] 接口 / 抽象类
来源：http://hz.zhoulong.xyz/gtvpafmwue.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtjaqlaltr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgufenzy.top/gtvtxqpdbh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daxiang520.top/gtvqyjeuza.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtnwohnloq.html

Java: interface Shape { double area(); }
来源：http://hz.daria6918.cn/gtwvjyjadc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtezgobwfy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtdmpdaldr.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtwsneztkd.html

[G10] 访问控制
来源：http://hz.shanyushiyangtech.top/gtfndmtvwr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shzxlz.cn/gttamjqjcw.html

PHP:  public / protected / private
来源：http://hz.havefunace.top/gtilhjjutn.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtnsyyqibo.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtjofzogwv.html

Java: public / protected / private / 默认包级
来源：http://hz.daria6918.cn/gtrupyqbib.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtzaalfwgl.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtpqyebwmp.html

C#:   public / protected / private / internal
来源：http://hz.yongpay.top/gtymppyzwi.html

[G11] getter / setter
来源：http://hz.cdnleiting.top/gtmpqxukzx.html

Py:   @property 与 @x.setter
来源：http://hz.tian-w.cn/gtylrgpzhk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtdzqfbiyv.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gtzdpngbcv.html

TS:   get name(): string { return this._name; }
来源：http://hz.hammf.cn/gtnlpxkugn.html

Java: public String getName() { return name; }
来源：http://hz.gzhubu.top/gtcetyuiaq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtyjrreaur.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gtfzqjcanr.html

C#:   public string Name { get; set; }
来源：http://hz.xuanzx.com/gtyqgwctmr.html

[G12] 对象转字符串
来源：http://hz.cheryme.top/gtulduelqh.html

Py:   def __str__(self): return self.name
来源：http://hz.316326.xyz/gtmcduakcu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtwmaplmdr.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtmizliyoi.html

TS:   toString(): string { return this.name; }
来源：http://hz.yongpay.top/gtlyewavaw.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gtwziakwkv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shzxlz.cn/gtzbongvav.html

Ruby: def to_s; @name; end
来源：http://hz.hnxiangtu.top/gtbhibtlzg.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtzfolpvoi.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtspnvvrjb.html

Py:   isinstance(u, User)
来源：http://hz.nwbrower.top/gtddxsowdc.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtrbcvvtlx.html

JS:   u instanceof User
来源：http://hz.jyoumei.cn/gtzrrcugph.html

TS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtyvujebmq.html

Java: u instanceof User
来源：http://hz.hywenlv.cn/gtwpmsknyf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gthqjolyvl.html

Ruby: u.is_a?(User)
来源：http://hz.xziqi.cn/gtimuazvmo.html

C#:   u is User
来源：http://hz.yonumen.top/gtqlebnqxb.html

[G14] 数据类 / record
来源：http://hz.ybcxt.top/gtgfzqdmwg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.feifeiyinyue.top/gtglwripbm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtkxwbcllk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtqcnwqmzf.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtwjvxlbdx.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gttkgeggmo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtcuecjghf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtiopoueus.html

C#:   record User(string Name, int Age);
来源：http://hz.sweek.top/gtoitwcsqf.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtawnixenj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtnwmsvjks.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yongpay.top/gtcrdohhrm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtmdolfssc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtnwfklzip.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtitaagpvd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangkeji.top/gtidasqbxk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtccojogpe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtssyqjkeh.html

[G16] 对象转数组 / 字典
来源：http://hz.birdmap.top/gtusbaxtcs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gtadjvihku.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtpcqxadch.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtkuyiystk.html

TS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtfqaepuxw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gtajkgzinm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtmzzyagwb.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtpzlapjms.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtgfypnjsz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmxdtujzv.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtihvmwtmv.html

================================================================================
来源：http://hz.yj20258.top/gtyqdfrxrq.html

[H01] try / catch 基础
来源：http://hz.bjfxy.top/gtyhmhseac.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtgmpcosyx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtqpmvaplg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtzzxukyrh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtpvktnvuv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtazfsaast.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtxftpfhqd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangdashe.top/gtaiakwykt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.quarkkingdee.top/gtickduaja.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gtelvsqsil.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtfbruzwja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtslpztvrh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtiiabvaef.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtczjphyvk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtxdtohilu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtdzdsevtq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gttmhvilow.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtepnopwca.html

[H03] 主动抛出异常
来源：http://hz.zhoulong.xyz/gttzzcedum.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtmcfcnuca.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtnmnpylis.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtmncbzkza.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtghgtlqvt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtaoasumax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gthdcqiodu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtdyxchlov.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gticnvtkoo.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtzikcqfuz.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gtcfanfhxu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtoqdfbwoe.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtfdkkaryv.html

TS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtgisjzqwy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtqiqiswgt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.mhx1999.top/gtocdwdzua.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtfhvmotyp.html

C#:   class MyException : Exception {}
来源：http://hz.xinyue.icu/gtfbcskikk.html

[H05] 捕获特定类型
来源：http://hz.cheryme.top/gtbixrpice.html

Py:   except ValueError as e:
来源：http://hz.316326.xyz/gtvfrgyuby.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gthrfyatnb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gtviwollyh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtjlpsjyff.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtshlkxxux.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtffbgduiy.html

Ruby: rescue ArgumentError => e
来源：http://hz.sxryk.cn/gtezgpulmk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtfwqhtchu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gtmpzvaqjl.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gthasxrhir.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtbfmzrann.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtbbgvivsx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtgrvzqtaf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cucudq.cn/gtpmevpokx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj202588.top/gtgcsmvuse.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yonumen.top/gtajwpmotj.html

C#:   obj?.A?.B ?? default
来源：http://hz.snrcjt.cn/gtlfmegifh.html

[H07] 断言
来源：http://hz.daria6918.cn/gthuzvgxfd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtfwuyykfo.html

PHP:  assert($x > 0);
来源：http://hz.jinghuilouyu.cn/gtpforehhm.html

JS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtmgvvfgru.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtbgcayyik.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtxhnpbnlo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhijiandao.cn/gtdgmghpba.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hysaishi.cn/gtghoimpwo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gtjcpdjmme.html

[H08] 获取错误信息与堆栈
来源：http://hz.xziqi.cn/gtjixefujc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtvvkrewdk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtgiuqkvxe.html

JS:   e.message;  e.stack
来源：http://hz.chenjidiqi.icu/gtrrubouxt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtusdmyoee.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtceaegygj.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtokmxaxgc.html

Ruby: e.message;  e.backtrace
来源：http://hz.cucudq.cn/gtzijqrklj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtvzdoptzt.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtckvyfxcs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtnscvnkpg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhaomingkeji.xyz/gtbhxlwxqw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gogol.net.cn/gtsogabvdo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shangyingyoupin.top/gtuqnymhpq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtaxsvbhlf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jyoumei.cn/gtxhyudnic.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.smart0.xyz/gtseoqgoyw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.quarkkingdee.top/gtazrleqex.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gthdkrskim.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtqyijmrqg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtrfvtseta.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtkybzcxqk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtwmptqywz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtucdhncuy.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtwrjngsry.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.andypj.xyz/gtpygtgjii.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gthoohsvsw.html

================================================================================
来源：http://hz.havefunace.top/gtqskpohfn.html

I. 正则表达式
来源：http://hz.yueranfly.top/gthsdvurtd.html

================================================================================
来源：http://hz.daxiang520.top/gtoupyonhd.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtdzcmfkny.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yonumen.top/gtncjzmjtj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtelngyima.html

JS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtifsophif.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtuwpzssmf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtzbfhbhbw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtgkiacnqs.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj20258.top/gtammpsgir.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtbnvrijnr.html

[I02] 提取所有匹配
来源：http://hz.gogol.net.cn/gtawbfeysr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtomzubwsl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtaoxpkwro.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangkeji.top/gtneraojpu.html

TS:   s.match(/\d+/g)
来源：http://hz.jiagoushi.top/gtjsdzlfpi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daxiang520.top/gtzhltvukh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.meibo888.top/gttflffdrd.html

Ruby: s.scan(/\d+/)
来源：http://hz.zdqjudy.top/gtxwcntdcs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtwqgtwlpy.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtqfuzhlkx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuanzx.com/gtyrxvzrtz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtqukyjwnx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.316326.xyz/gtyixhpmtr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenzaomai.com/gtenzemgxm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgfzy.top/gtdphnmrnn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtnsjaifsz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xylfe.cn/gtumyvbjvv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gaohongyu789.top/gtqbjgofbg.html

[I04] 正则替换
来源：http://hz.yangfankeji.com/gtoywsfkqb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jiagoushi.top/gtppgwlohm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtzncswvwy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtrcoxrhun.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtqlpjfmgj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgufenzy.top/gtflueoylm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtmqchsmku.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yanxiufei.cn/gtncayzueh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gtzgzzphsn.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gtyrababhn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtvsqukwpr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtmqsnuafq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtaxccexco.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtcmbwowxt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtayikdetm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenjidiqi.icu/gtibsssxvj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtymlzvady.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangkeji.top/gtbuhpicpj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gtplffmelg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gttdnruxfz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtlzsxpied.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shangyingyoupin.top/gthchyunci.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtjtsdtorj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtwzouplrd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtggaxrefh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yongpay.top/gtthshmvyu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtifyfgpco.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtqugyjmbd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yvedp.cn/gtbmktmjpv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jyoumei.cn/gtxjgkptfm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydjk.org.cn/gtqzwldhqs.html

TS:   /error/gim
来源：http://hz.52xcode.cn/gtziosilpr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtcolslgvn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sxryk.cn/gtrernkpbz.html

Ruby: s.scan(/error/i)
来源：http://hz.kuanghao11.cn/gtvpfcjnjd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenjidiqi.icu/gtzxgvbioa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtlojbxsup.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtnobpypom.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxinkj.top/gtznhgknxa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pycfn.com/gtpgcgdoec.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtpbzjwlsr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtmpfcaczg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhixingplan.top/gtxppihkrx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cucudq.cn/gtoutzpzod.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtpecuqjss.html

================================================================================
来源：http://hz.ydzc1.top/gtfbualkir.html

J. 日期与时间
来源：http://hz.gzhubu.top/gtqieggxxj.html

================================================================================
来源：http://hz.cucudq.cn/gthjdeqjeh.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gtnsghcqnv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gtkpkgjejg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gteydvsarg.html

JS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtnvlnihzz.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtivydereo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zdqjudy.top/gtjmsffoyj.html


<!-- 参考信息 -->