代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cheryme.top/gtwgohevqe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.feifeiyinyue.top/gthaaurius.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xziqi.cn/gtqyvozxkr.html

[F04] 追加写入文件
来源：http://hz.zycfv.cn/gtzimyatbz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtsqwwqeok.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtuieitrif.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnqzz.top/gtoaqjwjkv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gthlfohoxp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.svipenyu.cn/gthywvpqrq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gthkbhkksj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtifmavycb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangdashe.top/gthqkyqmwr.html

[F05] 判断文件或目录是否存在
来源：http://hz.sufxvd.cn/gtrthxfwew.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ivvv.top/gtuizrndrs.html

PHP:  file_exists("a.txt");
来源：http://hz.jianghu66.top/gtfixmegjc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtvgrmwxcs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtcxonwsfu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtkntribji.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.smart0.xyz/gtivdpuolm.html

Ruby: File.exist?("a.txt")
来源：http://hz.daxiang520.top/gtfoqxsldf.html

C#:   File.Exists("a.txt")
来源：http://hz.zhijiandao.cn/gtljxhrupz.html

[F06] 删除文件
来源：http://hz.0kj1m.cn/gtnkdqcxnp.html

Py:   os.remove("a.txt")
来源：http://hz.wangdashe.top/gtqcgateub.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtpfebkoyn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtqjithtfd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtpblmqnpz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtxpalckvz.html

Go:   os.Remove("a.txt")
来源：http://hz.hnqzz.top/gtehwrxcxj.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtdbwnrbma.html

C#:   File.Delete("a.txt");
来源：http://hz.xuetiantiany.cn/gtmlkmcush.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtatxkfihp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtlgbidqvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.smart0.xyz/gtkateeavg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtqefreddl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gttidhkzku.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtounwiuuf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtannarqbx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.c1oappe.top/gtgggmkffc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gtfdqtzmwo.html

[F08] 遍历目录
来源：http://hz.gogol.net.cn/gthtadhnso.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fzhhl.top/gtokwrbfla.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258.top/gtxjfuwryl.html

JS:   fs.readdirSync("dir")
来源：http://hz.xziqi.cn/gtpuzhqzoh.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gteayxbyzh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guannengcc.top/gtvvtnsrga.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gtoawcaqbw.html

Ruby: Dir.children("dir")
来源：http://hz.dianchejie.cn/gtfsrbagtv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtyqxdrxis.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtxwhnsynv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtbkwoeuqf.html

PHP:  filesize("a.txt");
来源：http://hz.jqgfzy.top/gtyumxbcge.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pengpengdd.cyou/gtqebnhnuw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtlhqvncvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gthkumohpb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.birdmap.top/gtvgsrvazv.html

Ruby: File.size("a.txt")
来源：http://hz.zhengqikj.top/gtbulvwnkj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.316326.xyz/gtjlxbbvtj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenjidiqi.icu/gtsiozpprf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtsrvkbxsy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtyccrpfuq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtfcmyddhh.html

TS:   path.extname("a.txt")
来源：http://hz.iojbl.cn/gttsytwjxr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hongshengwenyu.top/gtzlmrvudf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shzxlz.cn/gtvjoaduxr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtziuqjpxi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.9152youxi.cn/gtbxfpnkdq.html

[F11] 复制与移动文件
来源：http://hz.yuanzhike.top/gtphxdulio.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtcqweviuo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtigvjdtui.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtbwjtrrra.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtjnwltoop.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuetiantiany.cn/gtvhxarzxg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gtzpwmbvwm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtmjizyefq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtkeqbdpce.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtzkrfhryu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hfpthk.cn/gtunzrwrrj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xylfe.cn/gtjxdxdgzp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.svipenyu.cn/gtkpdwxepr.html

TS:   // 同上
来源：http://hz.redwolf501.top/gtkgqsnrwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gtrepotuxj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jiagoushi.top/gtxixzuvwr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.feifeiyinyue.top/gtyoxhyzxb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtonuiyclc.html

================================================================================
来源：http://hz.shuidangran.top/gtjbtgdagz.html

G. 面向对象
来源：http://hz.zdqjudy.top/gtpqzltxnr.html

================================================================================
来源：http://hz.gaohongyu789.top/gtvhrvplpg.html

[G01] 定义类
来源：http://hz.yuanzhike.top/gtqrqjnjkb.html

Py:   class User: pass
来源：http://hz.yongpay.top/gtxsoiglee.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtoibomsvk.html

JS:   class User {}
来源：http://hz.ehwqpu.com/gtsteqfsbl.html

TS:   class User { name: string = ""; }
来源：http://hz.jyoumei.cn/gtawyibjfo.html

Java: class User {}
来源：http://hz.havefunace.top/gtmilfmzyn.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gttfyhwzxw.html

Ruby: class User; end
来源：http://hz.ydjk.org.cn/gtjvgbgaxp.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtpygjuidr.html

[G02] 构造函数
来源：http://hz.zhixingplan.top/gtpgaqzfao.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinyuanbaomall.cn/gtffonvdzn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtlemohtvj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtrvyglbun.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtokpqtbzl.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtvrdhajxk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gthypayqlp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gaohongyu789.top/gtogrhrjug.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtmmzuhoyu.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gtklsobbog.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtpcaxpwcf.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtjbiiidbm.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtyjuurjsj.html

TS:   name: string = "x";
来源：http://hz.dianchejie.cn/gtctwcptch.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtmodetwhx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtioiqulnf.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtvilgnxnx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtfrwdtedr.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtsdzmviup.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtcfibpaii.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtdoumfvbb.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gttleyuesk.html

TS:   greet(): string { return this.name; }
来源：http://hz.fzhhl.top/gtybngxqnt.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtiitzyboa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sufxvd.cn/gtehydshjd.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gticyzfyej.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gtlupzijke.html

[G05] 继承
来源：http://hz.bjfxy.top/gtpghsrojn.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtgwimdpzs.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtymaytooa.html

JS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtwizbvjdq.html

TS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtulzkeiks.html

Java: class Admin extends User {}
来源：http://hz.svipenyu.cn/gtfambrqzw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhiwuduotai.top/gtcmqjfyos.html

Ruby: class Admin < User; end
来源：http://hz.9152youxi.cn/gtgbolmloy.html

C#:   class Admin : User {}
来源：http://hz.hnqzz.top/gtqsvmatvm.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtsziinwyz.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtakwkktkn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtmzpailep.html

JS:   greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtzzgqysso.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtggvdspeo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtsmhgzajp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtnawfbcwn.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gteldzhjem.html

C#:   public override string Greet() => "admin";
来源：http://hz.xziqi.cn/gtfsixszrp.html

[G07] 调用父类方法
来源：http://hz.aizwys.cn/gtalpgfptw.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gtgbzipdli.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gtjdxlsian.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gthbmoukin.html

TS:   super.greet();
来源：http://hz.smart0.xyz/gtnzamwlnn.html

Java: super.greet();
来源：http://hz.andypj.xyz/gthedhgbzo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xziqi.cn/gtqakhgquj.html

Ruby: super
来源：http://hz.hfpthk.cn/gtlgammmyi.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtwvlpcuvz.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gtoxieyrvv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.feifeiyinyue.top/gthqyushop.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtqcdyznep.html

JS:   static f() {}
来源：http://hz.jyoumei.cn/gtpprymhhv.html

TS:   static f(): void {}
来源：http://hz.haohaochexian.top/gtfpnvseth.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtpyblgjue.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gthytakrtr.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtlgqtimlf.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtsfsphfft.html

[G09] 接口 / 抽象类
来源：http://hz.zhaomingkeji.xyz/gtbhikdrys.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gtvcmwwsiu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gthsnsarmu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tian-w.cn/gtibikhmfu.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtvymgxfvu.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtkeeiaytx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tian-w.cn/gtnfvbljxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xylfe.cn/gtiezbnmqf.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhijiandao.cn/gtddznduev.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gttyteocbo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sxryk.cn/gtvtawpnqk.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtxdyblkun.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtkcmklgtv.html

TS:   public / protected / private
来源：http://hz.ppjwa.cn/gtqpstcpfg.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtpbohsdci.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigufen.top/gtbjlpzxnc.html

Ruby: public / protected / private
来源：http://hz.hongshengwenyu.top/gtjdbmpajy.html

C#:   public / protected / private / internal
来源：http://hz.mhx1999.top/gtblycwvjb.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtuqqkozoo.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtkedzjwbm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gthvojqyzu.html

JS:   get name() { return this._name; }
来源：http://hz.mhx1999.top/gtsgqolbud.html

TS:   get name(): string { return this._name; }
来源：http://hz.c1oappe.top/gtsbtcbarz.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtoyjaehxm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gtnqfhelaj.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtkrukzwzw.html

C#:   public string Name { get; set; }
来源：http://hz.shuidangran.top/gtxjhpwaiq.html

[G12] 对象转字符串
来源：http://hz.redwolf501.top/gtcucpizmn.html

Py:   def __str__(self): return self.name
来源：http://hz.dashuyun.cn/gtsllozgwm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gteqwopaft.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtrexszdty.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtruejvadp.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtzpopktdt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtbpvydgoq.html

Ruby: def to_s; @name; end
来源：http://hz.ydjk.org.cn/gtraduhlcz.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtytitijav.html

[G13] 判断对象类型
来源：http://hz.jqgfzy.top/gtsjlpmxau.html

Py:   isinstance(u, User)
来源：http://hz.yonumen.top/gthcdxnyzn.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtfttocbun.html

JS:   u instanceof User
来源：http://hz.0kj1m.cn/gtgijbvrsb.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gtbefbzbqi.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gtpzqvzsqz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangkeji.top/gtlgqpumud.html

Ruby: u.is_a?(User)
来源：http://hz.xylfe.cn/gtnmllwnfd.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtiwyjvzxo.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtpfnegscj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtxmnujolr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.snrcjt.cn/gtgykiuugg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuanzx.com/gtacrdkort.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtegvnavgz.html

Java: record User(String name, int age) {}
来源：http://hz.ydzc1.top/gtyfibwkga.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenjidiqi.icu/gtgwbnhrup.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.smart0.xyz/gtvcogefqx.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtvxeilzbe.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gtsrvnlqcl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtnjiyndjr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhaomingkeji.xyz/gtmtdsqyua.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gthooghfty.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtafpifvli.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtilppdevv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuanzhike.top/gtqcdbwyjg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtgyeeoubq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtwpzxubai.html

[G16] 对象转数组 / 字典
来源：http://hz.xuanzx.com/gtjmvzizuy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sxryk.cn/gtxsmrodod.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtfwvorqld.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtbyrjldqe.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtxtptzjzw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.quarkkingdee.top/gtevkvtwjp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtbqhkjgks.html

Ruby: obj.instance_variables
来源：http://hz.andypj.xyz/gtkxhdprmy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cheryme.top/gtqdwhpwdq.html

================================================================================
来源：http://hz.sxryk.cn/gtrrjgetkc.html

H. 异常与错误处理
来源：http://hz.yangfankeji.com/gtoipxlnge.html

================================================================================
来源：http://hz.ehwqpu.com/gtxnzurbox.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtegixymdq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangdashe.top/gtigoyzmgb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gthgqlilrw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnxiangtu.top/gtqjbkvjfr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtksusyrik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtrjvrdfyg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtryihjnbu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.iojbl.cn/gthpjaqury.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.bjfxy.top/gtejjjyzzm.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gthhyrzidm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nwbrower.top/gtkozmfdlm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtstofetar.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtsfpasbap.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtlidavurg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtcaijxhtg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtgzswffms.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtmemjrmjh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.c1oappe.top/gtogcnqfis.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gticwnznuf.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtglwtcvzx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtppjlzaxn.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtmivnqftr.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtyankqbgc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.meibo888.top/gtntfqoewq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gtvqkmbpqu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtddqilqqk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtqnwfmtel.html

[H04] 自定义异常类型
来源：http://hz.xingfuxueyuan.xyz/gthycnfbxd.html

Py:   class MyError(Exception): pass
来源：http://hz.zhengqikj.top/gtnfgmewkp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtphacmlle.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtrqyenkif.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtxymqtque.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtvuwkuwux.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangdashe.top/gtszghcmbw.html

Ruby: class MyError < StandardError; end
来源：http://hz.zycfv.cn/gtdllvxxyz.html

C#:   class MyException : Exception {}
来源：http://hz.zhixingplan.top/gtztqwpknw.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtqvqclqvf.html

Py:   except ValueError as e:
来源：http://hz.cqqwz.cn/gtmpnygekq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtshgpcccp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtbagyrlxe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtzlbestzq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtkeoghpau.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yangfankeji.com/gtjqnctzbl.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinghuilouyu.cn/gtodumfwqo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtbiydlpud.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yangfankeji.com/gtlrfwbkjt.html

Py:   value = d.get("k") or default
来源：http://hz.ywan-chungtsiang.top/gtwxgsmbzs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gtcvqnmqrz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtkgmmomkp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtxkvlkuxz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.smart0.xyz/gtxjxkpriz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tianlin.xyz/gtddgplvxq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yangfankeji.com/gtbckfqvtd.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtkvlfueba.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtpdqiawen.html

Py:   assert x > 0, "必须为正"
来源：http://hz.mhx1999.top/gtdnhylpmu.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtywkudkvw.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtxwfgfuaz.html

TS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtogeyjmzb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gtvzcfrcem.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxinkj.top/gtwotrnzak.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yvedp.cn/gtrqagurik.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtsuceifdi.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj202588.top/gtwxlqquht.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cheryme.top/gtetsfohvv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gtviypfudy.html


<!-- 参考信息 -->