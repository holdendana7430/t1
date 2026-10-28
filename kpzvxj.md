代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xziqi.cn/gtautzarhr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtzzbsiitf.html

Ruby: Dir.children("dir")
来源：http://hz.shuidangran.top/gtayzmveny.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtepiycjrq.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtdhvydqvf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.iojbl.cn/gtsdcekcth.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtckvjbtop.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtqnimpweg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gteyojudlk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gttclclboj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nwbrower.top/gtzatyysgc.html

Ruby: File.size("a.txt")
来源：http://hz.shangyingyoupin.top/gtxijypfos.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xziqi.cn/gtkdeppqvt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtijarcrnj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtcyaonjrk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yangfankeji.com/gtetxvqopx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtioqsuuqt.html

TS:   path.extname("a.txt")
来源：http://hz.redwolf501.top/gtvmyyoyor.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fengsongda.top/gtzrzuwbsi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gthwjxedag.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtrpljfbtn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zdqjudy.top/gthoskbetu.html

[F11] 复制与移动文件
来源：http://hz.hammf.cn/gtnabkoikg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtenwlqcwy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangkeji.top/gtrzxjdgcg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtvmjkpokc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtcgznojdu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuanzx.com/gtjyqsuqvh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtmkemrwnq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtrbzmecoo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gtxxdvpwnx.html

[F12] CSV 读写
来源：http://hz.chenjidiqi.icu/gtrfhxstvr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gaohongyu789.top/gtxmhwwpur.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtxdvisymw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yanxiufei.cn/gtaqtxyefx.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtmaeysuyb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtscnsgovm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zdqjudy.top/gtqbsxyzjq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yvedp.cn/gtvvonmcnz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtezcvakoc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtrasvazwl.html

G. 面向对象
来源：http://hz.pengpengdd.cyou/gtjpbbiqtb.html

================================================================================
来源：http://hz.jqgfzy.top/gtkwipkmmt.html

[G01] 定义类
来源：http://hz.xuanzx.com/gtzfmcceho.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtysmrfcem.html

PHP:  class User {}
来源：http://hz.yangfankeji.com/gtpnrhezws.html

JS:   class User {}
来源：http://hz.hongshengwenyu.top/gtwhfuhxoz.html

TS:   class User { name: string = ""; }
来源：http://hz.hfpthk.cn/gtthmroziv.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtklvbdwdl.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtanqbhhex.html

Ruby: class User; end
来源：http://hz.c1oappe.top/gtqwcouade.html

C#:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtvggqyhdb.html

[G02] 构造函数
来源：http://hz.snrcjt.cn/gtmjoysggt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tian-w.cn/gtcrapotdl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtjlpzhsza.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtijaqjxmb.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtsqounzvg.html

Java: User(String name) { this.name = name; }
来源：http://hz.xinyue.icu/gtkinthrro.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnxiangtu.top/gtncagljim.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtlzvgukeg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.bjfxy.top/gttvsgcixl.html

[G03] 实例属性
来源：http://hz.nwbrower.top/gtecfifnyv.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtqpvoalsz.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gtdjyxzsoo.html

JS:   this.name = "x";
来源：http://hz.haohaochexian.top/gtnnyooqlx.html

TS:   name: string = "x";
来源：http://hz.nanxuanxn.top/gtwujqwsgt.html

Java: private String name;
来源：http://hz.wangdashe.top/gtcilnxymy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jiagoushi.top/gtqwdydayt.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangtech.top/gtvlqpucng.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cucudq.cn/gtbpgwrrrq.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtatbqpajk.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtcptvysod.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cashguo.top/gtbfmfwnng.html

JS:   greet() { return this.name; }
来源：http://hz.haohaochexian.top/gthqadvjox.html

TS:   greet(): string { return this.name; }
来源：http://hz.guannengcc.top/gtkdnnqmsf.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gteenyvgfo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtkumwpixm.html

Ruby: def greet; @name; end
来源：http://hz.snrcjt.cn/gtcgfaaera.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtgsvrpxzw.html

[G05] 继承
来源：http://hz.tianlin.xyz/gtsjfshoyt.html

Py:   class Admin(User): pass
来源：http://hz.snrcjt.cn/gtuzmnbtzo.html

PHP:  class Admin extends User {}
来源：http://hz.zycfv.cn/gtbgbnoovg.html

JS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtxwfgiuhu.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtvslozumz.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gtmvsoimuw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gthsyaklru.html

Ruby: class Admin < User; end
来源：http://hz.nanxuanxn.top/gtbmoopnmp.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtxfiienwz.html

[G06] 重写方法
来源：http://hz.zhongyouzk.top/gtdcaydfta.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtrrclotoy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtnxxtkayl.html

JS:   greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtccsdimbh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtlkkbeupv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtxjxoyaqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtarynibqc.html

Ruby: def greet; "admin"; end
来源：http://hz.zhengqikj.top/gtimkshden.html

C#:   public override string Greet() => "admin";
来源：http://hz.gotoacloud.top/gtorzfvwsz.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtconiodsv.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gtbywbiqql.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangkeji.top/gtczzktpqe.html

JS:   super.greet();
来源：http://hz.yueranfly.top/gtazvhbfic.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtzpnjiveu.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtsvpuznnq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cheryme.top/gtwvqpqrnd.html

Ruby: super
来源：http://hz.yuanzhike.top/gtkjxjcrli.html

C#:   base.Greet();
来源：http://hz.yonumen.top/gtmqxjxhky.html

[G08] 静态方法与属性
来源：http://hz.gogol.net.cn/gterrmcqeh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtlpnbseaf.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtodwgwhzm.html

JS:   static f() {}
来源：http://hz.guannengcc.top/gtxfoczpdb.html

TS:   static f(): void {}
来源：http://hz.mhx1999.top/gtiwmmlugf.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gtdhqykzci.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtztbsyauw.html

Ruby: def self.f; end
来源：http://hz.yj20258888.top/gtkssvzsqb.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtmvaamlca.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtxfakhiqg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtilzqwrge.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtgtivwexh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangtech.top/gtwbhqdncx.html

TS:   interface Shape { area(): number; }
来源：http://hz.shuidangran.top/gtrsalqzqb.html

Java: interface Shape { double area(); }
来源：http://hz.ybcxt.top/gtezgmtdoy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtyaqagzkq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtqxhubhtr.html

C#:   interface IShape { double Area(); }
来源：http://hz.gzhubu.top/gtktajeiby.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtbpthdlma.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.feifeiyinyue.top/gtpullcyuc.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtwzpdkcgr.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtczsghefk.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtninulyzf.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtexklhpnb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sufxvd.cn/gtliqvtbfw.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gtgytjndsc.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gtdghhnsvk.html

[G11] getter / setter
来源：http://hz.nanxinkj.top/gtpddwpwyl.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtyqejsxhw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtwncnffya.html

JS:   get name() { return this._name; }
来源：http://hz.yj20258.top/gtxgriwukr.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gtpaycymns.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtqwulnbjt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtsaloksnj.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtbvkyxwmt.html

C#:   public string Name { get; set; }
来源：http://hz.tianlin.xyz/gttcluliwy.html

[G12] 对象转字符串
来源：http://hz.52xcode.cn/gtwuummhfh.html

Py:   def __str__(self): return self.name
来源：http://hz.pycfn.com/gtjerxecqd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtgieaxnrk.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtsivmqhnz.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtivblfdrs.html

Java: @Override public String toString() { return name; }
来源：http://hz.birdmap.top/gtfmbbkmwp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtwbgnbbxm.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangkeji.top/gtfldtwzop.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgufenzy.top/gtocqxwnzj.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtxngmdsgi.html

Py:   isinstance(u, User)
来源：http://hz.nwbrower.top/gtvbvsgcpc.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtetvxiaqh.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtgysyttqs.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtesygsxse.html

Java: u instanceof User
来源：http://hz.hnxiangtu.top/gttauxzmdq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtnxecodph.html

Ruby: u.is_a?(User)
来源：http://hz.xuetiantiany.cn/gtiftxkwpg.html

C#:   u is User
来源：http://hz.yj20258.top/gtjdxibjrj.html

[G14] 数据类 / record
来源：http://hz.zhengqikj.top/gtpqyagodd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jlsjyb.cn/gtjckpnxux.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dashuyun.cn/gtruzoszpe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuanzhike.top/gtiyesqdxr.html

TS:   type User = { name: string; age: number };
来源：http://hz.ybcxt.top/gtvqygmuvf.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtbetbgefs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydzc1.top/gtycrpnwbg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtvjjwohoa.html

C#:   record User(string Name, int Age);
来源：http://hz.yanxiufei.cn/gtteftdkuw.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtkxqanzcs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtjmlnqmxt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gthpthjorw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtgqladsqu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtacsvvpzn.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangshuangyany.cn/gtixdtqrgy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhengqikj.top/gthmvshiub.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yueranfly.top/gtumwkpwzr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gttjczogje.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gtfcikohhq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zdqjudy.top/gttohquxwa.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gtcfljshjw.html

JS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtryzandqr.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtauxonegj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.daria6918.cn/gtcotzmgmj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhongyouzk.top/gtnlcluysk.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtwyjxakiq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtjzzipnjd.html

================================================================================
来源：http://hz.aibaodan.cn/gtltypvszt.html

H. 异常与错误处理
来源：http://hz.ppjwa.cn/gtjpzoqkxr.html

================================================================================
来源：http://hz.xylfe.cn/gtyrqjtyvo.html

[H01] try / catch 基础
来源：http://hz.shuidangran.top/gtswbocnzj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tian-w.cn/gtdpcitoro.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigufen.top/gtsbwjwmav.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtncvdkzgn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ivvv.top/gtncdqauhk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yanxiufei.cn/gtridlrdfu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tianlin.xyz/gtoqukhvdq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtyhwlzoln.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtzhveltoz.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtfzzysckq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gthgekfwmy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtjmzqjrpf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtvxirfffv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtjduhpikv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtrdpvbljq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtuedwhgpc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtdzxlecyt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ivvv.top/gtuojlxqvc.html

[H03] 主动抛出异常
来源：http://hz.jinqigufen.top/gtusucsaaj.html

Py:   raise ValueError("错误信息")
来源：http://hz.gzhubu.top/gtayqwdcpy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtpcgnodml.html

JS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtnzehzlvj.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtqhexuere.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtlfsqozzc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuxming.cn/gtwrthstoi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtfahjymqd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtxhihefzf.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtdkegmeof.html

Py:   class MyError(Exception): pass
来源：http://hz.meibo888.top/gtuvzuwccu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtxzrtawcm.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtvbpfodzx.html

TS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtvkhlidnt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtxykjtnqn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtizsmgsim.html

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtvixxioyv.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gttktqkqbl.html

[H05] 捕获特定类型
来源：http://hz.sweek.top/gtbiawgvub.html

Py:   except ValueError as e:
来源：http://hz.smart0.xyz/gtelewjpdw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtvznjqova.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtkxzgfnye.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtopnnhsmy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yueranfly.top/gtwuxtfbvi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.svipenyu.cn/gtmetmcwys.html

Ruby: rescue ArgumentError => e
来源：http://hz.sufxvd.cn/gtdfayhccg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gttpqlzlrs.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xinyue.icu/gtmcuthobs.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigfzy.top/gtwuqmpwjc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtmpkstfjv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtxwrrxwua.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtjrvqfehe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtzjdveisi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj202588.top/gtbzagxypt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sxryk.cn/gtwthjwllm.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtcvamtuho.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtvszvdwjo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtddafmizs.html

PHP:  assert($x > 0);
来源：http://hz.nanxuanxn.top/gtafklhqdf.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtnbpjljph.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtoixpkxcd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtodqgxfhf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.birdmap.top/gtnvdqzhyo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtvjgzsbwc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gtzxgdxtbf.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinyuanbaomall.cn/gtbewabtwb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtcbjjtzhz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtehoryvha.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtifqrbfry.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aibaodan.cn/gtehqywnmk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtpundhljv.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtfabyjhxe.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gthbcsvnca.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtuxcvsvxr.html

[H09] 带错误码的异常
来源：http://hz.jianghu66.top/gtgctvlzlq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jlsjyb.cn/gtbhotymrd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.haohaochexian.top/gtcstkyeif.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydjk.org.cn/gtbjclwdlg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtcygaidxh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sysykeji.top/gtbipxrimv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangkeji.top/gtpyecjdph.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shzxlz.cn/gtjmhwsbjy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtghradzzk.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gtsmlkbzsf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gtrbnctxcs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtcnugojmk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtelascnmj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtblnjvhcg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtjbppyyie.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtgdhkdieq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gteaaydpaq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gtyuhcgbyd.html

================================================================================
来源：http://hz.kuanghao11.cn/gteceyapnd.html

I. 正则表达式
来源：http://hz.hywenlv.cn/gtnntgtflh.html

================================================================================
来源：http://hz.shzxlz.cn/gtqwwmuzki.html

[I01] 判断是否匹配
来源：http://hz.birdmap.top/gtsoehvgep.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtkzyawygu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hysaishi.cn/gtaqfwixzw.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gteqwjmhoj.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtmnaxdlmj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xylfe.cn/gtcdbgfwqe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtlczmdnos.html

Ruby: s.match?(/\d+/)
来源：http://hz.bjfxy.top/gtpzhfpguw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gtmbngqaff.html

[I02] 提取所有匹配
来源：http://hz.nanxuanxn.top/gtcgtukacn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jianghu66.top/gtiwmlxvrc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtjatuadgd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guowangkeji.top/gtgvbzpmrz.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtjydkwehn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.9152youxi.cn/gtvwqcfpkm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtdhkkiyjm.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydjk.org.cn/gtuilrrffw.html


<!-- 参考信息 -->