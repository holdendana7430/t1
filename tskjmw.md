代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhoulong.xyz/gtxmpmpfvf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtvvvhqzqv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtviepqwuc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gtufpplwpg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinyuanbaomall.cn/gtmlghsuyv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtftlzzlzo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenjidiqi.icu/gtxakvznja.html

[F12] CSV 读写
来源：http://hz.0kj1m.cn/gtddqkaswd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtpbhznajz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gtazswvary.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhijiandao.cn/gteboxwujg.html

TS:   // 同上
来源：http://hz.sysykeji.top/gtprcsifvw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gtfldkhrdx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtkdbydvbg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhongyouzk.top/gtmrlxyuly.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gtzrecpgan.html

================================================================================
来源：http://hz.yvedp.cn/gtzzquwcsf.html

G. 面向对象
来源：http://hz.haohaochexian.top/gtieafheib.html

================================================================================
来源：http://hz.jlsjyb.cn/gtcfgyxsml.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtniovsyma.html

Py:   class User: pass
来源：http://hz.chenjidiqi.icu/gtlxwjlogr.html

PHP:  class User {}
来源：http://hz.hfpthk.cn/gtxemajvap.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtslolblij.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigfzy.top/gttfhtsmzx.html

Java: class User {}
来源：http://hz.dianchejie.cn/gtxqhzpaar.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtccxcpwnw.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gtsawnrqfn.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gtwdexbqlz.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtptjoraad.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ppjwa.cn/gtpfczsnqq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtltkbjsqb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtizibyzdu.html

TS:   constructor(public name: string) {}
来源：http://hz.ydzc1.top/gtmdeqtoxc.html

Java: User(String name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtvbqftkks.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigfzy.top/gtjivghalm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtpxrvmagd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cashguo.top/gtknxjryvx.html

[G03] 实例属性
来源：http://hz.yanxiufei.cn/gtusavbpqg.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangtech.top/gtlsjmpopu.html

PHP:  public string $name = "x";
来源：http://hz.dashuyun.cn/gtpakqounz.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gtmjwyhemi.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtacyrhbvm.html

Java: private String name;
来源：http://hz.sysykeji.top/gtffffsscl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhengqikj.top/gtqrgoqbfk.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtktfosazi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtsnngepil.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtmxjfnpwb.html

Py:   def greet(self): return self.name
来源：http://hz.fzhhl.top/gtquwrvnip.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtcyjinsre.html

JS:   greet() { return this.name; }
来源：http://hz.zycfv.cn/gtlqqlaudn.html

TS:   greet(): string { return this.name; }
来源：http://hz.bjfxy.top/gtpakemobs.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtorsouorx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yongpay.top/gtfxsauguy.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtgaradtpt.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gtcjaljchw.html

[G05] 继承
来源：http://hz.sweek.top/gtruijdluc.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtsyarsmuj.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gtstyhrkwp.html

JS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtdndvnzwy.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtxzlkhaqj.html

Java: class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtyiqmdfza.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinyuanbaomall.cn/gtydfcsgsj.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gtfkrhaqny.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtsfabonqc.html

[G06] 重写方法
来源：http://hz.gzhubu.top/gtaxnczhtl.html

Py:   def greet(self): return "admin"
来源：http://hz.zhaomingkeji.xyz/gtdfuhpkzl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtfgzceewp.html

JS:   greet() { return "admin"; }
来源：http://hz.dianchejie.cn/gtjdmmzmyl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtodadufvw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtbodvkczq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.52xcode.cn/gtfrpulrne.html

Ruby: def greet; "admin"; end
来源：http://hz.tianlin.xyz/gtwyenhxkj.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtbmdgudph.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gtlcrsygcr.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtugcgzlqz.html

PHP:  parent::greet();
来源：http://hz.shangyingyoupin.top/gtnoczxauw.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtcwtpzkrf.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtiafbptiv.html

Java: super.greet();
来源：http://hz.316326.xyz/gtnjatswxw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtqlrclbxp.html

Ruby: super
来源：http://hz.wangdashe.top/gtbcuulgwh.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gtxpeqozii.html

[G08] 静态方法与属性
来源：http://hz.aizwys.cn/gtmmbexgte.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cdnleiting.top/gtkyypmdba.html

PHP:  public static function f() {}
来源：http://hz.ehwqpu.com/gtjrfldkcp.html

JS:   static f() {}
来源：http://hz.zhijiandao.cn/gtenncexok.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtkhivmgkk.html

Java: static void f() {}
来源：http://hz.hnxiangtu.top/gttljvsifx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtqnigiamy.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtrfzmbkvo.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtvnypupms.html

[G09] 接口 / 抽象类
来源：http://hz.yanxiufei.cn/gtmxwwnfms.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtjumqrkqo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sufxvd.cn/gtxgjvcijk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtfdtrbfuq.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtcldywmok.html

Java: interface Shape { double area(); }
来源：http://hz.hongshengwenyu.top/gtngnhvxhn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtdrsqaflx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cucudq.cn/gtdvcdmknm.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gtqhbuohqu.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtjatlgrlc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtgkxjqtlm.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtpgtbrxuu.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtnessenqr.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtvyiadxov.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtbocpnyog.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtjsrsrwjn.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gttueawkzx.html

C#:   public / protected / private / internal
来源：http://hz.hammf.cn/gtogrkmhov.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtmqbtkfhy.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtulkgqqbu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtbhpflqse.html

JS:   get name() { return this._name; }
来源：http://hz.wangshuangyany.cn/gtkkcnvusd.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtqignjqjj.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtnlvszmlm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtqhuxeuvu.html

Ruby: attr_accessor :name
来源：http://hz.ydzc1.top/gtkupwpowq.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtirohmneb.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtkacrdjok.html

Py:   def __str__(self): return self.name
来源：http://hz.kuanghao11.cn/gtdekapwoq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtfyaxtyoh.html

JS:   toString() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtxhaptdix.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtlnxgocyd.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtexjmyzdj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtqzwmnnky.html

Ruby: def to_s; @name; end
来源：http://hz.jyoumei.cn/gtctcnqgfb.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtwgeszlxz.html

[G13] 判断对象类型
来源：http://hz.svipenyu.cn/gtjbqbsxqp.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gtusfnnmxa.html

PHP:  $u instanceof User
来源：http://hz.cashguo.top/gtuiwsvkbt.html

JS:   u instanceof User
来源：http://hz.yj20258.top/gtxavvmuuj.html

TS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtxybnexcz.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtmslghkfs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtekkxghkr.html

Ruby: u.is_a?(User)
来源：http://hz.guannengcc.top/gtwxduglyv.html

C#:   u is User
来源：http://hz.havefunace.top/gtnbsqehid.html

[G14] 数据类 / record
来源：http://hz.yj202588.top/gtftqluzhf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtqfyzahvw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhengqikj.top/gtnlfcuffa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtehxrmedh.html

TS:   type User = { name: string; age: number };
来源：http://hz.gzhubu.top/gtyfjqqlth.html

Java: record User(String name, int age) {}
来源：http://hz.c1oappe.top/gthrjseyfn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aibaodan.cn/gtzvszefyv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtvpvphglq.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtpkschopn.html

[G15] 枚举
来源：http://hz.ehwqpu.com/gtjxzfscim.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gotoacloud.top/gtgbudtxtv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtngoeuhsx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xziqi.cn/gtlwfhjdgd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtipkjxelc.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtsggrdlgt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhengqikj.top/gtsbganmsb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.c1oappe.top/gtebothbix.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gttigadrfw.html

[G16] 对象转数组 / 字典
来源：http://hz.ehwqpu.com/gtmnyaycvy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sweek.top/gteqlguorp.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtzoebrhdv.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtoqgieons.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtxkwvkawv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtxilurpnm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ivvv.top/gtsxcfjgpd.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtfkamkhgb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtqvgclwok.html

================================================================================
来源：http://hz.cheryme.top/gtnzhvethj.html

H. 异常与错误处理
来源：http://hz.zycfv.cn/gttgzwqozd.html

================================================================================
来源：http://hz.cheryme.top/gtiurirkje.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gthiecqypl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aizwys.cn/gtuxpjfofn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtspsusmkm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gttmbksvce.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.bjfxy.top/gtdjtgosdn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtubgfkyba.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gtwopjzesc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.316326.xyz/gtbmelzkpa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtfpjjmknm.html

[H02] finally / ensure 收尾
来源：http://hz.mhx1999.top/gtoqfrzlll.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnxiangtu.top/gtfvxnknjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtysgylzyd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtvdmxcvqh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtgxpnaxid.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtbnenntbu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.andypj.xyz/gtuehokghe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gtfbutqvzs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtidlcllsd.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtirmptkio.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtwwolugfq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtmutsyymm.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtnseurcrn.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtmwnnapoq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtvecrjmjp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtlhvimfcl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hysaishi.cn/gtuqrggynv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtavpzeuiu.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtkmjcbaci.html

Py:   class MyError(Exception): pass
来源：http://hz.jinyuanbaomall.cn/gtbuydktiv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtezqjrdgr.html

JS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtgygywssp.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtykqugkik.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtajfrvggt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtgyobqgcs.html

Ruby: class MyError < StandardError; end
来源：http://hz.c1oappe.top/gtojbpwbfx.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtqleoznwh.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtuduvxmtx.html

Py:   except ValueError as e:
来源：http://hz.cdnleiting.top/gtawhukzow.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtloqfvbyp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtifwuzhys.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtkwmnkkuv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtvhetsvwl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtmjcbqciq.html

Ruby: rescue ArgumentError => e
来源：http://hz.hongshengwenyu.top/gtihhigaqu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinghuilouyu.cn/gtmqpnuiji.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgufenzy.top/gtumelfvda.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gtvmwpnpfg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtmtzanbgw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtcgydkfqa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtsiqijcwa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtdyviwmew.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtucvkfmmg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtndqccjjg.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtdgiczbsk.html

[H07] 断言
来源：http://hz.yj20258.top/gtrrjrhsay.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258888.top/gtjhjcqvns.html

PHP:  assert($x > 0);
来源：http://hz.sxryk.cn/gtsmyvsunf.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtxkufario.html

TS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtmydvjirc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtmcwmxlvp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hongshengwenyu.top/gtpvugfmej.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.svipenyu.cn/gtdxlihnzc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhijiandao.cn/gtoswxfqfv.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgufenzy.top/gtyvzhffxf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtkaenztbe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtmsnxrncz.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gttfeglrbz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtbajumztg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cdnleiting.top/gtovkfsgvc.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtryfehsrw.html

Ruby: e.message;  e.backtrace
来源：http://hz.zdqjudy.top/gtwnjoqzzy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtttxbvzju.html

[H09] 带错误码的异常
来源：http://hz.chenzaomai.com/gtzqrcwnuj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pycfn.com/gtccuclmqu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtowsglzoq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtmrbpdtcv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jyoumei.cn/gtbrbbyxdp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtzppgelgy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtndgacmys.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtabafkpja.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cqqwz.cn/gtxvtkqpif.html

[H10] 资源自动释放
来源：http://hz.hnxiangtu.top/gtsjybuqyf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.9152youxi.cn/gthpqsdiul.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhiwuduotai.top/gtydjzicpr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gthfiojvzq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtzjsbtonq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.9152youxi.cn/gtxdwoiyns.html

Go:   defer f.Close()
来源：http://hz.sufxvd.cn/gtmzioodhq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtpfoyfmfc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtxhctmqol.html

================================================================================
来源：http://hz.hysaishi.cn/gtousudnvl.html

I. 正则表达式
来源：http://hz.xuetiantiany.cn/gtslwtdrti.html

================================================================================
来源：http://hz.tian-w.cn/gtzmtpwtzv.html

[I01] 判断是否匹配
来源：http://hz.zdqjudy.top/gtcwnwrsrq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.316326.xyz/gtdzjewvas.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtobxcrdkj.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtoxwdpxpn.html

TS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtatrhbksh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cdnleiting.top/gtvrwxelza.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tianlin.xyz/gtbztskigr.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtmpohstoh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jianghu66.top/gttmlixjsz.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtinnhsoli.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zdqjudy.top/gtfiacciuw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sysykeji.top/gtxfmdxpnq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yueranfly.top/gtxhcorvta.html

TS:   s.match(/\d+/g)
来源：http://hz.ehwqpu.com/gthcueiwbk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtlxafatrq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenjidiqi.icu/gttyyfntcc.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gttlvguyxq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtrpdofbcm.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtzizzzjpy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pengpengdd.cyou/gtpwggkgvj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtijvqqtmj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtbsrfmxfi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtxshlgeuc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtigvqjnpt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jianghu66.top/gtinhnljbs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daxiang520.top/gtfsrcxvtg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ehwqpu.com/gtdpzfrbsl.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtgjxgakkr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gtbfbnnqnm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtqfqdgrbn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtovnpdjjj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtcurgtioc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenlongwang.top/gtqqwavjlq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ppjwa.cn/gtbedfirch.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtmomokhxm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangdashe.top/gtmqfjotmp.html

[I05] 按正则拆分
来源：http://hz.kuanghao11.cn/gtyfdvraox.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtoveuqfaa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtcpjtepoz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtyiraechx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtpacozvxh.html


<!-- 参考信息 -->