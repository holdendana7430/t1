代发 wailian999

[F01] 读取整个文件
来源：http://hz.wangdashe.top/gtycbmizsj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ydzc1.top/gtnaekcmbn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.bjfxy.top/gtfussyprr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtkntcvayf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.aizwys.cn/gttbnsllci.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtujzcjsgd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuxming.cn/gtisurngmw.html

Ruby: File.read("a.txt")
来源：http://hz.nanxinkj.top/gtqpsjiadd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenjidiqi.icu/gtzwsjzytd.html

[F02] 逐行读取文件
来源：http://hz.havefunace.top/gtjvclchcm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtyidjkmeg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangshuangyany.cn/gtcvxarynq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtjokjdkwf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtbeguzymh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtjhsowhis.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnxiangtu.top/gtpozafzfh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtyyssnjor.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nwbrower.top/gtsbcpfcnt.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtlwytkamr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtfacbclku.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydzc1.top/gtgnzyjtmn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtpbywxnhx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtauxsklkd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.redwolf501.top/gtprmpvuaz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtlizasgjo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xylfe.cn/gtgzojtzeu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtlfapjphf.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtzjguudpr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtdkseaqrq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtmclexrge.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtaibxgwbc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtytoykxsl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtwlpcupxj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtjwtwulew.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258888.top/gtxlipmpou.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtsclocxbd.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtmutgsnzq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tianlin.xyz/gtitvixinj.html

PHP:  file_exists("a.txt");
来源：http://hz.cucudq.cn/gtubirvwuy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtyetngfly.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtojeqhqym.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtcjqiqtlm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtbmtqetpg.html

Ruby: File.exist?("a.txt")
来源：http://hz.gzhubu.top/gtbhocyupu.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtpspsnemh.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtfvpmciep.html

Py:   os.remove("a.txt")
来源：http://hz.yj202588.top/gtnfmmihnx.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gthlntjeal.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtnmitlsuu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtotvjdoxy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtpyyqlzxa.html

Go:   os.Remove("a.txt")
来源：http://hz.iojbl.cn/gttbkrazbh.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtwfrepxll.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gtkezaljzz.html

[F07] 创建目录（含多级）
来源：http://hz.daria6918.cn/gticqhzyhx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jiagoushi.top/gthcxdsbfs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtpukveasx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtptpjnkji.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtxrklxplb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pengpengdd.cyou/gtljndqiid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gtnsiojmsv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtiisyjezs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zycfv.cn/gtjqzvdidr.html

[F08] 遍历目录
来源：http://hz.iojbl.cn/gtvvyjogmo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gtcsfwqmel.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gtyyirxauv.html

JS:   fs.readdirSync("dir")
来源：http://hz.xziqi.cn/gtuxbtgfnw.html

TS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtvahijyyu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtxixfwwuw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.316326.xyz/gtdngvfhau.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtkivddyhn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.feifeiyinyue.top/gtqfwlxjti.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtubbibqkg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtzptyehcn.html

PHP:  filesize("a.txt");
来源：http://hz.yj202588.top/gthuowpwfz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtemmqmkll.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gttvjbpxkn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtyhlqqsth.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.bjfxy.top/gttqyfmszr.html

Ruby: File.size("a.txt")
来源：http://hz.cqqwz.cn/gtkhnxoplc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hongshengwenyu.top/gtyekcaovb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gtvlbjnkyh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtwbdtdcil.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dianchejie.cn/gtevqeyjva.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtjxlsijwf.html

TS:   path.extname("a.txt")
来源：http://hz.yvedp.cn/gtlwjvppai.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fzhhl.top/gtafrbqeqc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cheryme.top/gtlsbtphrw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gtfydzkksj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtbmlggyht.html

[F11] 复制与移动文件
来源：http://hz.wangdashe.top/gtjffzmhfg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtxjwxprjh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258888.top/gtjwaluhda.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtdwspzlot.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtaomswycf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtvkyexcry.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtpaprcxew.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtutuaotfv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gtkyrsbnar.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtblkmbroc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yanxiufei.cn/gtjjywyekj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ppjwa.cn/gtuddxlula.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtzamnecan.html

TS:   // 同上
来源：http://hz.aibaodan.cn/gtyszznmdb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydjk.org.cn/gthyzavodb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtjhtsnzcr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gttitzdnsl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sysykeji.top/gtcqemvjpj.html

================================================================================
来源：http://hz.52xcode.cn/gtmfkcykxo.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtmdgdndwp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtixjrlbwm.html

[G01] 定义类
来源：http://hz.sweek.top/gtvddkobqr.html

Py:   class User: pass
来源：http://hz.ybcxt.top/gtmrgmwwys.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtntboyclw.html

JS:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtijvjnrog.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gtpeyqxhtf.html

Java: class User {}
来源：http://hz.redwolf501.top/gtszaqvzoj.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtfvujitck.html

Ruby: class User; end
来源：http://hz.yonumen.top/gtryzpxjzu.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtedbnmsgo.html

[G02] 构造函数
来源：http://hz.aizwys.cn/gtfyehiaoe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgufenzy.top/gtgbhguoyj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtoywjogng.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jianghu66.top/gtkrxxclpk.html

TS:   constructor(public name: string) {}
来源：http://hz.cucudq.cn/gtfvgoxfzd.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtxjtmrdfo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ehwqpu.com/gtdyxdohdr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtbfftvchv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daxiang520.top/gtirqfbvma.html

[G03] 实例属性
来源：http://hz.xingfuxueyuan.xyz/gtvijygnct.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtnbodetla.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtzjhrxbhj.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtcffqmwof.html

TS:   name: string = "x";
来源：http://hz.yonumen.top/gtykolmwdn.html

Java: private String name;
来源：http://hz.yj20258.top/gtvjcupudl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gtfatnkfom.html

Ruby: @name = "x"
来源：http://hz.birdmap.top/gtituuyvui.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dashuyun.cn/gtibgdtfjt.html

[G04] 定义方法
来源：http://hz.dianchejie.cn/gtxkznfmse.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtxbjvzmfs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtslevbeyb.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtktlprfzz.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtsvgvjlrg.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtcxugfzhz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtuticejlc.html

Ruby: def greet; @name; end
来源：http://hz.cqqwz.cn/gtraywgukf.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtdzzdpjfz.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtsldoyydh.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gttvzkaslq.html

PHP:  class Admin extends User {}
来源：http://hz.redwolf501.top/gtxzxsujzf.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtuxqekzpd.html

TS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtqxkyumql.html

Java: class Admin extends User {}
来源：http://hz.svipenyu.cn/gtdkttavrp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtexbcpfjs.html

Ruby: class Admin < User; end
来源：http://hz.jiagoushi.top/gtsmdvbbtz.html

C#:   class Admin : User {}
来源：http://hz.kuanghao11.cn/gtmqqomqql.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtglgrrlyt.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtjqjrnxmx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtciotglie.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtimubuhso.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtixcyqmwb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtpnqfptop.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtgehbbptv.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gttkkxquds.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtgmjebofp.html

[G07] 调用父类方法
来源：http://hz.sysykeji.top/gtccwtdebt.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtoylcwlro.html

PHP:  parent::greet();
来源：http://hz.chenjidiqi.icu/gtbhstkufa.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gthinrctos.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gtbbkombil.html

Java: super.greet();
来源：http://hz.feifeiyinyue.top/gtpvlouoep.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cashguo.top/gthiolzhtk.html

Ruby: super
来源：http://hz.yangfankeji.com/gtxytbuhbe.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtjwqpfwpj.html

[G08] 静态方法与属性
来源：http://hz.jinghuilouyu.cn/gtygtrziet.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.svipenyu.cn/gtmxjrlwws.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtguilaofz.html

JS:   static f() {}
来源：http://hz.jinyuanbaomall.cn/gttawhhzyh.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gtrqcpulzg.html

Java: static void f() {}
来源：http://hz.zhoulong.xyz/gtiacuujbx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.iojbl.cn/gtbvoxijhr.html

Ruby: def self.f; end
来源：http://hz.shuidangran.top/gtoudtmkro.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gtrxcdrnfk.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtvsyakptu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tianlin.xyz/gthnthxtls.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gtylikpsox.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ywan-chungtsiang.top/gtjclvjmbj.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gthftqlpqs.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtkckedhvn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgfzy.top/gtuepwxvpl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtnrzmdehq.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenjidiqi.icu/gtscqckdcy.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtfoebuuxo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hongshengwenyu.top/gtyfbjygoo.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtjjypvpts.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtlpggnmmt.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtcfikymxv.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gttirckryp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hysaishi.cn/gtshpqraii.html

Ruby: public / protected / private
来源：http://hz.xziqi.cn/gtlxusjsai.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtwlmnryza.html

[G11] getter / setter
来源：http://hz.yvedp.cn/gtjseohjea.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtidtrhowz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ivvv.top/gtntbpalfa.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtjdcxauwf.html

TS:   get name(): string { return this._name; }
来源：http://hz.tianlin.xyz/gtogaojdxw.html

Java: public String getName() { return name; }
来源：http://hz.jinqigfzy.top/gthmfzdrlp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtsaiqudtj.html

Ruby: attr_accessor :name
来源：http://hz.hnqzz.top/gtztaxttqy.html

C#:   public string Name { get; set; }
来源：http://hz.chenzaomai.com/gtloeftrdk.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtnuzhfibb.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtpfiwozai.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtmgshejmo.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtmqlbwblk.html

TS:   toString(): string { return this.name; }
来源：http://hz.wangdashe.top/gtwaihcbjv.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gtrrcnsggm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guannengcc.top/gtbwcropwx.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gtorszjwtb.html

C#:   public override string ToString() => Name;
来源：http://hz.chenzaomai.com/gtxqhwsfij.html

[G13] 判断对象类型
来源：http://hz.yonumen.top/gtxlwvfxdv.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtiewuldck.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtitgpoahb.html

JS:   u instanceof User
来源：http://hz.xuetiantiany.cn/gtfhlgmrwy.html

TS:   u instanceof User
来源：http://hz.daxiang520.top/gtazbonxya.html

Java: u instanceof User
来源：http://hz.quarkkingdee.top/gtofogklzx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj202588.top/gtltkcnvxd.html

Ruby: u.is_a?(User)
来源：http://hz.aizwys.cn/gtkbuycmwr.html

C#:   u is User
来源：http://hz.andypj.xyz/gtvijgkacd.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gttmgdixyl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtmczmndca.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.316326.xyz/gtmclpgygg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtvhyxwrhk.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtvbxbruwd.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtjzlpwnbm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gteawuwwoc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtpocvqufh.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtzjjlbzjp.html

[G15] 枚举
来源：http://hz.ydzc1.top/gteycnovdu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gttflpmgtk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yangfankeji.com/gtynsfkvwc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtyvlszhdf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gteaiwpkib.html

Java: enum Color { RED, GREEN }
来源：http://hz.hongshengwenyu.top/gtvgjxzpgu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cashguo.top/gtcgjasbcw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gtghnbnzud.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtccukuiwn.html

[G16] 对象转数组 / 字典
来源：http://hz.jiagoushi.top/gtvnikqpae.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pycfn.com/gtrnitjxqw.html

PHP:  get_object_vars($obj);
来源：http://hz.jyoumei.cn/gtsfhwprpt.html

JS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtwwzzvruv.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtsocsnpcs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtdgicfjxa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtladbancu.html

Ruby: obj.instance_variables
来源：http://hz.wangshuangyany.cn/gtjotbrffb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gtsbkxhyiw.html

================================================================================
来源：http://hz.xziqi.cn/gtodeqsvvt.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtnxixqvfu.html

================================================================================
来源：http://hz.jqgfzy.top/gtyhkpiviz.html

[H01] try / catch 基础
来源：http://hz.birdmap.top/gtcowhawuc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gttyimqoit.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gthrcurmbf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtqiauaunb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtwsghyexj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xingfuxueyuan.xyz/gtvcmkrphu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shangyingyoupin.top/gtyvhotbjp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtydkfrvac.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtvugvsrsq.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtokrrfnju.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhaomingkeji.xyz/gtgxnzfldq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtgjueexsh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtfvvzisct.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtviukpsel.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtnsdhcwyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xinyue.icu/gtvyivglsx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj202588.top/gtvtojdyuu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ppjwa.cn/gtpyvnnbqe.html

[H03] 主动抛出异常
来源：http://hz.ywan-chungtsiang.top/gtuipdvhyq.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtqgwttcbw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtwafuqmsm.html

JS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtgnxfnuoj.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtkuhwoncx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtiojwqskw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuetiantiany.cn/gtweramzzu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ivvv.top/gtnbznvnxu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtkrcainif.html

[H04] 自定义异常类型
来源：http://hz.snrcjt.cn/gtexofvapr.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtoytfjakq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtviqruwtg.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtwzuelnvi.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtcxxgbmjc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yvedp.cn/gtigcrjyvp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtuqdiqdvh.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj20258.top/gtfmxwrntd.html

C#:   class MyException : Exception {}
来源：http://hz.ybcxt.top/gtcbxvbvad.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gteldumjgv.html

Py:   except ValueError as e:
来源：http://hz.jinqigfzy.top/gtamlnbcza.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jianghu66.top/gtzvyslokb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtelnzyuza.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtkvqwkqty.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtomyxuvnq.html


<!-- 参考信息 -->