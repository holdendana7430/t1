代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hysaishi.cn/gtdzijsiqg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtnjwrqozv.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtykclqffz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtacreggni.html

[F09] 获取文件大小
来源：http://hz.yuanzhike.top/gtexoolenm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gteghjetmf.html

PHP:  filesize("a.txt");
来源：http://hz.nanxinkj.top/gtyrtzvczu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtglkckchn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtmzvhgeyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtujwtdjsz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gotoacloud.top/gtcconrdho.html

Ruby: File.size("a.txt")
来源：http://hz.ybcxt.top/gtbiwhditv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenlongwang.top/gthbovgubd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zycfv.cn/gtiyzllhky.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtrgciehkq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhiwuduotai.top/gtlugbzihn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtascniuaa.html

TS:   path.extname("a.txt")
来源：http://hz.yueranfly.top/gtrbcpgxqa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtbmlypyum.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtawgljupo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtxadchuey.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yonumen.top/gtbmktmlxd.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtngwfdwiy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtpjyypcmk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jianghu66.top/gtwjwrdtrb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtrdqrirha.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtobvymekh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xinyue.icu/gthdildnil.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtxjsqzeau.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtxiuefupn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gtaclihucv.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gtzphfkjsy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gogol.net.cn/gtjrjaorvv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yanxiufei.cn/gtrkbprerq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hnxiangtu.top/gtvvxvimst.html

TS:   // 同上
来源：http://hz.shuidangran.top/gtosdgvukj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtonnddwzf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.smart0.xyz/gtevjihzlx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.kuanghao11.cn/gtasjlejjm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangkeji.top/gtdesufjqk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlrjburcn.html

G. 面向对象
来源：http://hz.sxryk.cn/gttrjtwlvb.html

================================================================================
来源：http://hz.tianlin.xyz/gtywxuless.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtqolzbxsp.html

Py:   class User: pass
来源：http://hz.0kj1m.cn/gtufoicvqa.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtetcsjdyb.html

JS:   class User {}
来源：http://hz.xuanzx.com/gtwvivddlh.html

TS:   class User { name: string = ""; }
来源：http://hz.ydzc1.top/gtquxiuacd.html

Java: class User {}
来源：http://hz.jinghuilouyu.cn/gtcssoijmm.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtkkrxvhja.html

Ruby: class User; end
来源：http://hz.feifeiyinyue.top/gtnqleirkl.html

C#:   class User {}
来源：http://hz.yj202588.top/gtbbaqjfjf.html

[G02] 构造函数
来源：http://hz.smart0.xyz/gtlrqxtcvv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.svipenyu.cn/gtluwoitty.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sufxvd.cn/gtspxdcuvk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.haohaochexian.top/gtddpwpvei.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtdfqxumrz.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gtxhuroxpi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhongyouzk.top/gtlgdwztlk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhixingplan.top/gtffjmjtys.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtmrlsszbc.html

[G03] 实例属性
来源：http://hz.quarkkingdee.top/gtegoyrxgi.html

Py:   self.name = "x"
来源：http://hz.cucudq.cn/gtluubruqd.html

PHP:  public string $name = "x";
来源：http://hz.wangshuangyany.cn/gtwpbeswxh.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gtvbaugujo.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gtjsfkvzey.html

Java: private String name;
来源：http://hz.daxiang520.top/gtcdacaenr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtcqwnkzev.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtgdvxvuvq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtnngsrkgd.html

[G04] 定义方法
来源：http://hz.yanxiufei.cn/gtsfbgezxb.html

Py:   def greet(self): return self.name
来源：http://hz.yuxming.cn/gtxctzgbvg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtyyrjamzj.html

JS:   greet() { return this.name; }
来源：http://hz.hysaishi.cn/gtccmszuxd.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtbnmtzquf.html

Java: String greet() { return name; }
来源：http://hz.ivvv.top/gtyfllrrnf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtixsvasdu.html

Ruby: def greet; @name; end
来源：http://hz.yuxming.cn/gtejyyggjp.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtqqtkpoqj.html

[G05] 继承
来源：http://hz.tianlin.xyz/gtlqnfnauf.html

Py:   class Admin(User): pass
来源：http://hz.ybcxt.top/gtxfrooinx.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gthixvbikn.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtjvtdubdo.html

TS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gtxqgkfooq.html

Java: class Admin extends User {}
来源：http://hz.jqgfzy.top/gtargcoqgp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtkodxxhuj.html

Ruby: class Admin < User; end
来源：http://hz.jiagoushi.top/gtiygbgqep.html

C#:   class Admin : User {}
来源：http://hz.sysykeji.top/gtxhgeoffh.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtbxitqkfl.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtdmrfxpyw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gthjfqukoz.html

JS:   greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtvsiwjisu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtqpgqnlxp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gturgsiqse.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuanzhike.top/gtrpmbcioy.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtffflygpu.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtlrselqwj.html

[G07] 调用父类方法
来源：http://hz.fengsongda.top/gtzwezvisc.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtnikahlym.html

PHP:  parent::greet();
来源：http://hz.svipenyu.cn/gtqhpuchrs.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtknhiimsh.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtavevcbxx.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtrrhtlebw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhengqikj.top/gtqulyffgg.html

Ruby: super
来源：http://hz.cqqwz.cn/gtupocnlpo.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtgjmmfjza.html

[G08] 静态方法与属性
来源：http://hz.yuanzhike.top/gtesyfzxhp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtdbilldsm.html

PHP:  public static function f() {}
来源：http://hz.jyoumei.cn/gtojyygjpg.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtejikkisz.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtsbzoigzp.html

Java: static void f() {}
来源：http://hz.smart0.xyz/gtwzgenyum.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gtfsqpkqlk.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtztnhrief.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtxjgcdtyf.html

[G09] 接口 / 抽象类
来源：http://hz.yonumen.top/gtlrgesrrl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangshuangyany.cn/gtjaaqxmui.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtpwbevzps.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.redwolf501.top/gtxodeqqkj.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtddfjmhis.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtftopfpcv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nwbrower.top/gtasbnescg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.316326.xyz/gtplhfxtjq.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtfnprpmfv.html

[G10] 访问控制
来源：http://hz.quarkkingdee.top/gtamzsijan.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtxvlddadk.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gtgpenywqw.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtpqbaolts.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtcfqtlcyj.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtnwldvpqw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtxqopaiwm.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtofkteqvl.html

C#:   public / protected / private / internal
来源：http://hz.jinghuilouyu.cn/gtlxvxgqqz.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gtnnndwmmh.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtwlogqtyh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtifqpoohb.html

JS:   get name() { return this._name; }
来源：http://hz.feifeiyinyue.top/gtushuyeps.html

TS:   get name(): string { return this._name; }
来源：http://hz.hfpthk.cn/gttdgaifzm.html

Java: public String getName() { return name; }
来源：http://hz.gotoacloud.top/gtrjloqvex.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yonumen.top/gtqajabcxu.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtoyjqyygw.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtawrywyeh.html

[G12] 对象转字符串
来源：http://hz.jinghuilouyu.cn/gtcodegtun.html

Py:   def __str__(self): return self.name
来源：http://hz.quarkkingdee.top/gttkeqgzrc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtuyyhjjla.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtshchlfyx.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtedpocqye.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtyahrtxan.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtvpyjtyrb.html

Ruby: def to_s; @name; end
来源：http://hz.jinyuanbaomall.cn/gtqxhzvngx.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtytgtpxvs.html

[G13] 判断对象类型
来源：http://hz.jinyuanbaomall.cn/gtdiikkudb.html

Py:   isinstance(u, User)
来源：http://hz.cashguo.top/gtjjirdekt.html

PHP:  $u instanceof User
来源：http://hz.hongshengwenyu.top/gtzcvffrwh.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtejawoewy.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gthlutschz.html

Java: u instanceof User
来源：http://hz.ppjwa.cn/gtxsgpmmby.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhixingplan.top/gtjqbtlmrz.html

Ruby: u.is_a?(User)
来源：http://hz.yonumen.top/gtfjzhepvj.html

C#:   u is User
来源：http://hz.yueranfly.top/gtkssvfcqr.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtraizcmfq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtgsnzrevf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtxiquuygf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gttrqymaro.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj202588.top/gtnstnyzwz.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtmkudylkm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gteovgxosr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gthkbospbz.html

C#:   record User(string Name, int Age);
来源：http://hz.hfpthk.cn/gtrxwnving.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtkxbhdypu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gtmtlkjqew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhiwuduotai.top/gteryezjdo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtpksetljp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtsexrvdey.html

Java: enum Color { RED, GREEN }
来源：http://hz.tian-w.cn/gtibfewjxn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtnjospxrf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cheryme.top/gtibsnltua.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuetiantiany.cn/gteftnwtvm.html

[G16] 对象转数组 / 字典
来源：http://hz.tanke756.top/gtzdzghpao.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zycfv.cn/gtuwmxwuxa.html

PHP:  get_object_vars($obj);
来源：http://hz.9152youxi.cn/gtbtdbkfis.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtdvmjetct.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtsdhrkppw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtscxerjmd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.c1oappe.top/gtyzgbhbhc.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtlxxyedtd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yanxiufei.cn/gthllifnxg.html

================================================================================
来源：http://hz.xuanzx.com/gtkmfvkqsd.html

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtmblnysib.html

================================================================================
来源：http://hz.iojbl.cn/gtwnaxjiyp.html

[H01] try / catch 基础
来源：http://hz.guowangkeji.top/gtrsdgtnfz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj20258.top/gtdxwdikxx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hysaishi.cn/gtkmsopfyb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtacivrouc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtzkmowpim.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj202588.top/gtzdcvktzw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangshuangyany.cn/gthgxxdsha.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtfkqlcbgr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtzpteazgi.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtakesrxty.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtpbpyccki.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtrgbqwbbv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtxybspwvy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtirznjlyz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtnhvaygup.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtqkxspnsq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gtshbvorqy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yangfankeji.com/gtcuuoonxr.html

[H03] 主动抛出异常
来源：http://hz.zhiwuduotai.top/gteahhhzpp.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gthpzjuiqz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtlxprzvoq.html

JS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtxqgifdbv.html

TS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtzwxcvjfw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtgxwcpsbu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sweek.top/gtuichdehu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtwljtevrc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtqdakfpuo.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtyekbulxj.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgfzy.top/gtzclyqfop.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtxpmcvuxn.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtnbjrehnh.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtksyqlpzr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gthmrfmfrn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtkgtuadct.html

Ruby: class MyError < StandardError; end
来源：http://hz.dianchejie.cn/gtxkcsajfu.html

C#:   class MyException : Exception {}
来源：http://hz.chenjidiqi.icu/gtqpdezqin.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gtiwotezen.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gtlsresthl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtmynuqyxm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtzibivaos.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtzoaulwhy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtcqiikunc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydjk.org.cn/gtldehepsj.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtkfwiqylw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.9152youxi.cn/gtmyyhtjnh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtkarhyuoo.html

Py:   value = d.get("k") or default
来源：http://hz.chenlongwang.top/gtpsotvzbq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtpdwplebc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtryfxqcos.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtichjpoxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tian-w.cn/gtkhafaeve.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.svipenyu.cn/gthbfhqjtc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtdvajlidy.html

C#:   obj?.A?.B ?? default
来源：http://hz.yanxiufei.cn/gtnsazwvcb.html

[H07] 断言
来源：http://hz.fengsongda.top/gtskfevmmr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tianlin.xyz/gtppnhluae.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtcpfburcz.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtgbqktggr.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtnqsjuhvs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtedkiwxzm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fzhhl.top/gtexejmoso.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtsfwzpokj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtfwquppmj.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtpcdxwdil.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gaohongyu789.top/gtlzopfcnu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gtqdjgnyhq.html

JS:   e.message;  e.stack
来源：http://hz.shuidangran.top/gtwhmcryzm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuetiantiany.cn/gtrtmxcmsr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangkeji.top/gtydzxbidi.html

Go:   err.Error()
来源：http://hz.jinqigfzy.top/gtkcynwibm.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtgcwoxezq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtuwvvatma.html

[H09] 带错误码的异常
来源：http://hz.jiagoushi.top/gtrbbhgxfb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtnbnuetyb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gthjfkkybn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtlujcbags.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gtjxfhjarj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtzjmkoyop.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yvedp.cn/gtyypsfiio.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtavoguvln.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtzyerfeqg.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtaxijjibm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daxiang520.top/gtufopcgby.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuanzx.com/gtdkvpzhaq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinghuilouyu.cn/gthnfcogka.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtbxskryaq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgufenzy.top/gtgdsibuco.html

Go:   defer f.Close()
来源：http://hz.hywenlv.cn/gtrspbgceg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xziqi.cn/gtxonpqtvz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtmmyarman.html

================================================================================
来源：http://hz.9152youxi.cn/gtfztvnods.html

I. 正则表达式
来源：http://hz.yonumen.top/gtsdcaijni.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmotgwcrj.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gtkxkkople.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtbazsovzh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuxming.cn/gtqhbcwdkw.html

JS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtvorgabdf.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtlequaavd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtxpepsaix.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daxiang520.top/gtffctrhrt.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtkoqlosyd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhixingplan.top/gtwwrawwdo.html

[I02] 提取所有匹配
来源：http://hz.guowangkeji.top/gtfnlwcmuh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhengqikj.top/gthxgmoptw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gthtpoaoxc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtikssjrzg.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtsybhgvyc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gttinwlvqn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtdqnggyld.html

Ruby: s.scan(/\d+/)
来源：http://hz.yanxiufei.cn/gtwdeykrqp.html


<!-- 参考信息 -->