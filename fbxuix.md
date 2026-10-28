代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenlongwang.top/gtotkldjac.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtvcirvpau.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtlbwsvhaz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtpouiacxd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yueranfly.top/gtokainwxu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtkmlojevw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtqqjwhzem.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gtrviruzsv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.c1oappe.top/gtkdvioqij.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhijiandao.cn/gtpxpckmdj.html

JS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtzhzuzivn.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtwddovqpi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtfdqxoegi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxinkj.top/gtnnkomeaz.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtnvwpadjp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtznjjwpjp.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtbvrimzzj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.quarkkingdee.top/gtqeysftpj.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtulsiwemc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtizulxyzo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtccesykbl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtbrrebgku.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtcmfumkmt.html

Ruby: File.size("a.txt")
来源：http://hz.tian-w.cn/gtchtsbxtp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtogszkgxg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gtvdykxsng.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtmdyrfdvv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtuygudidv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtxybfnldl.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gtejcqshrj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cdnleiting.top/gtgcdvgqhg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gtdwcptpzs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtqmegxequ.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yuanzhike.top/gtzpcltyry.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtjzrackkk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtkxyxmjkf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aizwys.cn/gtpirliken.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtvrbmxogz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtifjqjuyd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yongpay.top/gtpmrrtcgg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtegtjdzwq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtqqplwgqa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtuzjwcevh.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gtxbxhugpc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cucudq.cn/gtudywiogp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtoxgxsvau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtwarxcnbh.html

TS:   // 同上
来源：http://hz.andypj.xyz/gttcazrgnb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gttsshfpiy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.vqdsnc.cn/gtmqnpmtyc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgfzy.top/gtuahuajkn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gtkujdmrlk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzofraiaq.html

G. 面向对象
来源：http://hz.dianchejie.cn/gtqemcvaml.html

================================================================================
来源：http://hz.svipenyu.cn/gtzrlkgktm.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtfoiszpht.html

Py:   class User: pass
来源：http://hz.wangdashe.top/gtxpyvljmu.html

PHP:  class User {}
来源：http://hz.jinqigfzy.top/gtopdaioei.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtwzfphuvm.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtbhwuvzos.html

Java: class User {}
来源：http://hz.gzhubu.top/gtvwxueaqm.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gtwsodzgbn.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtrlefuhdw.html

C#:   class User {}
来源：http://hz.yuanzhike.top/gtavjdbujg.html

[G02] 构造函数
来源：http://hz.snrcjt.cn/gtxdzgxjsx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gotoacloud.top/gtnvarofur.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinyuanbaomall.cn/gtkmjjigzt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtikfkvsef.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gtfrjyohtp.html

Java: User(String name) { this.name = name; }
来源：http://hz.ybcxt.top/gthgskwcri.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuanzhike.top/gtwhuuzwhh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtyxdatxcz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.9152youxi.cn/gttvvdaplr.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtvhstrgms.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtgtbdnkmh.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtliraqwda.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangtech.top/gtznkyhebx.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gttceyvepc.html

Java: private String name;
来源：http://hz.52xcode.cn/gtcohdpqur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangkeji.top/gtfdelnkxt.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gtketkiuhj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gzhubu.top/gtvnfzybyq.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtpiwapipc.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtvzljswbv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtdgzevqwz.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtcgmegwpc.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtsmgzvotz.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtoajqwqsx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtbvlomjpo.html

Ruby: def greet; @name; end
来源：http://hz.jqgfzy.top/gtwfnqhbap.html

C#:   public string Greet() => Name;
来源：http://hz.xuetiantiany.cn/gtfsyiyqce.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtwkcklsoh.html

Py:   class Admin(User): pass
来源：http://hz.zycfv.cn/gtnyrljobb.html

PHP:  class Admin extends User {}
来源：http://hz.fengsongda.top/gtpojvioni.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtczrlkpoq.html

TS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtuxhlcntp.html

Java: class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtczofmvox.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zycfv.cn/gtivmbbxbh.html

Ruby: class Admin < User; end
来源：http://hz.jqgufenzy.top/gtzhqvdgdf.html

C#:   class Admin : User {}
来源：http://hz.hfpthk.cn/gtscpuofsu.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtjdoaaqlq.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtvidrkmpc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yueranfly.top/gttyvegbzm.html

JS:   greet() { return "admin"; }
来源：http://hz.pycfn.com/gtiqadlvvp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtrnoukfzj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtzavrphzf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jianghu66.top/gtuzsvbjtp.html

Ruby: def greet; "admin"; end
来源：http://hz.sweek.top/gtspidwcve.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtbcwrpxqa.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gtpisvhjjk.html

Py:   super().greet()
来源：http://hz.zhixingplan.top/gtcxbydlee.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtottdwhqx.html

JS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtaryskhwc.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtknycfaxv.html

Java: super.greet();
来源：http://hz.hammf.cn/gtplifrfsm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sufxvd.cn/gtyhlqfgsc.html

Ruby: super
来源：http://hz.yuanzhike.top/gtyaiaimid.html

C#:   base.Greet();
来源：http://hz.cheryme.top/gtlnbxdnur.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtmiemeujm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuanzhike.top/gtqfkkvjfd.html

PHP:  public static function f() {}
来源：http://hz.sweek.top/gthsptlmve.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtdmkxwvlr.html

TS:   static f(): void {}
来源：http://hz.gogol.net.cn/gtkebszxmi.html

Java: static void f() {}
来源：http://hz.yj202588.top/gtoqxxiozm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhiwuduotai.top/gtyuuprjro.html

Ruby: def self.f; end
来源：http://hz.jinghuilouyu.cn/gtdsfllhri.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtwjdooggw.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangkeji.top/gtiuqmntkd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtcfgaebkt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtibhipcit.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtvcjvslpi.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtfqabowml.html

Java: interface Shape { double area(); }
来源：http://hz.quarkkingdee.top/gtwymgjadm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuanzx.com/gtiftfavyn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtkjnfwhmn.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtirwymteh.html

[G10] 访问控制
来源：http://hz.tanke756.top/gthrtrfkcn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtktgspbjs.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtpalfipgx.html

JS:   #private 字段；其余公开
来源：http://hz.cashguo.top/gtfbfkljew.html

TS:   public / protected / private
来源：http://hz.sweek.top/gtxcbvozuh.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtbkjgnpai.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nwbrower.top/gtndbwvvzv.html

Ruby: public / protected / private
来源：http://hz.nwbrower.top/gtveruxzim.html

C#:   public / protected / private / internal
来源：http://hz.zdqjudy.top/gtywmhzyto.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtmfzoviry.html

Py:   @property 与 @x.setter
来源：http://hz.jinghuilouyu.cn/gtvseinvwa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtjgneinng.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gthtgfylhe.html

TS:   get name(): string { return this._name; }
来源：http://hz.meibo888.top/gtjstwpiiu.html

Java: public String getName() { return name; }
来源：http://hz.daria6918.cn/gtpzaexbrw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtauwydduc.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtdbbvkqpx.html

C#:   public string Name { get; set; }
来源：http://hz.shangyingyoupin.top/gtpmrlefck.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtyedgooup.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gttfcfoegh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtmtzhvwct.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gttesygxuh.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtfsppmtby.html

Java: @Override public String toString() { return name; }
来源：http://hz.daxiang520.top/gthgamshzh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtiiywtise.html

Ruby: def to_s; @name; end
来源：http://hz.pengpengdd.cyou/gtenaevjwb.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gtrucxwhgx.html

[G13] 判断对象类型
来源：http://hz.jinghuilouyu.cn/gtvqvxvqpg.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangtech.top/gtxymbcchc.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtvqqompuq.html

JS:   u instanceof User
来源：http://hz.jianghu66.top/gtxrcxzqos.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtvwkxvciy.html

Java: u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtclhnwcei.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtsebyyuzr.html

Ruby: u.is_a?(User)
来源：http://hz.andypj.xyz/gtjtfnbmmt.html

C#:   u is User
来源：http://hz.xuanzx.com/gtvzgbalwf.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtkqbefldg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jlsjyb.cn/gtlzcxzxdw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuxming.cn/gtqhkixwtr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sweek.top/gtzdeamtga.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenjidiqi.icu/gtzvndrpwt.html

Java: record User(String name, int age) {}
来源：http://hz.hywenlv.cn/gtebnvmzdv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydzc1.top/gtpokoxfsd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangkeji.top/gtvlvvakms.html

C#:   record User(string Name, int Age);
来源：http://hz.havefunace.top/gthnuqoyhq.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gtktfkyqlq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtpbipbewt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gtuwhqudbg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtclnltobp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtqyjoemck.html

Java: enum Color { RED, GREEN }
来源：http://hz.andypj.xyz/gtjqbcqtno.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jiagoushi.top/gtgfjqsivk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zycfv.cn/gtzpxdduxt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtfqyjfran.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtuphyoqge.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtxubharwy.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtkcqtftbp.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtqibswfcq.html

TS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtslziepbu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtdiqvsgep.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtyafjatsd.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtiqfztdfp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtejwgegba.html

================================================================================
来源：http://hz.cdnleiting.top/gtozivaoyc.html

H. 异常与错误处理
来源：http://hz.iojbl.cn/gteqrnfadz.html

================================================================================
来源：http://hz.yangfankeji.com/gtvvmzdfxn.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gthtcaiwmt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shuidangran.top/gtmexjeemf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tian-w.cn/gtxcpliduw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtjiutxihp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtlaaeautr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhaomingkeji.xyz/gtuebvpdbt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtanwwksbu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtgwvwjffq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhiwuduotai.top/gtlqilppoy.html

[H02] finally / ensure 收尾
来源：http://hz.cucudq.cn/gtnjeqqqqr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtrbflqoxk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtgavrtkfq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtraqbmcao.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtsiqkxtui.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtlxpputfd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.meibo888.top/gtotykkpue.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtbchipnmu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangdashe.top/gtcasmzyoi.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtppmdsspv.html

Py:   raise ValueError("错误信息")
来源：http://hz.jyoumei.cn/gtzbjllrmd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtaorzebdb.html

JS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtentbhitk.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtryjmiwpt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj202588.top/gtchzsorfw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dashuyun.cn/gtqktzltxf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ivvv.top/gtshomxakc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtfrqwubjo.html

[H04] 自定义异常类型
来源：http://hz.ivvv.top/gtvcjugqfi.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtskuhwluv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtzdzctjze.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtvcknsxwh.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtxbxvlwlg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtgupkddzw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtstbujvqk.html

Ruby: class MyError < StandardError; end
来源：http://hz.52xcode.cn/gtfjdwdahs.html

C#:   class MyException : Exception {}
来源：http://hz.havefunace.top/gtomyrdnuk.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtjxphcrzn.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtmxkequav.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aibaodan.cn/gtnggpkfzb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtjarjlcxz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtqgeutlhk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yueranfly.top/gtzkplttbo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yvedp.cn/gtanxkqlln.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtjwjyoqaf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.0kj1m.cn/gtyyslcbiu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtwfxlhgkz.html

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gtzbmizfti.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtqvqkihcc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtdjlkgvom.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtaqkyspzt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pycfn.com/gtxaaafncm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gtecoeqpdb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sysykeji.top/gtukctgiwk.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuxming.cn/gtciufeboj.html

[H07] 断言
来源：http://hz.feifeiyinyue.top/gtzdylujzf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jlsjyb.cn/gtkfecdkjt.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gtdifyslnv.html

JS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtjqwnjefx.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtrosgjvnw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtqfommwnq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhijiandao.cn/gtebjhwxut.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tianlin.xyz/gtxcojfcxb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gtlnylzxbn.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtzsyfxnbw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhongyouzk.top/gtrfukylxw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gttrgrnksh.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtwzxmjzyv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtkwudaitj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gtjsiijxqr.html

Go:   err.Error()
来源：http://hz.zdqjudy.top/gtgueoqiko.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtkdemyaod.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtzcztwvee.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtvblpvlht.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gogol.net.cn/gtgxtmwtun.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gtxxxckxkz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtmrgefeak.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gtwbxaxwys.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gteyhmfuxv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtpbzcaibq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gttnmpsdwe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.0kj1m.cn/gtjowbrvxk.html

[H10] 资源自动释放
来源：http://hz.jinghuilouyu.cn/gtcehbonfd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtlwcjudoe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gttdqhnkbl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtlpetbhak.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtduvnkxvp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtlzyjlvsp.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtejqbdowb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtrlgmzmfo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtukenlxax.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmyolmcgy.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtmiyzdkjc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtidavvtxk.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtbytpcugw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gteigftkcx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.c1oappe.top/gtxmwuwdyl.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtpavkanns.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtrooxpstu.html


<!-- 参考信息 -->