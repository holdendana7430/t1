代发 wailian999

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtqjdauokf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sufxvd.cn/gtxghogpnt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.316326.xyz/gtzdjimfmg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtagdaolhl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhiwuduotai.top/gtusyjhkfq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtcupdcwfw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtafmdyqwu.html

Ruby: File.read("a.txt")
来源：http://hz.guannengcc.top/gtzyjwniji.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nwbrower.top/gteiddhyyh.html

[F02] 逐行读取文件
来源：http://hz.yangfankeji.com/gtskpqqwew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtvsdyhohs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.c1oappe.top/gtbufhdvtr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigfzy.top/gtqgcqobos.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtusrfjzwc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtxqhabqzw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.wangdashe.top/gtakmxwzdl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuanzhike.top/gthrjibmnc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtqdpaqrhx.html

[F03] 写入文件（覆盖）
来源：http://hz.zycfv.cn/gtluasynqs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.316326.xyz/gtmzkimtxg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtvxmzlvzn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtjmhlcyso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtyizcqods.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtpncgvljy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtqygzpaoh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gtcfdmztbl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.0kj1m.cn/gttbcnqpvn.html

[F04] 追加写入文件
来源：http://hz.aibaodan.cn/gteypaajto.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gthjsxmeyk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgufenzy.top/gtitrhimoh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtvdyabelb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtpxxlfnmb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhixingplan.top/gtnhwgwsvb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.52xcode.cn/gtccctjmum.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangshuangyany.cn/gtblcgdpqz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pengpengdd.cyou/gtgwhnwths.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtypvppzxi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtqnvkvdrv.html

PHP:  file_exists("a.txt");
来源：http://hz.cdnleiting.top/gtekujrbjy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.havefunace.top/gtvoznoqca.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtlomakgoa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtpgblstvc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gthhypkkdx.html

Ruby: File.exist?("a.txt")
来源：http://hz.vqdsnc.cn/gtestegnyl.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtnyacqdmt.html

[F06] 删除文件
来源：http://hz.ybcxt.top/gtchbydesc.html

Py:   os.remove("a.txt")
来源：http://hz.gaohongyu789.top/gtbyppovlf.html

PHP:  unlink("a.txt");
来源：http://hz.yuanzhike.top/gtojaipcig.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtcepbydnp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtuvwjprtz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtxciwnzmc.html

Go:   os.Remove("a.txt")
来源：http://hz.xinyue.icu/gtebilqtpx.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtruhzpwph.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtwtufgjfx.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gthxdqgfwk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jiagoushi.top/gtmobmfysh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sufxvd.cn/gtjfquqprg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtmxsfuvgj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gtwpuqmssj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ivvv.top/gtruqazoux.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gotoacloud.top/gtnpgygxga.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.316326.xyz/gtxbwxozhl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gtwmviebht.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtloqkhgsj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtgsxrrown.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtzzbjqbox.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtjbxlhbeh.html

TS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtyhqlfewh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gttqnebqhk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtcwtblrjx.html

Ruby: Dir.children("dir")
来源：http://hz.quarkkingdee.top/gtctzyeagr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cqqwz.cn/gtwvxeuzji.html

[F09] 获取文件大小
来源：http://hz.sxryk.cn/gtyijkkdmz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtchryldpx.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigufen.top/gtbdzwqnny.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtkulrekyw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtziamrztr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtskwiutja.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.feifeiyinyue.top/gtfehhsqew.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtremxiysn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtpqemfckt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinyuanbaomall.cn/gtssixbncy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtxieujdct.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuanzx.com/gtocxtdwyn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtzabvscdh.html

TS:   path.extname("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtexbnbhyt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tian-w.cn/gtlepobsjz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuanzx.com/gtosldyndq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtrklqhilg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gtagofhiva.html

[F11] 复制与移动文件
来源：http://hz.nanxuanxn.top/gtcjcotmgy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtmmwsiyvs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.havefunace.top/gtlciobnyr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtwsbgetxm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtxwvihhqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtfmebsusg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.feifeiyinyue.top/gtqgcbartt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtzskxaftx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangtech.top/gtfnogaesl.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtmbuataqt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxuanxn.top/gtexmutaap.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtignoutzi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.haohaochexian.top/gtchxfhlvr.html

TS:   // 同上
来源：http://hz.aizwys.cn/gtzictfhuy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gtmllbzobo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gthhcsjsrs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydzc1.top/gtbjfjpccx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tian-w.cn/gtypfbwcmh.html

================================================================================
来源：http://hz.cqqwz.cn/gtkhootcnu.html

G. 面向对象
来源：http://hz.xziqi.cn/gtrqbcmuak.html

================================================================================
来源：http://hz.bjfxy.top/gtnweyhcol.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtuqhsifkd.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtvgdsowfn.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gthxkwxwye.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtdcndqctl.html

TS:   class User { name: string = ""; }
来源：http://hz.nwbrower.top/gtbgigztsd.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtyestszas.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtcrgkyzac.html

Ruby: class User; end
来源：http://hz.andypj.xyz/gtvqxfbphr.html

C#:   class User {}
来源：http://hz.redwolf501.top/gtfojylqgg.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gtrmcuxgzx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgufenzy.top/gtsmmftjlh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtocfhunbq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtyzadadwe.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxinkj.top/gtyyepnjoo.html

Java: User(String name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtcuwgfzoi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnqzz.top/gtgrdxawtv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtxowgigtf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.meibo888.top/gtorihmibl.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtxsgqvyga.html

Py:   self.name = "x"
来源：http://hz.sufxvd.cn/gtfthtjxbg.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gthugzieyr.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtrkxszfhr.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gthapgoxzd.html

Java: private String name;
来源：http://hz.sysykeji.top/gtkrzbvcyv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gtbuyxqngv.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gtuuitwqsr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zdqjudy.top/gtzdgkchpy.html

[G04] 定义方法
来源：http://hz.bjfxy.top/gtujtixjru.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtfnahvsww.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtejnkgioy.html

JS:   greet() { return this.name; }
来源：http://hz.xuanzx.com/gttufjpsiu.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gthfojgkzk.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtisbphfdx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtqcoqprrb.html

Ruby: def greet; @name; end
来源：http://hz.hnqzz.top/gthqaktovu.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gtxedjbhwp.html

[G05] 继承
来源：http://hz.zhixingplan.top/gtrjffokze.html

Py:   class Admin(User): pass
来源：http://hz.hongshengwenyu.top/gtljvrxkvj.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtaqoporhw.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gttdvpyyit.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtwevvdlsj.html

Java: class Admin extends User {}
来源：http://hz.andypj.xyz/gtefgutdae.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hysaishi.cn/gtpakywysb.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtpnmaoqsr.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gtbiqgaqhi.html

[G06] 重写方法
来源：http://hz.cdnleiting.top/gtlitmnmhq.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtzbtcazrw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtseqyrplr.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtivtulqtc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtoxcxaylk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtxvnxksnk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuetiantiany.cn/gtdimwjesk.html

Ruby: def greet; "admin"; end
来源：http://hz.birdmap.top/gtjnfiotrp.html

C#:   public override string Greet() => "admin";
来源：http://hz.aibaodan.cn/gtmzbqkoeh.html

[G07] 调用父类方法
来源：http://hz.yuxming.cn/gttxwcejoi.html

Py:   super().greet()
来源：http://hz.redwolf501.top/gtostpaesg.html

PHP:  parent::greet();
来源：http://hz.xuanzx.com/gtthcvttav.html

JS:   super.greet();
来源：http://hz.gotoacloud.top/gtjdhyyeqm.html

TS:   super.greet();
来源：http://hz.chenlongwang.top/gtmlroakvj.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtivmkcecy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.mhx1999.top/gtvyxhwybm.html

Ruby: super
来源：http://hz.nanxuanxn.top/gtbmkoelyi.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtnpjlzvpc.html

[G08] 静态方法与属性
来源：http://hz.feifeiyinyue.top/gtftmtpimc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gthymssifh.html

PHP:  public static function f() {}
来源：http://hz.c1oappe.top/gtifbctnke.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gttnkwczsb.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtjfpakxuy.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtwamccqbo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtiaqqzwej.html

Ruby: def self.f; end
来源：http://hz.dianchejie.cn/gtislualzg.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gtyvhsxscv.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtkndurlhp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtpxoxntuh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtancnisog.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydzc1.top/gtcpskwbjc.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtipuhcsrz.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gtstmsgeng.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtbqraqlmk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtcwqwvrqs.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtmitxjkak.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtiempmauy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtfbgneoav.html

PHP:  public / protected / private
来源：http://hz.feifeiyinyue.top/gtlxrpotra.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtkwzijqdj.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gtuanbvrqr.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtzookrdwj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhongyouzk.top/gteserxnte.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtmgazbfod.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gtnyglgqds.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gtkkzgzjov.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gthielkahh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtxqjnkygf.html

JS:   get name() { return this._name; }
来源：http://hz.jqgfzy.top/gtijwvssqm.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangshuangyany.cn/gtwpoxpsbu.html

Java: public String getName() { return name; }
来源：http://hz.zhongyouzk.top/gtckjhvjpk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nwbrower.top/gtdjexlhyd.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtowdamohf.html

C#:   public string Name { get; set; }
来源：http://hz.hysaishi.cn/gtfowoujpl.html

[G12] 对象转字符串
来源：http://hz.zhengqikj.top/gtzzkpovuv.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgufenzy.top/gtgeswgtgn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtzgpsemxq.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtnruawkai.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtgcwhfwnb.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtbahzujkw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sxryk.cn/gtimupmoxa.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtqcoipenk.html

C#:   public override string ToString() => Name;
来源：http://hz.havefunace.top/gtcawygtjl.html

[G13] 判断对象类型
来源：http://hz.snrcjt.cn/gtmxdjltna.html

Py:   isinstance(u, User)
来源：http://hz.0kj1m.cn/gtihhsattz.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gtqntpjfwh.html

JS:   u instanceof User
来源：http://hz.yuanzhike.top/gtjrvauraf.html

TS:   u instanceof User
来源：http://hz.cucudq.cn/gtnuhgvtoe.html

Java: u instanceof User
来源：http://hz.ybcxt.top/gtilpreouh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fzhhl.top/gtmttbvqcb.html

Ruby: u.is_a?(User)
来源：http://hz.kuanghao11.cn/gtahnthynq.html

C#:   u is User
来源：http://hz.dianchejie.cn/gtznwahcfm.html

[G14] 数据类 / record
来源：http://hz.yueranfly.top/gtndiknfmu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guannengcc.top/gtwjvawfix.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xylfe.cn/gtdnpymxzv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtrbjokzfh.html

TS:   type User = { name: string; age: number };
来源：http://hz.hywenlv.cn/gtkpgjfshs.html

Java: record User(String name, int age) {}
来源：http://hz.ydzc1.top/gttfrhxxml.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhengqikj.top/gtgfeopgyd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ehwqpu.com/gtnauskdpp.html

C#:   record User(string Name, int Age);
来源：http://hz.yvedp.cn/gtmssdzbyk.html

[G15] 枚举
来源：http://hz.havefunace.top/gtundbhkky.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinghuilouyu.cn/gtqqqaxyat.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gtuhtkyufo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtighbwmqf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtljdmuoyg.html

Java: enum Color { RED, GREEN }
来源：http://hz.hywenlv.cn/gtvraolsnk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtjzzsgwmo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.haohaochexian.top/gttujlnpbl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtgztsvcsl.html

[G16] 对象转数组 / 字典
来源：http://hz.jiagoushi.top/gttgeyuzmb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtecfzfkjr.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtqkguiaes.html

JS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtzedfaoiv.html

TS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtifhuolng.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtbxcmvwqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtdbbtxhel.html

Ruby: obj.instance_variables
来源：http://hz.birdmap.top/gtermhxsmf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gtpherodhd.html

================================================================================
来源：http://hz.zhengqikj.top/gtlopgxxrl.html

H. 异常与错误处理
来源：http://hz.zycfv.cn/gtvrblgmkc.html

================================================================================
来源：http://hz.svipenyu.cn/gtkiwcabww.html

[H01] try / catch 基础
来源：http://hz.haohaochexian.top/gtgmadhenh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gtptnjkisu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtnuiijbcg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtetwhjtti.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gttcvvszgj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gtgdpxhxkc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtlqklzanc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnqzz.top/gtehzznkeq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sweek.top/gtvynbjwsh.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gtnnaxwvsj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shuidangran.top/gteyrpbxxw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtqullhikb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtrznfaahl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtgdlxyrnm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtwewweifi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtbawhaonl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sysykeji.top/gtzeyoqqmp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gtesnpshmj.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gtlysyvcpv.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gtaefnmbgb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtexnjebbs.html

JS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtmiiakkuu.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gttasihhju.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtrovvvkze.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtwwayqifp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shzxlz.cn/gtoihvebui.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtqwpyntzf.html

[H04] 自定义异常类型
来源：http://hz.hongshengwenyu.top/gtcnochzxh.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtjdzmylnk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangdashe.top/gtkhhnmcoc.html

JS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtudrcxdbq.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gttwxkgwom.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtowlyatlr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangtech.top/gtbxgtiupq.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgfzy.top/gtvxbeexye.html

C#:   class MyException : Exception {}
来源：http://hz.xylfe.cn/gtppujlmhr.html

[H05] 捕获特定类型
来源：http://hz.jqgufenzy.top/gtehhpvdpm.html

Py:   except ValueError as e:
来源：http://hz.xylfe.cn/gtfiknqehr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtgzndjokl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtzaovxawj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtlfducfpk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtkbykbseq.html


<!-- 参考信息 -->