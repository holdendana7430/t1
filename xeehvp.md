代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtvncxsome.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.feifeiyinyue.top/gtdgezrvqo.html

Ruby: Dir.children("dir")
来源：http://hz.guannengcc.top/gtwzdxjpva.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtxdjdbfwv.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gtflxhychk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtulggabqd.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtfkwmapfn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtbshxuibf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtnwvalasq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtloidisee.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtelgnexju.html

Ruby: File.size("a.txt")
来源：http://hz.vqdsnc.cn/gtoowmdmun.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtwtbzbyuu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhiwuduotai.top/gttqxitqmg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtcgwyserm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.feifeiyinyue.top/gtxhxrdtvq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtdpnbkdsb.html

TS:   path.extname("a.txt")
来源：http://hz.haohaochexian.top/gtvbpocxlw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gthhcsoidn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtojkipphm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtqlaraszc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yangfankeji.com/gtlanzlatu.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtzstisoku.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtfpyxyaus.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinghuilouyu.cn/gtxmbjnozn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtxednjyra.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtdrpntkhj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtlpwbjnii.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jlsjyb.cn/gtkagizgno.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtotcuisjp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gtqueganjq.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtdsmsmkvb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xylfe.cn/gtopjcigpw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtkwnynspj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhijiandao.cn/gteqluuldw.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtzyznztjx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zycfv.cn/gtfbhlkigb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtcnahfivh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gtfrizdfrt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gtinppeqdu.html

================================================================================
来源：http://hz.yangfankeji.com/gtdsybjyxx.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtqvkswzqt.html

================================================================================
来源：http://hz.yj202588.top/gtueeoswms.html

[G01] 定义类
来源：http://hz.iojbl.cn/gtabxcvlup.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtoclzsoee.html

PHP:  class User {}
来源：http://hz.gzhubu.top/gtwobxhydb.html

JS:   class User {}
来源：http://hz.shanyushiyangtech.top/gtszygzsht.html

TS:   class User { name: string = ""; }
来源：http://hz.hammf.cn/gttohgiwdq.html

Java: class User {}
来源：http://hz.guannengcc.top/gtbldplvwx.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtnzisvfvq.html

Ruby: class User; end
来源：http://hz.ydjk.org.cn/gtudtwbjox.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtgjzoyyhd.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtagwwymkc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtcikswqvi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtmwvbqnxb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydzc1.top/gtgbavgcdf.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtaqxdjdtw.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtaxpabnfj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtxidskaut.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtwpnmzzcp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtplzaneza.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gtssrlvtmm.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtnqjrqfuk.html

PHP:  public string $name = "x";
来源：http://hz.tian-w.cn/gtlnngebje.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtncvgxuau.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gttfahcwuv.html

Java: private String name;
来源：http://hz.smart0.xyz/gttqhstjjv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigfzy.top/gteanqyyad.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtiinvhsus.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zdqjudy.top/gtswkhftxu.html

[G04] 定义方法
来源：http://hz.zhoulong.xyz/gtpvwcaove.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtxjubbpgd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gttqrhxyzv.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtvbomuwbv.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtfnwcdazy.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtkhwcfeub.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtyfsspxnp.html

Ruby: def greet; @name; end
来源：http://hz.bjfxy.top/gtjshyqtij.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gtwnyhfssg.html

[G05] 继承
来源：http://hz.jiagoushi.top/gtuayygncq.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gttenxporb.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtmmbsxnrm.html

JS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gteviegnpr.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtnjjoqkng.html

Java: class Admin extends User {}
来源：http://hz.hammf.cn/gteccaujsb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangkeji.top/gtdgektiae.html

Ruby: class Admin < User; end
来源：http://hz.fzhhl.top/gttxwxgqle.html

C#:   class Admin : User {}
来源：http://hz.havefunace.top/gtjltyrfyf.html

[G06] 重写方法
来源：http://hz.mhx1999.top/gtpavkuqcx.html

Py:   def greet(self): return "admin"
来源：http://hz.zhiwuduotai.top/gtngpuqjwb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtzjuktvps.html

JS:   greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtlldetpif.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtevgsofjw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtkgonumoe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtisurkzle.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtmpitywhx.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtknoeejql.html

[G07] 调用父类方法
来源：http://hz.zhengqikj.top/gtawwpjpba.html

Py:   super().greet()
来源：http://hz.hammf.cn/gtvjxuwjci.html

PHP:  parent::greet();
来源：http://hz.yj202588.top/gtdsyhmfrg.html

JS:   super.greet();
来源：http://hz.aizwys.cn/gtiuyzyjmp.html

TS:   super.greet();
来源：http://hz.quarkkingdee.top/gtixkuegby.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtykarhjou.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhongyouzk.top/gtwnrpioqq.html

Ruby: super
来源：http://hz.xylfe.cn/gtrwdnlnvv.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtrrzliual.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtnljpufgu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ivvv.top/gtnufdmace.html

PHP:  public static function f() {}
来源：http://hz.sufxvd.cn/gtuyrtxojp.html

JS:   static f() {}
来源：http://hz.hongshengwenyu.top/gtktrlwzgs.html

TS:   static f(): void {}
来源：http://hz.jqgufenzy.top/gtyvxaujql.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtynmgmwvt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtvyekjagw.html

Ruby: def self.f; end
来源：http://hz.xylfe.cn/gtyzuewzmm.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gtwusyvcuy.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtqkpubhgl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtlbmwkked.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtmuajvytj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hfpthk.cn/gtrxoquzdy.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtfwsvitjh.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gteiuowtvm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgufenzy.top/gturmwbtht.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gzhubu.top/gtqyrzgobf.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gtlmysdagc.html

[G10] 访问控制
来源：http://hz.svipenyu.cn/gtvcvrpthc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtwqnwngqh.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtuapafkrb.html

JS:   #private 字段；其余公开
来源：http://hz.sufxvd.cn/gtxlfntfhs.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtulsuzelq.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtnrgigesa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shangyingyoupin.top/gtxagpkuhp.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtuwfsplnr.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gttmhqxrkn.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtdptzrnqy.html

Py:   @property 与 @x.setter
来源：http://hz.birdmap.top/gtiluxplpu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtxfuqygvi.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gtumorrgqd.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtlhhqxbup.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gtyrdaqrby.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hfpthk.cn/gtaxjllffo.html

Ruby: attr_accessor :name
来源：http://hz.52xcode.cn/gtrluvptoj.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gtxvfsxegt.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtlwpwxxfh.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtytezwlsi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtriyrewfn.html

JS:   toString() { return this.name; }
来源：http://hz.ehwqpu.com/gthbvswzld.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtssmhakqn.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gtflixocqd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtvftmczpw.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtookuvguk.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gttydrhbbh.html

[G13] 判断对象类型
来源：http://hz.meibo888.top/gtpnmhuvwq.html

Py:   isinstance(u, User)
来源：http://hz.ydjk.org.cn/gtppfouhvo.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtznloacst.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtyoldlccx.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtpvfpxkdw.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtcuwrkauq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hongshengwenyu.top/gtqdppozwh.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258888.top/gtoiybrppj.html

C#:   u is User
来源：http://hz.52xcode.cn/gtzsvfpxcc.html

[G14] 数据类 / record
来源：http://hz.9152youxi.cn/gtrjtfkcwm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtokmvjaej.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtqgllqwuw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtpxydaohm.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtmgpqfqxv.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtspwmmyja.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtfddnghif.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtbmqjbrim.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtfnaiwrsd.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gttzgxpzyl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtqkitylnl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtljsuiqxu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtcnnhgpyj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gterwfxhvc.html

Java: enum Color { RED, GREEN }
来源：http://hz.sysykeji.top/gtmsjtuqfr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtwqjnotkz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtvdbulggs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtqxhyovhm.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtkraoqbti.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pycfn.com/gtbrjyzevc.html

PHP:  get_object_vars($obj);
来源：http://hz.daria6918.cn/gtjkprwrqt.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtelmpwnyg.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtmldzzlqb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gttaowowdb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ybcxt.top/gtbfizgcug.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtscwuzqpm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtfjpqfqfm.html

================================================================================
来源：http://hz.cheryme.top/gtebblfitv.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtgwdwqjzx.html

================================================================================
来源：http://hz.jinqigfzy.top/gtmqoysosw.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gtzqnlxwlp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cheryme.top/gtxbtkrstm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangdashe.top/gtimoaaynr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtohmorbvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtoawcwlvk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nwbrower.top/gtcwxmxkqj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gthymyaxcg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenjidiqi.icu/gtbqnhcjjk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gteesankqe.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gtvwvnznea.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtaeqjygps.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtwtbpdrqb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtmozeigqb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gttvaukysv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtwwnfcihg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gtnhmdgafa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gtrnizfumo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.vqdsnc.cn/gtvnylvogg.html

[H03] 主动抛出异常
来源：http://hz.hongshengwenyu.top/gtvregwqiw.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtrymhbwqx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtdkoymhmm.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtrcnaeiok.html

TS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gthjbyyakl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gttnosntqi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gttdbcihnd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shangyingyoupin.top/gtwadpijis.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtojqylnbr.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtfnnyvdlb.html

Py:   class MyError(Exception): pass
来源：http://hz.fengsongda.top/gtzjuftjmz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtzmemblqz.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gthrphldje.html

TS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gthxunarqp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtdqkwibvd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtromjyejp.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gthzpeebit.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtudrbeghk.html

[H05] 捕获特定类型
来源：http://hz.nanxuanxn.top/gtujefxdby.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtlayhbqme.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xingfuxueyuan.xyz/gtkmfhoktj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtuklnwjys.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtourehpeq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtfekmafee.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtrzwlujjv.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtokzqeggo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yonumen.top/gtrgkwpjeb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgfzy.top/gtprlkaray.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtrgqcuxod.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sweek.top/gtwlditcxy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gteuwaqdqt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtarsudynz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtetfpzaiw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tian-w.cn/gtjzeqwyqe.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtwxiqqmcy.html

C#:   obj?.A?.B ?? default
来源：http://hz.sweek.top/gtbsapnsxp.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtcmtcslla.html

Py:   assert x > 0, "必须为正"
来源：http://hz.haohaochexian.top/gtzwtbffsr.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtwiwikinn.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gthrykxchj.html

TS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtwpdzywsa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtqtctiagy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.iojbl.cn/gtwercccod.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gtkjawpppj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtelvttgub.html

[H08] 获取错误信息与堆栈
来源：http://hz.xylfe.cn/gtkjujbpjm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnqzz.top/gtrmzqnrkh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.smart0.xyz/gtbffnsjaa.html

JS:   e.message;  e.stack
来源：http://hz.jianghu66.top/gthzjjxted.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hfpthk.cn/gtjzaizstj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtmoudcyol.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtkpgfhwxh.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gtfyzuetmf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gtgnpaoqjj.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gtyypqsduc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtxotxkues.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtctxkzmow.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gtnvgglctd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tanke756.top/gtjqxlsegx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gtuonkrtap.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtunvwipnn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dianchejie.cn/gtyuohiplb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhijiandao.cn/gtvyjtsrkq.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtzurwffed.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gtkcviiycd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jyoumei.cn/gtkxrazmqc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gttljhpalc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtynxjemel.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtffzzgova.html

Go:   defer f.Close()
来源：http://hz.cucudq.cn/gthoqqjosm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.bjfxy.top/gtxuxjpngj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258888.top/gtaqlofedy.html

================================================================================
来源：http://hz.wangdashe.top/gtlbmslpqg.html

I. 正则表达式
来源：http://hz.shzxlz.cn/gtesvhlkxo.html

================================================================================
来源：http://hz.zhixingplan.top/gtbwscensm.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtgggtlyiy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtlsstbgov.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cashguo.top/gtmcyqepsb.html

JS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtbrxacrvx.html

TS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtlbigqwfe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gttoniwhkh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dashuyun.cn/gtkefkvzrx.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtdumedtfp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtyjuyyeah.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gttjbzrsnu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guannengcc.top/gtvmyfagxu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtcwgduesu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.snrcjt.cn/gtjpzqraoz.html

TS:   s.match(/\d+/g)
来源：http://hz.gogol.net.cn/gtksvkmcjp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jyoumei.cn/gtvqzxtlke.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhengqikj.top/gtasozplal.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtbcgsvzyy.html


<!-- 参考信息 -->