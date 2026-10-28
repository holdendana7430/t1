代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.iojbl.cn/gtlbjshibi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtbgqnqsgv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangshuangyany.cn/gtpncsufya.html

[F12] CSV 读写
来源：http://hz.ywan-chungtsiang.top/gtuxrnqpui.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hammf.cn/gtqxwtajdh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtnrvwukxy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gtuexpczii.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtrtadqezl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zdqjudy.top/gtmoreojmd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tanke756.top/gtvenrjxfi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sxryk.cn/gtkokfunao.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gtcruhoqri.html

================================================================================
来源：http://hz.yvedp.cn/gtmfejxhcv.html

G. 面向对象
来源：http://hz.xuanzx.com/gtxtnuskha.html

================================================================================
来源：http://hz.zdqjudy.top/gtabprnoeh.html

[G01] 定义类
来源：http://hz.yanxiufei.cn/gtqdyoaekw.html

Py:   class User: pass
来源：http://hz.sufxvd.cn/gtiagigpen.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtwfurddkz.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtqandpxnk.html

TS:   class User { name: string = ""; }
来源：http://hz.52xcode.cn/gtkuxizrvk.html

Java: class User {}
来源：http://hz.quarkkingdee.top/gtlyslfumv.html

Go:   type User struct { Name string }
来源：http://hz.zhengqikj.top/gtabnulgiy.html

Ruby: class User; end
来源：http://hz.havefunace.top/gtvcuudlcs.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtpnaesagx.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtlduzjqlz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tanke756.top/gttrqbggbd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gtmbsujzdb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fzhhl.top/gtampdvynx.html

TS:   constructor(public name: string) {}
来源：http://hz.xuanzx.com/gtpafhtyxg.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gtfcizxryv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xingfuxueyuan.xyz/gtkeivclah.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuanzx.com/gtujiskzgg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.iojbl.cn/gtsrhmpfob.html

[G03] 实例属性
来源：http://hz.chenjidiqi.icu/gtxnsoavgf.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtssiepsvl.html

PHP:  public string $name = "x";
来源：http://hz.redwolf501.top/gtrmbohapc.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtxtijmvej.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtrwharbzt.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtqtqkblns.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtlpxvmgdr.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gttihwtuce.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhiwuduotai.top/gtkqtcidnx.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtxfctvrzq.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtvseiorqc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtmvowvoct.html

JS:   greet() { return this.name; }
来源：http://hz.zhongyouzk.top/gtlxjngfpd.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtlhxpgcjl.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtokewciqp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pycfn.com/gtxitwning.html

Ruby: def greet; @name; end
来源：http://hz.zhoulong.xyz/gtqjnwwgey.html

C#:   public string Greet() => Name;
来源：http://hz.gaohongyu789.top/gtrodbhovn.html

[G05] 继承
来源：http://hz.tian-w.cn/gtrcngpkjf.html

Py:   class Admin(User): pass
来源：http://hz.guowangkeji.top/gtxlsvqsit.html

PHP:  class Admin extends User {}
来源：http://hz.cashguo.top/gtojdftvop.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtgfwryhuz.html

TS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtesaoocml.html

Java: class Admin extends User {}
来源：http://hz.iojbl.cn/gtckfkclqu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtlzrmeojz.html

Ruby: class Admin < User; end
来源：http://hz.snrcjt.cn/gtgnawfvna.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtdlnvyddl.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtixcfibjp.html

Py:   def greet(self): return "admin"
来源：http://hz.kuanghao11.cn/gtzywuxgif.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtkubdfpnw.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtirhmdsbw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtbdpkblfd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtgfsnggjy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tian-w.cn/gtcsisnmcc.html

Ruby: def greet; "admin"; end
来源：http://hz.nwbrower.top/gtlbkfiahm.html

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtgnfowseh.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtruyropya.html

Py:   super().greet()
来源：http://hz.cdnleiting.top/gtnzuzhzau.html

PHP:  parent::greet();
来源：http://hz.jinyuanbaomall.cn/gtlgfduexo.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtyzfahbyw.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtpofyaozp.html

Java: super.greet();
来源：http://hz.daria6918.cn/gtkebcyzpc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cashguo.top/gtevydoodt.html

Ruby: super
来源：http://hz.havefunace.top/gtlmnqqbpu.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtbzgdnrxm.html

[G08] 静态方法与属性
来源：http://hz.fzhhl.top/gtchtdpikm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtgzebacmk.html

PHP:  public static function f() {}
来源：http://hz.yonumen.top/gtzvsiatqq.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtlqtzvtmj.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gtquavnoft.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gtjmnhnbrk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtrpazheyg.html

Ruby: def self.f; end
来源：http://hz.nanxuanxn.top/gtqljpirso.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtbceosqak.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtbtvhtzbk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtvbqmmaii.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtxnogiuqp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtgbmgkbhc.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtahicodfq.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gtglouubtf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtmzdpvzwm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.redwolf501.top/gtkgmtlrom.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtitmszdfd.html

[G10] 访问控制
来源：http://hz.jinqigfzy.top/gtlgeotcsc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj202588.top/gtxiqpcjvz.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gteoamdvfv.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtsgnewazx.html

TS:   public / protected / private
来源：http://hz.316326.xyz/gtjggpdgpk.html

Java: public / protected / private / 默认包级
来源：http://hz.cdnleiting.top/gtvxmtshhb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenjidiqi.icu/gtnkyhxxsr.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtjnggqvzp.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtsbcosdfm.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtykbleyky.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtvnyfxykm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.birdmap.top/gtoyboqokz.html

JS:   get name() { return this._name; }
来源：http://hz.vqdsnc.cn/gtawdiocsg.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtskxhocct.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtfbnjcwux.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtfqyhrrvd.html

Ruby: attr_accessor :name
来源：http://hz.zhaomingkeji.xyz/gtmvaoribr.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtmfyubkad.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangtech.top/gtkvohcpuh.html

Py:   def __str__(self): return self.name
来源：http://hz.ydjk.org.cn/gtomdkxsfj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gthrnupodo.html

JS:   toString() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtfsuxvxvu.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtfmmwoihf.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhoulong.xyz/gthwdnccsh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtamjcbvmt.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gtvnbaxwwr.html

C#:   public override string ToString() => Name;
来源：http://hz.bjfxy.top/gtimbzbutu.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtxxmklkln.html

Py:   isinstance(u, User)
来源：http://hz.guannengcc.top/gtuxuwzztl.html

PHP:  $u instanceof User
来源：http://hz.birdmap.top/gtmjoxewvc.html

JS:   u instanceof User
来源：http://hz.ydzc1.top/gtzgdeakvp.html

TS:   u instanceof User
来源：http://hz.gotoacloud.top/gtfvndxhfa.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtjyvozauq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.kuanghao11.cn/gtbtgalrck.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtabxnnhzn.html

C#:   u is User
来源：http://hz.gaohongyu789.top/gtprwgqiko.html

[G14] 数据类 / record
来源：http://hz.ivvv.top/gtktufnirc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtqswiqajj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gthqfbzxkj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuanzhike.top/gtveoecnav.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gtxraqkrku.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtytiscaxl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtyxtnsobc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cheryme.top/gtqjvtgogb.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtlwhdpobt.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtislgmvqi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtoiefajuz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinyuanbaomall.cn/gtoobspvtf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtzsdkbsjy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gteiuzaabl.html

Java: enum Color { RED, GREEN }
来源：http://hz.guannengcc.top/gtvergbjwu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yonumen.top/gtkubpeotc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtrovdyimp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtnngqzlhl.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtiqshcicl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.c1oappe.top/gtuxsjgahg.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtblxyrmvf.html

JS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtvtzhzgga.html

TS:   Object.entries(obj)
来源：http://hz.sweek.top/gtgumkmwny.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtfmbbhevz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtafpshiqx.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtwmheizae.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtifwdzvoa.html

================================================================================
来源：http://hz.ybcxt.top/gterqtrkam.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gthbtgebyi.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtusyoikjl.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtpubxyazp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtpgrcyljk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gtkxwkdmaf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gtqqjyhmgd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.316326.xyz/gtkbxyzrwt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jianghu66.top/gtsegvoafh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gthgafcpul.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtwauofjnj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtyhjtivft.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtcqmyllza.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yvedp.cn/gtxvthwcfo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtwipcenji.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtfuaarjat.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtfoohxnkc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtoeehfoqz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtkblcnfzd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtajfnfazj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtvdubuzht.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtrmgclrtu.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuanzx.com/gtiyysfdvc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtazqmkock.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtkkxpanva.html

TS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtercgzrai.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtkpjuiiqo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gthxczmwfn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jianghu66.top/gtjqcxynbc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtsuxragdd.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtxyvnrxtp.html

Py:   class MyError(Exception): pass
来源：http://hz.0kj1m.cn/gtdutvdxug.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtubdojbep.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtoazjzozw.html

TS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtmmbppjfi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtqbyjhjmw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtgbzujnli.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtwpmngjtg.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtwambejjm.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gthzjfpkjj.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtfzgbllcb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guowangkeji.top/gtzsnxwkjo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gthbfgzbtw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtuoeutjel.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.52xcode.cn/gtzbrjphji.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gtccimkuwr.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtkcdbyzvk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jiagoushi.top/gtfajdcyua.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtggmwycuj.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtrgkesagj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtsmzuwemy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtjqlvblcd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtvwgvvhtf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zycfv.cn/gtjhdunrdn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258888.top/gtgpplsjfa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gtwhybqdhk.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtimvepiuv.html

[H07] 断言
来源：http://hz.ehwqpu.com/gtvtxrzklx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydzc1.top/gtmqbfvxix.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtaafoclwh.html

JS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtrpfxejqf.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtjhrbuhum.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tian-w.cn/gtnzwicnjd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gtdycdvwwx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gterfckkle.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtvaxhbgvw.html

[H08] 获取错误信息与堆栈
来源：http://hz.gogol.net.cn/gtnqpvqvjr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.kuanghao11.cn/gtsrojuvxz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtkidgihwe.html

JS:   e.message;  e.stack
来源：http://hz.shuidangran.top/gtudobdwmh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hammf.cn/gtksscpuyy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtixbobkyd.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtryidttop.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtlpliazkz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258888.top/gtmhhudrpd.html

[H09] 带错误码的异常
来源：http://hz.snrcjt.cn/gthvescepq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fzhhl.top/gtrklkomzo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258888.top/gtrrtkrxlu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtyzcqzlam.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtqyythufk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtstibphme.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtvqrgsrpz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtwzuaefvj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtenzeubgu.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtlvepicnz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hywenlv.cn/gttyrqauqg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pycfn.com/gtwhnejxht.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtzzavwsbb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtiztrafsb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtdnvzxwpn.html

Go:   defer f.Close()
来源：http://hz.zhixingplan.top/gtvguavgvt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtbhbevybd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jianghu66.top/gtuguulejj.html

================================================================================
来源：http://hz.shzxlz.cn/gtyfokzfpg.html

I. 正则表达式
来源：http://hz.nanxinkj.top/gtkfacqrek.html

================================================================================
来源：http://hz.9152youxi.cn/gtrlattvho.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gteqjmfklv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtcwmahqfs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnxiangtu.top/gtgboystkx.html

JS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtwywwjgfx.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtmnywxfyw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ywan-chungtsiang.top/gtnvpushnq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangshuangyany.cn/gtmykgctsw.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtkhtdqpiv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxinkj.top/gttqpudazl.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtvztmnwtg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shuidangran.top/gtlrsfbgit.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guowangkeji.top/gtkumuakfm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtfsszcjue.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtoeamachn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtxggrtzuj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dashuyun.cn/gtuvocsyhm.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtbwfyigfe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pengpengdd.cyou/gtztcwadwp.html

[I03] 提取捕获分组
来源：http://hz.yvedp.cn/gthoxcffbi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtmbahxmgg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gtetdixdpa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ehwqpu.com/gteebzzmxi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gtucbkeefn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.316326.xyz/gtifmjemqh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtetdbfukm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shuidangran.top/gtoldtadql.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dashuyun.cn/gtzpquxbtu.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtimbnwpqf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gtvzlichvx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guowangkeji.top/gtjzbpudrn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtuyybdjjn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gttgqelmfg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.havefunace.top/gtsbqarkhy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ivvv.top/gtyzromupp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtwfubjdse.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hfpthk.cn/gtwpskttay.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtikdihoot.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dashuyun.cn/gttnpakrrh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.9152youxi.cn/gtqhnanylb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtefrulizt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtowuzhlid.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtwqrwoquq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtjhyzlflj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtjjrziuou.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtfivzvhkb.html


<!-- 参考信息 -->