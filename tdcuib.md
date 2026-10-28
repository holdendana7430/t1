代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.dianchejie.cn/gtwyzdosks.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtjjnpyhti.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gthvwibdgg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuxming.cn/gtfqjkfxjf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtfimzcxdv.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258888.top/gtdmxwymvf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gtpjlvrvfb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtqggplcys.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtmmlasemr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gttnjbghdl.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gthkcfrngx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtomtmroqv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxinkj.top/gtvpvgawhc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtcgxbfcwa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtqbxqcepc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtolqmtchq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hysaishi.cn/gtwtjlnxcb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtidegwrzx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.snrcjt.cn/gtmwgbccey.html

[F12] CSV 读写
来源：http://hz.zhengqikj.top/gtzfltzter.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtldmppmvz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtmkovvyqu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gtdirkncuq.html

TS:   // 同上
来源：http://hz.xziqi.cn/gteyexhhfe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tian-w.cn/gtkmbeqefo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gtcospjtif.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aibaodan.cn/gtuxpxfizf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shangyingyoupin.top/gtrasrdoic.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlzjirhko.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtgynlmvpn.html

================================================================================
来源：http://hz.birdmap.top/gtzirvocnf.html

[G01] 定义类
来源：http://hz.guannengcc.top/gtmspgjbxi.html

Py:   class User: pass
来源：http://hz.dianchejie.cn/gtsptrkpct.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtnywnikhh.html

JS:   class User {}
来源：http://hz.cqqwz.cn/gtopmcijwr.html

TS:   class User { name: string = ""; }
来源：http://hz.daria6918.cn/gtaatasnkt.html

Java: class User {}
来源：http://hz.redwolf501.top/gtxohcufus.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtfspsujcm.html

Ruby: class User; end
来源：http://hz.aibaodan.cn/gtmmsdichp.html

C#:   class User {}
来源：http://hz.yonumen.top/gtfeepohyf.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gthqfbyjdx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gtlcdykrlz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtopeyvauy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtyfaexwji.html

TS:   constructor(public name: string) {}
来源：http://hz.sysykeji.top/gtzblxsrsw.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtzvjtkgdp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtzpwnkgzh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ywan-chungtsiang.top/gtiofhtemr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtpacatxlt.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gtqdanfvgg.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gttbxvosnz.html

PHP:  public string $name = "x";
来源：http://hz.hysaishi.cn/gttzsisqra.html

JS:   this.name = "x";
来源：http://hz.sufxvd.cn/gtnovramoh.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtczxglikq.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtfxshjrzc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gtiwynmekp.html

Ruby: @name = "x"
来源：http://hz.jinyuanbaomall.cn/gtclzuxocd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hywenlv.cn/gtuurblyzp.html

[G04] 定义方法
来源：http://hz.zycfv.cn/gtpgblmcic.html

Py:   def greet(self): return self.name
来源：http://hz.kuanghao11.cn/gtlnrfakkc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtsvycuvwi.html

JS:   greet() { return this.name; }
来源：http://hz.dashuyun.cn/gtejnazdkw.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtgodofwiw.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gtnodmnntm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.c1oappe.top/gtobhfetsn.html

Ruby: def greet; @name; end
来源：http://hz.ydzc1.top/gtiiajymhq.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gtsexdpodt.html

[G05] 继承
来源：http://hz.0kj1m.cn/gtdjdwgqcu.html

Py:   class Admin(User): pass
来源：http://hz.sufxvd.cn/gtomdpegyx.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtkbwsqtad.html

JS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtkmphxjiv.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtjsyjbrxt.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtogxxmfsi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ehwqpu.com/gtcbeqvjxv.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtmjlgbpmp.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtasoaztgj.html

[G06] 重写方法
来源：http://hz.shuidangran.top/gtmxxehcey.html

Py:   def greet(self): return "admin"
来源：http://hz.yongpay.top/gtrzhvepfb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtqecpfvwg.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtanhqdrgn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtpecoqswv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtehxklwdw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtyuiwslnn.html

Ruby: def greet; "admin"; end
来源：http://hz.xuetiantiany.cn/gthzxhhjua.html

C#:   public override string Greet() => "admin";
来源：http://hz.sxryk.cn/gtwwysupdn.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtibznrkqu.html

Py:   super().greet()
来源：http://hz.yueranfly.top/gtnritfkbj.html

PHP:  parent::greet();
来源：http://hz.shangyingyoupin.top/gttdrsydnh.html

JS:   super.greet();
来源：http://hz.hnqzz.top/gtthqngvwx.html

TS:   super.greet();
来源：http://hz.havefunace.top/gtobxqqizd.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gtkbhqepkp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtgyjvkbwq.html

Ruby: super
来源：http://hz.hnxiangtu.top/gtacnwzjju.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtalhqmwoj.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtfbsoypjn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtqkzllehu.html

PHP:  public static function f() {}
来源：http://hz.daxiang520.top/gtfeibbusu.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtkhqnkawx.html

TS:   static f(): void {}
来源：http://hz.haohaochexian.top/gtdjjxcmzi.html

Java: static void f() {}
来源：http://hz.birdmap.top/gtabweuevc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtlwvscfya.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtadhptdqt.html

C#:   public static void F() {}
来源：http://hz.chenlongwang.top/gtztfwkxwr.html

[G09] 接口 / 抽象类
来源：http://hz.jyoumei.cn/gtkfvvlvtz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fengsongda.top/gtefrfzvzz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xylfe.cn/gtiqsaxxyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gtpwevyvdj.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtxwtnpias.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangtech.top/gtssjvlzos.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtvvzrimsv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shangyingyoupin.top/gtxudstctj.html

C#:   interface IShape { double Area(); }
来源：http://hz.sxryk.cn/gtqdrghaca.html

[G10] 访问控制
来源：http://hz.xingfuxueyuan.xyz/gtezhndjcs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtrasrrbip.html

PHP:  public / protected / private
来源：http://hz.jyoumei.cn/gtrpxkcwze.html

JS:   #private 字段；其余公开
来源：http://hz.quarkkingdee.top/gtfsyrkfme.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gttumpirag.html

Java: public / protected / private / 默认包级
来源：http://hz.ydjk.org.cn/gtzgqoxjhz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gtjhirbkwk.html

Ruby: public / protected / private
来源：http://hz.yanxiufei.cn/gtckkeiwal.html

C#:   public / protected / private / internal
来源：http://hz.jinghuilouyu.cn/gtilenzgee.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtslawchfj.html

Py:   @property 与 @x.setter
来源：http://hz.yueranfly.top/gtuvqwkxud.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtxtzznklf.html

JS:   get name() { return this._name; }
来源：http://hz.zhijiandao.cn/gtnrxmiqqq.html

TS:   get name(): string { return this._name; }
来源：http://hz.yangfankeji.com/gtwjckwqbs.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gttknfpkha.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.redwolf501.top/gtumkbjxgl.html

Ruby: attr_accessor :name
来源：http://hz.yj20258888.top/gtgtroewrq.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtnmfyigcz.html

[G12] 对象转字符串
来源：http://hz.nwbrower.top/gtlaqwnema.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gtuedtisbf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtmdasokzy.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtjogonnlm.html

TS:   toString(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtnitjlgji.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxuanxn.top/gtxizwmgbc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtqamggffe.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtjlnlfwrc.html

C#:   public override string ToString() => Name;
来源：http://hz.zycfv.cn/gtwcznhsnu.html

[G13] 判断对象类型
来源：http://hz.cheryme.top/gtbohgcnxr.html

Py:   isinstance(u, User)
来源：http://hz.kuanghao11.cn/gtwjhmtfkd.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gttlgdyxrh.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gthgcjxfwn.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtlrrhrpwb.html

Java: u instanceof User
来源：http://hz.redwolf501.top/gtlonodhmq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtjxxkehzj.html

Ruby: u.is_a?(User)
来源：http://hz.svipenyu.cn/gtgrwygjwg.html

C#:   u is User
来源：http://hz.zycfv.cn/gtjanqfwok.html

[G14] 数据类 / record
来源：http://hz.jqgfzy.top/gtdjskzovt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yanxiufei.cn/gtdvqlbwan.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gtajtwvfci.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnxiangtu.top/gtluvlfebo.html

TS:   type User = { name: string; age: number };
来源：http://hz.kuanghao11.cn/gtrtwolktk.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtrhegdukq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhijiandao.cn/gtedvjmtod.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gtdazaaygi.html

C#:   record User(string Name, int Age);
来源：http://hz.jlsjyb.cn/gtqahdybvv.html

[G15] 枚举
来源：http://hz.xinyue.icu/gtdqogrrdx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jianghu66.top/gtahrjmqdz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gtdagovzky.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gtbgekehvu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtronhpdqs.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gtqjyzvtiq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xingfuxueyuan.xyz/gtgelgnuws.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtnwskeysp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtdaenvdyu.html

[G16] 对象转数组 / 字典
来源：http://hz.yanxiufei.cn/gtwbnajlft.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.52xcode.cn/gtuohyoryf.html

PHP:  get_object_vars($obj);
来源：http://hz.shuidangran.top/gtovvlerho.html

JS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtvycfjxhe.html

TS:   Object.entries(obj)
来源：http://hz.yuanzhike.top/gtlqafdtnb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtaqnfxnai.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gtorhwesku.html

Ruby: obj.instance_variables
来源：http://hz.hammf.cn/gtoagoznaj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gtxdoawlev.html

================================================================================
来源：http://hz.sufxvd.cn/gtwhrbnkvm.html

H. 异常与错误处理
来源：http://hz.yueranfly.top/gtfgwoubkb.html

================================================================================
来源：http://hz.birdmap.top/gtcagvbwvv.html

[H01] try / catch 基础
来源：http://hz.yonumen.top/gtwcjholqa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj20258.top/gtsjsjfuik.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtpzfdxawm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gteycaoboq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtqbptluim.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yuxming.cn/gtzlgbpojz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.smart0.xyz/gtotamjwin.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.bjfxy.top/gtubezxepo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtcnjzcopb.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigufen.top/gtfbeuolfu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gzhubu.top/gtovwvhkcd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtsaepethy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtqqetyxyp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtuvgdxnyg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtietxmbwt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtntaobdic.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtsmtkrrnv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gtydicvabc.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gtvjjsdwwv.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtxzdolbfn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtvrilfwve.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtqmjzbske.html

TS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtakrmjldh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtpuyihhws.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtgvaxzthy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtzufbxkzu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtqpkofvzp.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtihbnzgjk.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtqugfgqji.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtcaqkzqrn.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtuyjfspcw.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gthuepbmyc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gttykobqse.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtyywbbzmr.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtnbrvlsay.html

C#:   class MyException : Exception {}
来源：http://hz.chenlongwang.top/gtojbenqjg.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtduydvtxj.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gthcqnhath.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sweek.top/gtljxerlde.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtmetwfjlp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtnuuhauqp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shuidangran.top/gtrepwcaty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ppjwa.cn/gtcshacudp.html

Ruby: rescue ArgumentError => e
来源：http://hz.tian-w.cn/gthmytwvlg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xylfe.cn/gtftrcowlo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuanzhike.top/gtipbqzqqc.html

Py:   value = d.get("k") or default
来源：http://hz.hongshengwenyu.top/gtspzvzear.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtyfmbpzet.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtcfllrbay.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gthxvzbmsc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.havefunace.top/gtrxzxdaqw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtcjzelosc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangshuangyany.cn/gtwjkkgrpj.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtcyjumrfx.html

[H07] 断言
来源：http://hz.yuxming.cn/gtpzbmxvub.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhijiandao.cn/gtsjjkpknv.html

PHP:  assert($x > 0);
来源：http://hz.yj20258888.top/gtjybrejdg.html

JS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gtbgwacvcc.html

TS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtkbpmdese.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtbmxczumk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtrgbrpeld.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dianchejie.cn/gtpkkrnmsj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yanxiufei.cn/gthpwwsycm.html

[H08] 获取错误信息与堆栈
来源：http://hz.tianlin.xyz/gttkxxorcx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtsmdjputj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnxiangtu.top/gtkughjdgj.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gtgjfsdrke.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtoktppivk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtabuamwim.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtgxvnzpps.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhixingplan.top/gtzujtoukd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhijiandao.cn/gtlahgdzif.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtgyprzxmm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.feifeiyinyue.top/gtbflirlgt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtqsxlizjk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtynnzhfsj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.birdmap.top/gtfcnzeooz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtvbfpmdki.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hywenlv.cn/gtbyljitlf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangdashe.top/gtopcmmvzc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxinkj.top/gtmvdipgpx.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtcqlmbagu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tanke756.top/gtrsurcgiz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnqzz.top/gtgcvjlazc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtqdptyzix.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtssemmyxw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.iojbl.cn/gtklukznjx.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtplbjnyrn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.quarkkingdee.top/gtyfjqwxmb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gthnpyfofx.html

================================================================================
来源：http://hz.hfpthk.cn/gtwrabpaok.html

I. 正则表达式
来源：http://hz.xuanzx.com/gtgkitqgni.html

================================================================================
来源：http://hz.jyoumei.cn/gtpresykjf.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gthmnvrzst.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gtbxxbrrdk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtviketbyk.html

JS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtjefnppnc.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtqrfiuolt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xingfuxueyuan.xyz/gtlsehlkwp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtnhimtvtg.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnqzz.top/gtqwqkpcwp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gtraudxfee.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gtslvwwpht.html

Py:   re.findall(r"\d+", s)
来源：http://hz.birdmap.top/gtglvgrqlr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtbhanpcgg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gtudwncmiw.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtdcvwdbvu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtljntkcet.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtcvegprlk.html

Ruby: s.scan(/\d+/)
来源：http://hz.hfpthk.cn/gtfiolyvve.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guannengcc.top/gtfualistz.html

[I03] 提取捕获分组
来源：http://hz.yangfankeji.com/gtmelsxyjs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtyhmvuowy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cdnleiting.top/gtytrktbca.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtkdxyyrak.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yongpay.top/gtrpndymfb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sweek.top/gtogznwwsp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yueranfly.top/gtdefqgqec.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtprpndlyl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinghuilouyu.cn/gtnlwxrxxh.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gtddgogxqw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangkeji.top/gtowwfnbqt.html


<!-- 参考信息 -->