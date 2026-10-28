代发 wailian999

[F01] 读取整个文件
来源：http://hz.xziqi.cn/gtkyaduqjo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtejzxicmk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gtokxemswk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gteqmzmcdu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cashguo.top/gtqzszyfbp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtcjzeehql.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xylfe.cn/gtohbabcbz.html

Ruby: File.read("a.txt")
来源：http://hz.cucudq.cn/gthqixebdv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sufxvd.cn/gtxfwhrijg.html

[F02] 逐行读取文件
来源：http://hz.zhengqikj.top/gtxodtunbb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtemgraslh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gzhubu.top/gtziqvaxwr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtrvafjngw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtyjdvjsdd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtlflszvgq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtcoxkxroy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtyhodubce.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxinkj.top/gtoxzlarrh.html

[F03] 写入文件（覆盖）
来源：http://hz.zhiwuduotai.top/gthegryutj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtionkaoif.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aizwys.cn/gtdrjxyjdc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtaumwjshh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gttenuksnt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gtzltxrbuv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yonumen.top/gtekiodzui.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.c1oappe.top/gtrdyreimm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtoxcpebhe.html

[F04] 追加写入文件
来源：http://hz.andypj.xyz/gtspmursoj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtnwhuqvmd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.snrcjt.cn/gtqtxzargx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtlljxgook.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gttbusymtf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtiorpttuq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cashguo.top/gtfslsqyib.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gtjhwcfywr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtenesfekh.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtmyputdyd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtvskhvfuj.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gthdjshkqn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.vqdsnc.cn/gtgajigaso.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenzaomai.com/gtqtrpwiyn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtxgihxbvp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuanzx.com/gtghuhckku.html

Ruby: File.exist?("a.txt")
来源：http://hz.nwbrower.top/gtmiemgakg.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtzrmvheyt.html

[F06] 删除文件
来源：http://hz.fzhhl.top/gtyqucvshb.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtfjizyakc.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtdonlgjij.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gttsnqmcmu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtwkodmhyz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtfqkpbenb.html

Go:   os.Remove("a.txt")
来源：http://hz.yj20258.top/gtpkbyvjke.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtgutqmwmf.html

C#:   File.Delete("a.txt");
来源：http://hz.zhengqikj.top/gtjfdusyew.html

[F07] 创建目录（含多级）
来源：http://hz.pycfn.com/gtuottcvab.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.iojbl.cn/gtocydbtjk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gtwtorhxnw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtnvrqpfqp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtklenxbdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtfyouhqgx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gtdytbdnur.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj202588.top/gtqrnayyjy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.52xcode.cn/gtcmggjrza.html

[F08] 遍历目录
来源：http://hz.jinghuilouyu.cn/gttclyzfsi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtdjvjurvr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtzyxrxywn.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gteduapham.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtekuqnjsk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtgbchmhwi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtmzwfmtkg.html

Ruby: Dir.children("dir")
来源：http://hz.tanke756.top/gtxinowkyt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jiagoushi.top/gtrzzsarbn.html

[F09] 获取文件大小
来源：http://hz.xingfuxueyuan.xyz/gtamhpvwro.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gtlxxaciko.html

PHP:  filesize("a.txt");
来源：http://hz.andypj.xyz/gtzhjtrwyd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtdwfbxygp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtekzzmnrg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtseoocsav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fengsongda.top/gtvfbuvxrx.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtduzyuuix.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtxfglmiab.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtxtuikycw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtrdehkxvn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258888.top/gtqhdbsocc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gteldwljoc.html

TS:   path.extname("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtjdvsyrqv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtllxxuoru.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtwpmhcvld.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtwsrfodkp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gtnocrxwxr.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gtxmormbpz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtaaypajfb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhiwuduotai.top/gtxdtwghdk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtllgswjkp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtmqfdqoqu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtpzcmcsnd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtgdqedluq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtvweuvoqt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.havefunace.top/gtufagpcep.html

[F12] CSV 读写
来源：http://hz.zhijiandao.cn/gtgvrxewop.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtyblexxsz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.52xcode.cn/gtbngryajf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hywenlv.cn/gtddroeyfw.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtsbcmlgny.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.kuanghao11.cn/gtsjuksnxw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtewyhixtw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yueranfly.top/gtzocutzmh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jiagoushi.top/gtkjawfwwd.html

================================================================================
来源：http://hz.cqqwz.cn/gtetznulge.html

G. 面向对象
来源：http://hz.yj20258888.top/gtlinmnenm.html

================================================================================
来源：http://hz.hnqzz.top/gtatifmtfc.html

[G01] 定义类
来源：http://hz.sysykeji.top/gttcswonya.html

Py:   class User: pass
来源：http://hz.quarkkingdee.top/gteceyngos.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtxdwgkqfd.html

JS:   class User {}
来源：http://hz.c1oappe.top/gtsynybmxb.html

TS:   class User { name: string = ""; }
来源：http://hz.c1oappe.top/gtqfxtnzsu.html

Java: class User {}
来源：http://hz.jqgfzy.top/gttsuawexr.html

Go:   type User struct { Name string }
来源：http://hz.tanke756.top/gtrugattfh.html

Ruby: class User; end
来源：http://hz.yonumen.top/gttayflnei.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtshknwuvk.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtktitccru.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aizwys.cn/gtznbjaoub.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gteldmbchg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gthpeuflpm.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gtiobviwln.html

Java: User(String name) { this.name = name; }
来源：http://hz.tianlin.xyz/gthhmcbpxt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnqzz.top/gtexatafti.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shuidangran.top/gtvykjtzwd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtyvxrewfn.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtplfrfora.html

Py:   self.name = "x"
来源：http://hz.zycfv.cn/gtstuclrue.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtdeknqbin.html

JS:   this.name = "x";
来源：http://hz.ydzc1.top/gtwabjhirc.html

TS:   name: string = "x";
来源：http://hz.xingfuxueyuan.xyz/gtmkfglaox.html

Java: private String name;
来源：http://hz.hnqzz.top/gttvuexuyd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gtxnllukvr.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtydatrjdz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtaflevpul.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtoosfyfzh.html

Py:   def greet(self): return self.name
来源：http://hz.birdmap.top/gtvzmzksfu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtnipexczb.html

JS:   greet() { return this.name; }
来源：http://hz.ybcxt.top/gtvpaklfcu.html

TS:   greet(): string { return this.name; }
来源：http://hz.yonumen.top/gtxysnhqsl.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtctnycnkz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.wangdashe.top/gtgefwddsk.html

Ruby: def greet; @name; end
来源：http://hz.c1oappe.top/gtjkwdvxfy.html

C#:   public string Greet() => Name;
来源：http://hz.nanxinkj.top/gtccerkvil.html

[G05] 继承
来源：http://hz.aizwys.cn/gtzkkhtuqy.html

Py:   class Admin(User): pass
来源：http://hz.hongshengwenyu.top/gtcodlbhcn.html

PHP:  class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtiaifqcjk.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gthjdbbjis.html

TS:   class Admin extends User {}
来源：http://hz.hnqzz.top/gtokfrpylm.html

Java: class Admin extends User {}
来源：http://hz.hnqzz.top/gtmrrdulrp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhixingplan.top/gtsuljxelw.html

Ruby: class Admin < User; end
来源：http://hz.dashuyun.cn/gtcbqvizjy.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtnuqnzmkd.html

[G06] 重写方法
来源：http://hz.jlsjyb.cn/gtnqocnwpz.html

Py:   def greet(self): return "admin"
来源：http://hz.zhixingplan.top/gtanhqzqpv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtoiepcvxm.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtxwxaqvhy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtkgszvfft.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtknwefubs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenjidiqi.icu/gtwpcyohxb.html

Ruby: def greet; "admin"; end
来源：http://hz.xingfuxueyuan.xyz/gtvokuvznb.html

C#:   public override string Greet() => "admin";
来源：http://hz.0kj1m.cn/gtohziajjd.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtkhdalkag.html

Py:   super().greet()
来源：http://hz.yueranfly.top/gtvpdmuqpv.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtjpsenxbg.html

JS:   super.greet();
来源：http://hz.yueranfly.top/gtuseyvlqz.html

TS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtcgvxerov.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtezuheflb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgfzy.top/gtvfjfjjrp.html

Ruby: super
来源：http://hz.jyoumei.cn/gtsqdebxvr.html

C#:   base.Greet();
来源：http://hz.zdqjudy.top/gtvwbekpdr.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtlxxlblev.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.quarkkingdee.top/gtimorckxj.html

PHP:  public static function f() {}
来源：http://hz.cucudq.cn/gtpbbhsdpo.html

JS:   static f() {}
来源：http://hz.snrcjt.cn/gtfjwvlgiw.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gtqbkszcte.html

Java: static void f() {}
来源：http://hz.shanyushiyangkeji.top/gtizmpnxsh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xingfuxueyuan.xyz/gtyrifjicw.html

Ruby: def self.f; end
来源：http://hz.shuidangran.top/gtqnjfuctd.html

C#:   public static void F() {}
来源：http://hz.jinghuilouyu.cn/gtfszbhqjf.html

[G09] 接口 / 抽象类
来源：http://hz.jinqigufen.top/gtzecbcuxm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtbjtczpls.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtvljadbvx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtdowzwgze.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtseywoete.html

Java: interface Shape { double area(); }
来源：http://hz.yuxming.cn/gtoxbhvsbf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xinyue.icu/gtmfnczliu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtyrbcvlpd.html

C#:   interface IShape { double Area(); }
来源：http://hz.yonumen.top/gtmfejigum.html

[G10] 访问控制
来源：http://hz.zhengqikj.top/gtxpdujdnn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gtdtchfxwr.html

PHP:  public / protected / private
来源：http://hz.tanke756.top/gtactckspv.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtruaiakxz.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gtkjkurker.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtzddevppm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtxcqjeyri.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gthqyhlpxc.html

C#:   public / protected / private / internal
来源：http://hz.jianghu66.top/gthlcvvjpv.html

[G11] getter / setter
来源：http://hz.gaohongyu789.top/gtqmrgvfnr.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gtrqkvhada.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtzwqxasea.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtzgfzqlzt.html

TS:   get name(): string { return this._name; }
来源：http://hz.nwbrower.top/gtwqmhbfyh.html

Java: public String getName() { return name; }
来源：http://hz.yongpay.top/gtxvrwwgva.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtmgymujua.html

Ruby: attr_accessor :name
来源：http://hz.pengpengdd.cyou/gtkgqrltos.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtiomtglwn.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtpekenfhq.html

Py:   def __str__(self): return self.name
来源：http://hz.sysykeji.top/gtobjykkaq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtykvcexgc.html

JS:   toString() { return this.name; }
来源：http://hz.gzhubu.top/gtaruxonkn.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gttytmnxsh.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtfwypqccm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.havefunace.top/gtmjtmelyw.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtrzsscfoj.html

C#:   public override string ToString() => Name;
来源：http://hz.kuanghao11.cn/gtmrlzwujx.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtgmcpmobi.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gtmlkzshpf.html

PHP:  $u instanceof User
来源：http://hz.cashguo.top/gtahuwiino.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtwerbibqn.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtqjwehzga.html

Java: u instanceof User
来源：http://hz.tian-w.cn/gtslpprmvx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fzhhl.top/gtpnftxvcy.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtxjhdxyqd.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtfqgfmdqx.html

[G14] 数据类 / record
来源：http://hz.xinyue.icu/gtxodvfdqx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtomibbsqc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtdcxtfvda.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtdlwcefpo.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtnmphwpbx.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtegnjyvcm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.c1oappe.top/gtypfqnagf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtjuapadvz.html

C#:   record User(string Name, int Age);
来源：http://hz.yj202588.top/gtqjbmujkw.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtucsaojxd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhijiandao.cn/gtwwudcdzs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guannengcc.top/gtokltkqmz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pengpengdd.cyou/gtfkusgpib.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtshurszxk.html

Java: enum Color { RED, GREEN }
来源：http://hz.yueranfly.top/gtfjhrmarp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtqavuukze.html

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gtzvaudthq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtsgnrjsgg.html

[G16] 对象转数组 / 字典
来源：http://hz.xingfuxueyuan.xyz/gturnsykfk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtbucwlvry.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtvmmoueqr.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtnnhrppmb.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtenoisvwf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yanxiufei.cn/gtkcvcygrg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.birdmap.top/gtzraizzge.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gtkebzriql.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tanke756.top/gtogkivtut.html

================================================================================
来源：http://hz.cdnleiting.top/gtsfuvewhy.html

H. 异常与错误处理
来源：http://hz.jinyuanbaomall.cn/gtafgwlnmt.html

================================================================================
来源：http://hz.zhijiandao.cn/gttzuojjut.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gtvdkhgbzk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtrofuxmdt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.fzhhl.top/gtiupseoll.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.quarkkingdee.top/gthydgdcri.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.52xcode.cn/gtgxxhibum.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtcbgdynhp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuxming.cn/gtopuyvgzb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hammf.cn/gtvwrmzrnl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tian-w.cn/gtmulbrdel.html

[H02] finally / ensure 收尾
来源：http://hz.zhengqikj.top/gtizuofvfm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guannengcc.top/gtennqhdlf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtcljbxbqi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtejmchece.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtoogimflk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtapiecjsu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtmuyhciew.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gzhubu.top/gtepjzyula.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.52xcode.cn/gtxbsmiidc.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtcmtzqcrb.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gtzezxfqxy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtszqipxyt.html

JS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtvnslyvkc.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtmpvfumjw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtzmzjxcdc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gtxarvjivv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zycfv.cn/gttgcgmceq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtctvvzpsd.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtilrzynvf.html

Py:   class MyError(Exception): pass
来源：http://hz.hysaishi.cn/gtskdbjbtv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.iojbl.cn/gtxkyypnpy.html

JS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtkdnvysed.html

TS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gtwtnsmifv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ybcxt.top/gtemhhyhjv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dianchejie.cn/gtljuwigrx.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtsxbrhqws.html

C#:   class MyException : Exception {}
来源：http://hz.316326.xyz/gtfzbdbakp.html

[H05] 捕获特定类型
来源：http://hz.ywan-chungtsiang.top/gtdjkzivdj.html

Py:   except ValueError as e:
来源：http://hz.sweek.top/gtjrhevhrp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtkwndoeyi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtlwwvghcs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtkbiiwnop.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtoftehpot.html


<!-- 参考信息 -->