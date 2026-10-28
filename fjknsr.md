代发 wailian999

[F01] 读取整个文件
来源：http://hz.ydjk.org.cn/gtendtgefw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zycfv.cn/gtbsnayawx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sweek.top/gtimyjyrtf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gttlnqzdbg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.havefunace.top/gtefmkbbjm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtiruxwyaj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtighwqael.html

Ruby: File.read("a.txt")
来源：http://hz.9152youxi.cn/gtpdwzyvcf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xziqi.cn/gtttzgcbin.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gtyviewytr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cucudq.cn/gtbjqzseos.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.redwolf501.top/gtddounuwo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtzepkeamw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gttzxpsnxv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtujcldmqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gtcminjpsi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cheryme.top/gteqdkwdwo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnqzz.top/gtdvyfyivl.html

[F03] 写入文件（覆盖）
来源：http://hz.feifeiyinyue.top/gteorsxgge.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258888.top/gtmsostbtb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tian-w.cn/gttfnxcvuv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtgpvpuona.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gttqkaqike.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuanzx.com/gtmosxuutp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.guannengcc.top/gtazdyocou.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtonwseazp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258888.top/gtmsvzrylh.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gteltfqgif.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cdnleiting.top/gtrgqfxiak.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pycfn.com/gtinlzcjhi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtprxmsmez.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hysaishi.cn/gtkkyjtlkz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.quarkkingdee.top/gtjtbjxmri.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtwlbukguz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gthvnsckgv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtexsbbjnn.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtvyxfwkdn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.wangdashe.top/gtylinvqjt.html

PHP:  file_exists("a.txt");
来源：http://hz.kuanghao11.cn/gtonropgut.html

JS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtqwvczyfi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtqgkqldxr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtoikqjaxv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigfzy.top/gtetqtqcks.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigfzy.top/gtukgtddyr.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gtvnvcryam.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtaucbyqfd.html

Py:   os.remove("a.txt")
来源：http://hz.pycfn.com/gtbbvkzivh.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtjoqylovp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtggcqbulb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtvlviibbt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtbehvrlpz.html

Go:   os.Remove("a.txt")
来源：http://hz.zhijiandao.cn/gtpejwcnto.html

Ruby: File.delete("a.txt")
来源：http://hz.zhixingplan.top/gtkimhuqel.html

C#:   File.Delete("a.txt");
来源：http://hz.zycfv.cn/gtfrbdlrma.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258.top/gtdcwakavg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.meibo888.top/gtyqcgojht.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhixingplan.top/gtzibdxpba.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtzeexffxs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtekywmfvp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtjomqqjef.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.meibo888.top/gtooxdxjxw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydzc1.top/gttayzggtf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gaohongyu789.top/gtlsrewimu.html

[F08] 遍历目录
来源：http://hz.nwbrower.top/gtfpsgyfiu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yangfankeji.com/gtccptgcvg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtfknxfcum.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtjsenlkrj.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtmptjzngi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtciyrsxez.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xuetiantiany.cn/gtpahwxmuo.html

Ruby: Dir.children("dir")
来源：http://hz.iojbl.cn/gtptosrvvu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtthhbsjpm.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtfhxiqewi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gtpbzzyvzn.html

PHP:  filesize("a.txt");
来源：http://hz.sufxvd.cn/gtkgwyacaq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtageibmbh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtvdwopnia.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtutejvucp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj202588.top/gtbmgfzxfz.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtxrqtcrlq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuxming.cn/gtmpexhvdg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtjfxrstjo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtqgpuvbet.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daxiang520.top/gtxcvobpgj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtajhorrar.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gtsblhqitp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtvmdkgkfg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtdeivcxjq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtlrengkqb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtvzhkslhc.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtfzfcyclm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtqkcomeip.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ehwqpu.com/gtkwkbiwlf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtghokmwcx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtivfhkdwo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenjidiqi.icu/gtkrwobmhn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtzwnqzazt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtzsteqbne.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgufenzy.top/gtdoggigkh.html

[F12] CSV 读写
来源：http://hz.hongshengwenyu.top/gtovysyldn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yanxiufei.cn/gtcoyxqeeq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shzxlz.cn/gtakzgpiml.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gtrxokyoey.html

TS:   // 同上
来源：http://hz.xuanzx.com/gtiffqhnyw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hammf.cn/gtmxtpoixz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.havefunace.top/gtxqssxxjf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinyuanbaomall.cn/gtkmdsrsxe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fzhhl.top/gtydvqkfzu.html

================================================================================
来源：http://hz.cashguo.top/gtwbxxgjfw.html

G. 面向对象
来源：http://hz.bjfxy.top/gtsuqwvcbm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtzcgcbwth.html

[G01] 定义类
来源：http://hz.fzhhl.top/gtfkgezyaf.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtabpkqrix.html

PHP:  class User {}
来源：http://hz.hnxiangtu.top/gtattccvkh.html

JS:   class User {}
来源：http://hz.0kj1m.cn/gtqrbiqtll.html

TS:   class User { name: string = ""; }
来源：http://hz.shzxlz.cn/gteflikpft.html

Java: class User {}
来源：http://hz.aizwys.cn/gtfnphrggm.html

Go:   type User struct { Name string }
来源：http://hz.yongpay.top/gtohxhgodz.html

Ruby: class User; end
来源：http://hz.jianghu66.top/gtcrpgppin.html

C#:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtrxoqoyqb.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtovakswwk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtatedsemp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.316326.xyz/gthgghwrqc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj202588.top/gtxalrxqnr.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtadeyrewq.html

Java: User(String name) { this.name = name; }
来源：http://hz.ybcxt.top/gtpyijbuhw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tian-w.cn/gttggknpbw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gttgiowpqc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gturyuewiv.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gticqfzgvi.html

Py:   self.name = "x"
来源：http://hz.hongshengwenyu.top/gtrgeiznfv.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtkvfnrasc.html

JS:   this.name = "x";
来源：http://hz.yj202588.top/gtvegntofg.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtoybkvylb.html

Java: private String name;
来源：http://hz.ehwqpu.com/gtjzmjduqz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhiwuduotai.top/gtodwjwift.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gtmzstuhik.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xziqi.cn/gtrkryvgif.html

[G04] 定义方法
来源：http://hz.haohaochexian.top/gtacoaezmy.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtxeubhuev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtrnjguqmf.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtmzsecxfe.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtuwkjxldp.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtgntffgxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtburncfud.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gtwficssyc.html

C#:   public string Greet() => Name;
来源：http://hz.cheryme.top/gtrcuidmcp.html

[G05] 继承
来源：http://hz.shuidangran.top/gtsnxkvryi.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtesfwpebb.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtugxldohh.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtmwhfmfgt.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtnzweaqgy.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtdhcdrtya.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtgkqodbnw.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtuzpbwknu.html

C#:   class Admin : User {}
来源：http://hz.shanyushiyangkeji.top/gtxhfygkfn.html

[G06] 重写方法
来源：http://hz.ydzc1.top/gtzvgebdqo.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258.top/gtqoayzgop.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtmiwucjcp.html

JS:   greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtmzpjszxq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtactsweaa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtkilzmgxw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxuanxn.top/gtjqhefdmr.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtpbgjklpc.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtcscsofva.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtszpxvbcb.html

Py:   super().greet()
来源：http://hz.tianlin.xyz/gtkmecaajo.html

PHP:  parent::greet();
来源：http://hz.tianlin.xyz/gtvfjdhkzf.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtqmszpveo.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtidltvzwj.html

Java: super.greet();
来源：http://hz.zhixingplan.top/gtpqdbwygk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangdashe.top/gtrxtebdae.html

Ruby: super
来源：http://hz.havefunace.top/gtijeofgec.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtnekcldeh.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gtjzjdtjjt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.52xcode.cn/gtraumasgn.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtceilmtxa.html

JS:   static f() {}
来源：http://hz.pycfn.com/gtxihkittv.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtsqhayxvi.html

Java: static void f() {}
来源：http://hz.xinyue.icu/gtemocvque.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guowangkeji.top/gtslyzvnvp.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtzdcdzjem.html

C#:   public static void F() {}
来源：http://hz.ppjwa.cn/gtpikjpixa.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtgllrkdmn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xinyue.icu/gtwwajgtmc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtyyxmthtz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinghuilouyu.cn/gtohuxwqsp.html

TS:   interface Shape { area(): number; }
来源：http://hz.xziqi.cn/gtkhfhynzs.html

Java: interface Shape { double area(); }
来源：http://hz.jqgfzy.top/gtnrpobcky.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tian-w.cn/gtdjyahxmt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtxaxosaiq.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gtipcosphx.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtgdlamhrw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fengsongda.top/gtucnenhgi.html

PHP:  public / protected / private
来源：http://hz.xuanzx.com/gtnyyrhxgx.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtxcdpcdqy.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gtnbdiabnk.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtnabpmojv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daria6918.cn/gtdlvydvab.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtpdgrchiy.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtwcndmduj.html

[G11] getter / setter
来源：http://hz.ybcxt.top/gtvwmwoonw.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtegwtdtuf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtzuqzzjvi.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtdrwmtsty.html

TS:   get name(): string { return this._name; }
来源：http://hz.aizwys.cn/gttvxlexwm.html

Java: public String getName() { return name; }
来源：http://hz.jinqigufen.top/gtoukdcgof.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yvedp.cn/gtrgdrxsts.html

Ruby: attr_accessor :name
来源：http://hz.zhixingplan.top/gtskduntte.html

C#:   public string Name { get; set; }
来源：http://hz.hnqzz.top/gttfowltcx.html

[G12] 对象转字符串
来源：http://hz.jinqigufen.top/gttzyqqmiz.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtansfcxhi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtzpwpxrxn.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtqbqgrfem.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtqzzdhxmf.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtbnepsbmb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ivvv.top/gtssxygoel.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtcgfgtrra.html

C#:   public override string ToString() => Name;
来源：http://hz.gzhubu.top/gtwnqzabwh.html

[G13] 判断对象类型
来源：http://hz.yonumen.top/gtpxfqvlqm.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gttxvkojno.html

PHP:  $u instanceof User
来源：http://hz.yj202588.top/gtssyejkwd.html

JS:   u instanceof User
来源：http://hz.gogol.net.cn/gtibvyqjqq.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gttztnvzle.html

Java: u instanceof User
来源：http://hz.tian-w.cn/gtkbiwngsc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gzhubu.top/gtrtxzvlus.html

Ruby: u.is_a?(User)
来源：http://hz.redwolf501.top/gtihyosuqy.html

C#:   u is User
来源：http://hz.tanke756.top/gtrqjlrwyp.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtipttwoqo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtzhlqqqun.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sysykeji.top/gtpsuwzzii.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtpeqrmwdo.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuetiantiany.cn/gteczelhng.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtexbdjkov.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnqzz.top/gttfsoafry.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gtllppadye.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtzatgulwk.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtuopahgio.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aibaodan.cn/gtqjuhtqqn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtgkzjahuc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hammf.cn/gtvdqxxmji.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtqokholny.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtlgrnzsmh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ywan-chungtsiang.top/gttvyjrrca.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ybcxt.top/gttoparoip.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtwvdrpezl.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtbfhtktva.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtqvfdamrs.html

PHP:  get_object_vars($obj);
来源：http://hz.xinyue.icu/gtdvvdvudj.html

JS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtukdmrluh.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtzufdzskv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtatgcmqhk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtqmoftmvj.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtwypbpxqc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.bjfxy.top/gtmgxcwecb.html

================================================================================
来源：http://hz.cdnleiting.top/gtdygabzkr.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gtzlefdrqe.html

================================================================================
来源：http://hz.sufxvd.cn/gtrcywoprg.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtdrjcowyw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yvedp.cn/gtejbratfu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtgqehgcls.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtzzhwjpck.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtjttuwedo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shuidangran.top/gtbspifjcv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtgljxrswd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtjdvuyoob.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtmowuniip.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gtndnulwef.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtzuhxmbvk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtziiqghfs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtbtryctxc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtwwshjhnm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gthhxdmxyh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guowangkeji.top/gtpsfokfon.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtbfebttyo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yanxiufei.cn/gtlarnnqfz.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtpisqupoc.html

Py:   raise ValueError("错误信息")
来源：http://hz.jianghu66.top/gtgjpaoawh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gthmxlnsbi.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtiwoarqad.html

TS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gttvvzyvbt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtntzlsifv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtuiauudou.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinghuilouyu.cn/gtfsyopjjs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtzfdvvtar.html

[H04] 自定义异常类型
来源：http://hz.guowangkeji.top/gtvhrbpqud.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtypwtepqo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtrjwznwwj.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtnstszwim.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtcifxjrpi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtuxkfebys.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhoulong.xyz/gtcffcdftp.html

Ruby: class MyError < StandardError; end
来源：http://hz.cqqwz.cn/gtvlzvtctb.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gtrvshobqv.html

[H05] 捕获特定类型
来源：http://hz.chenlongwang.top/gtwrmcmvnv.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtzvsmxjiy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtovxrjpnj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtuddgffhf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtnyruleun.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fzhhl.top/gtvculnkxg.html


<!-- 参考信息 -->