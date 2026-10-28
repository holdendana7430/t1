代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hywenlv.cn/gtrlthwogz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtxougzqne.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtvdyctldh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gzhubu.top/gtboakoaom.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hywenlv.cn/gtukpqvvrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gtnsezekuv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtwycoxlse.html

[F08] 遍历目录
来源：http://hz.zhaomingkeji.xyz/gtxqhnhrye.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtsjiwipag.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xingfuxueyuan.xyz/gtpstuszkk.html

JS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtxzzuupos.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtcmoyqoku.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtlcevpoiu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtwvautnln.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtoxlaedun.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtcqrlissc.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtqehjpzwy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigufen.top/gtrryogkxy.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtuyiavmjz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtjsermwfv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtbmxobhuc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtwaerhsgz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenjidiqi.icu/gtliaugxmm.html

Ruby: File.size("a.txt")
来源：http://hz.ydzc1.top/gtwbzxsowh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pengpengdd.cyou/gtrcjankjz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangtech.top/gtrqnepntj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gthjogbnwk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hfpthk.cn/gtqenhoafk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtkapphuvz.html

TS:   path.extname("a.txt")
来源：http://hz.gotoacloud.top/gtxyakutgh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gthtvkpvtl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hysaishi.cn/gtrlwmhrww.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtouyczjcn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.dianchejie.cn/gtaarxgyle.html

[F11] 复制与移动文件
来源：http://hz.aizwys.cn/gtdplmqbqu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtiioewsja.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigfzy.top/gthoskptqc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtmhrsbhth.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtxiqbwytp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.smart0.xyz/gtjhjjdkxa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shuidangran.top/gthswmqodi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtikeizmde.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cheryme.top/gtkdvpwvht.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gtogcdjame.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtzmvhofyd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtliuscwqj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj202588.top/gtepyyduch.html

TS:   // 同上
来源：http://hz.sweek.top/gtdqlhqvpy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgufenzy.top/gtxivwtktb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.mhx1999.top/gtcmtdjlcc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtnbfbyehv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cashguo.top/gtkyqseyxw.html

================================================================================
来源：http://hz.jqgfzy.top/gtjglmuwbr.html

G. 面向对象
来源：http://hz.ehwqpu.com/gtulmfrtme.html

================================================================================
来源：http://hz.fzhhl.top/gtzwpxsehf.html

[G01] 定义类
来源：http://hz.redwolf501.top/gtfqfkrpxc.html

Py:   class User: pass
来源：http://hz.aizwys.cn/gtafckwprz.html

PHP:  class User {}
来源：http://hz.hnxiangtu.top/gtabmmrxwn.html

JS:   class User {}
来源：http://hz.chenjidiqi.icu/gtjwquipwo.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtqbvljlvb.html

Java: class User {}
来源：http://hz.cqqwz.cn/gtfjsrjqof.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtwwywuvbs.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtwwvenvvi.html

C#:   class User {}
来源：http://hz.hnxiangtu.top/gtlljngizg.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtvwsjvvng.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.andypj.xyz/gtqyjrvzqu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigufen.top/gtckilddnx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtamktdwng.html

TS:   constructor(public name: string) {}
来源：http://hz.aizwys.cn/gtwkqiwdtl.html

Java: User(String name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtryusswnn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fzhhl.top/gthcsvvsuu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.haohaochexian.top/gtpqdcipnk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gtmyeuuifx.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtfnzahcgn.html

Py:   self.name = "x"
来源：http://hz.ydzc1.top/gtafottkvs.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtalpnkuoh.html

JS:   this.name = "x";
来源：http://hz.yj20258888.top/gthmsnzmum.html

TS:   name: string = "x";
来源：http://hz.jyoumei.cn/gtwogmvhui.html

Java: private String name;
来源：http://hz.52xcode.cn/gtvxcvtbqy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangdashe.top/gtpnayyqhy.html

Ruby: @name = "x"
来源：http://hz.nanxuanxn.top/gtgrjulsxk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtimcfihts.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gttgpdvnky.html

Py:   def greet(self): return self.name
来源：http://hz.shzxlz.cn/gtkkywmwtm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtldwsihcb.html

JS:   greet() { return this.name; }
来源：http://hz.hnxiangtu.top/gtkjyqxigg.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtvmmclcqg.html

Java: String greet() { return name; }
来源：http://hz.ppjwa.cn/gtjtzbvpmv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtwfraxebx.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtmgrjrrzp.html

C#:   public string Greet() => Name;
来源：http://hz.gzhubu.top/gtvhztlnvr.html

[G05] 继承
来源：http://hz.yj202588.top/gtlbuccdhd.html

Py:   class Admin(User): pass
来源：http://hz.tian-w.cn/gtsscuwayn.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtcrcffzsw.html

JS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtvwllmken.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtandhpbux.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtjzinhryw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cheryme.top/gtaoglihdg.html

Ruby: class Admin < User; end
来源：http://hz.wangdashe.top/gtpkhzrvnq.html

C#:   class Admin : User {}
来源：http://hz.cucudq.cn/gtsflpqrgt.html

[G06] 重写方法
来源：http://hz.ivvv.top/gtxpjwdxpn.html

Py:   def greet(self): return "admin"
来源：http://hz.cashguo.top/gtscmnpwdp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtrykecofv.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtkazjpptf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtqofzxgsn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yvedp.cn/gtspnuukoo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtbqlqmpxv.html

Ruby: def greet; "admin"; end
来源：http://hz.sufxvd.cn/gtnootncfw.html

C#:   public override string Greet() => "admin";
来源：http://hz.svipenyu.cn/gtfahkxcvx.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtwmwtarin.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtdaknfsmf.html

PHP:  parent::greet();
来源：http://hz.jyoumei.cn/gtzvcyjkss.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtqbongddx.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtgxypmtlx.html

Java: super.greet();
来源：http://hz.chenlongwang.top/gtplnkkxju.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuanzhike.top/gtwqnkknov.html

Ruby: super
来源：http://hz.52xcode.cn/gtqninffea.html

C#:   base.Greet();
来源：http://hz.birdmap.top/gtvcguabba.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtvjowkxpa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangkeji.top/gtmlacqawu.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gttgqzwlcd.html

JS:   static f() {}
来源：http://hz.snrcjt.cn/gtrqgfxwms.html

TS:   static f(): void {}
来源：http://hz.jlsjyb.cn/gtwcjmsbyc.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtmrqmjzkn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtzapkxykq.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtbhfbsszp.html

C#:   public static void F() {}
来源：http://hz.jiagoushi.top/gtaujmxcer.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtgrybmlol.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.havefunace.top/gthpbnwbuj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gtoboxzgjl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtrexuxhdt.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtttpopxlf.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gttcjanqbx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ywan-chungtsiang.top/gtobcdipqe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtntanhaty.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtjpeztash.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gthfkwmcdr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gttpvueump.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gtrbgapxki.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtnrfuvvlk.html

TS:   public / protected / private
来源：http://hz.andypj.xyz/gtvoyprnrr.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtvvrwqpec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtiqtrsamj.html

Ruby: public / protected / private
来源：http://hz.fengsongda.top/gtajaiunvn.html

C#:   public / protected / private / internal
来源：http://hz.gogol.net.cn/gtgvvdrsyo.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtiqdiqaxp.html

Py:   @property 与 @x.setter
来源：http://hz.jinqigufen.top/gtjosvwljv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtcdbkmrzk.html

JS:   get name() { return this._name; }
来源：http://hz.svipenyu.cn/gtpdozzxkx.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtvndlqnap.html

Java: public String getName() { return name; }
来源：http://hz.zhixingplan.top/gtgfmzuihx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtptfyxjii.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gtfeseuohi.html

C#:   public string Name { get; set; }
来源：http://hz.jlsjyb.cn/gtniilpieh.html

[G12] 对象转字符串
来源：http://hz.kuanghao11.cn/gtrvwxtvqw.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtqtxredgn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ivvv.top/gtiacwrrvp.html

JS:   toString() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtcmxprsby.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtedixkxke.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtqbabiqvs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zycfv.cn/gtugigaofu.html

Ruby: def to_s; @name; end
来源：http://hz.mhx1999.top/gtsojzmmyp.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtshcnbgms.html

[G13] 判断对象类型
来源：http://hz.cheryme.top/gtkgiawxjn.html

Py:   isinstance(u, User)
来源：http://hz.ppjwa.cn/gtzhypozrc.html

PHP:  $u instanceof User
来源：http://hz.cheryme.top/gtfhxiajsn.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gtntpzzaxt.html

TS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtgxpbswei.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtbamouoce.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtejkrwsow.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtuleixpif.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtcpqsjkxs.html

[G14] 数据类 / record
来源：http://hz.316326.xyz/gtydclnwqw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cashguo.top/gtcidzobat.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtvkhbylvb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gthwfxccci.html

TS:   type User = { name: string; age: number };
来源：http://hz.0kj1m.cn/gtwwhwfyjp.html

Java: record User(String name, int age) {}
来源：http://hz.aibaodan.cn/gtzjepwagx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gttempzgqe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhaomingkeji.xyz/gtlpvxgkfb.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258.top/gtmjhgmpgf.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtmhvqeogz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhijiandao.cn/gtvupldmyb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gtlngdvydc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangdashe.top/gthnbgntbf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gthepfekbn.html

Java: enum Color { RED, GREEN }
来源：http://hz.shuidangran.top/gtqgyikqpu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtzmyvokee.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hywenlv.cn/gtzpsyfnbu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtuidbhwrf.html

[G16] 对象转数组 / 字典
来源：http://hz.52xcode.cn/gtyzbfzrgo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtgkhpcrsr.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtahjvwhny.html

JS:   Object.entries(obj)
来源：http://hz.sweek.top/gtxtaslnba.html

TS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtyzfqyocc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtaweuyhbl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtwemjjhiu.html

Ruby: obj.instance_variables
来源：http://hz.nwbrower.top/gthukixxyt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.mhx1999.top/gtaovnfdlt.html

================================================================================
来源：http://hz.tanke756.top/gtpybejsee.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gthfflyucz.html

================================================================================
来源：http://hz.cheryme.top/gtfjzgmrlu.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtdbotnvlk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shuidangran.top/gtkjzolwid.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtxmxpuuuu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtknvsgywl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtnugesjxr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pengpengdd.cyou/gtqjzqzpex.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangtech.top/gtzjrvideu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jianghu66.top/gtzhzouvpc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtibiwgwtr.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtmlmjqidp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shuidangran.top/gtftfloizq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtfegnxosf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtjklzzufo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtqyovxuqd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtzggkfvox.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtiiqbhcxm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtodohcjdu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gttiyowwci.html

[H03] 主动抛出异常
来源：http://hz.gotoacloud.top/gtgkeqjafd.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtrjopfajy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtefehhgik.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtzzdvnklz.html

TS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtujnetkrs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gttvhpchcz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtzrdsuana.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shangyingyoupin.top/gtrxoldmiy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtmbncxxwn.html

[H04] 自定义异常类型
来源：http://hz.sxryk.cn/gtxcosyhde.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtxbbaqfym.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtfgxseqkr.html

JS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtrdekzegd.html

TS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtdwmbebpu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtqzkcvfok.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtltclcvum.html

Ruby: class MyError < StandardError; end
来源：http://hz.gotoacloud.top/gtyzycfabo.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtncfbreak.html

[H05] 捕获特定类型
来源：http://hz.guowangkeji.top/gtnhinyzxp.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtltzecieb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gthxlqcvwb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gthvfjcmft.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtnivsebpe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinyuanbaomall.cn/gtexsshkfc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gzhubu.top/gtaccmwvrn.html

Ruby: rescue ArgumentError => e
来源：http://hz.meibo888.top/gtobdgolqf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fzhhl.top/gtzqyqzzxz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fzhhl.top/gtovxyovof.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtcyixssnp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtncpnjdco.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtibfdsmyj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtigonavvr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hysaishi.cn/gtdoptufzv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.andypj.xyz/gtxeminkww.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhengqikj.top/gtqhefptie.html

C#:   obj?.A?.B ?? default
来源：http://hz.haohaochexian.top/gttrstoqte.html

[H07] 断言
来源：http://hz.jianghu66.top/gtwuaaipaz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gthfrkbiig.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtygxxrgfi.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtuvkvdxac.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtaszjbjcr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtwecpmuej.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtocrftmcx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhongyouzk.top/gtcraguoau.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtvgayqxkg.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhaomingkeji.xyz/gtutbhezkj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuanzx.com/gtlfvtytyy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shangyingyoupin.top/gtwwrmkpel.html

JS:   e.message;  e.stack
来源：http://hz.tanke756.top/gtppuugcts.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtcdmlunrw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhijiandao.cn/gtmfrqkvji.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gtltrzqclt.html

Ruby: e.message;  e.backtrace
来源：http://hz.fengsongda.top/gtfmyrioht.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydjk.org.cn/gtsxmksusi.html

[H09] 带错误码的异常
来源：http://hz.jiagoushi.top/gtgiwqgozz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.mhx1999.top/gtwwroobke.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtrbehpbiv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtocomwqsl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daxiang520.top/gtsvmcvead.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gtmhnjrcld.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ywan-chungtsiang.top/gtlsptthpi.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtjeqcanjc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtuvkusgly.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtqvfhgutq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gtyobvlvgl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.52xcode.cn/gtpbhensmm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtefszvoud.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtlqluauqw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.mhx1999.top/gtrfjywmbv.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtfuvnubzr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dianchejie.cn/gtiqhyrrux.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtxmfmjcyr.html

================================================================================
来源：http://hz.sufxvd.cn/gtbtflfsuf.html

I. 正则表达式
来源：http://hz.ppjwa.cn/gtijgnpqtk.html

================================================================================
来源：http://hz.zhixingplan.top/gtwcweugdf.html

[I01] 判断是否匹配
来源：http://hz.hongshengwenyu.top/gtgoslcgac.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtisiprdiy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gthnzahizy.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtazgoopot.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtqiqqrreu.html


<!-- 参考信息 -->