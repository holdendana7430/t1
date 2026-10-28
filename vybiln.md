代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtydyzrbzj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtuqkumjrc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtrkbaklgy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cucudq.cn/gtzrlewahj.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtmmovwbxu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtyoxhrbeh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtcrbpcrxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtpfxqftng.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtnqgrulss.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhengqikj.top/gtahlndlqn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.quarkkingdee.top/gthfuacubs.html

Ruby: s.bytesize;  s.length
来源：http://hz.hammf.cn/gtqegjxwlw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtbkzcsfus.html

================================================================================
来源：http://hz.cashguo.top/gtfijtnxcd.html

F. 文件与目录
来源：http://hz.ybcxt.top/gtvxhzsusa.html

================================================================================
来源：http://hz.hywenlv.cn/gtrypflmeb.html

[F01] 读取整个文件
来源：http://hz.gaohongyu789.top/gtzmgpvrmz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.svipenyu.cn/gtkixgbabx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gtxcowvbhz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shuidangran.top/gtjcjjjyih.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtmambcdye.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtwyyzidfq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtjgdlbawb.html

Ruby: File.read("a.txt")
来源：http://hz.yangfankeji.com/gtrdkunjjk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hysaishi.cn/gtfiaiusjj.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtiahlpkrg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dianchejie.cn/gtemszntzx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.haohaochexian.top/gtimxieotu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtzqrmnrsj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtcqfoqotd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtaffqxudl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gthksmosei.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtevifyfzk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shzxlz.cn/gtlylifmjf.html

[F03] 写入文件（覆盖）
来源：http://hz.tian-w.cn/gtyogpwrbf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gogol.net.cn/gtmbcqvowx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gthhznlkye.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtejuqkveb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gthzktldpr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtccachety.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jyoumei.cn/gtspdxamiw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jyoumei.cn/gtuvuzmzrr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtzoojmdxj.html

[F04] 追加写入文件
来源：http://hz.daxiang520.top/gtuhykjydo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ybcxt.top/gtxnzkjmod.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gteztcqktu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtdgykvmth.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtauafrzbh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtvnmzcmys.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daria6918.cn/gteympahjv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtnqownvwy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtpogmgzrv.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtleihdahj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dianchejie.cn/gtglivuzoj.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtqnlchbot.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtjtmzjqfp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtxymjhkyt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtarfuenve.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hongshengwenyu.top/gtoydcxfcy.html

Ruby: File.exist?("a.txt")
来源：http://hz.quarkkingdee.top/gtvpnzhisa.html

C#:   File.Exists("a.txt")
来源：http://hz.hammf.cn/gteogjsliz.html

[F06] 删除文件
来源：http://hz.yj20258888.top/gttyqzixaw.html

Py:   os.remove("a.txt")
来源：http://hz.jianghu66.top/gtziqgyfye.html

PHP:  unlink("a.txt");
来源：http://hz.sweek.top/gthsgabwuf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtxcovkmlo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtxiuvdtcm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtdvyvtidr.html

Go:   os.Remove("a.txt")
来源：http://hz.shzxlz.cn/gtxakbyouw.html

Ruby: File.delete("a.txt")
来源：http://hz.yj202588.top/gtkgtjtped.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtwpwilrbe.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258888.top/gtjsmcgxwi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.andypj.xyz/gtvkapfrfu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gttaitexjy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gttmotflqp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtmewosoco.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinyuanbaomall.cn/gtvssleypp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtgomeypcu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnxiangtu.top/gtejejdzgv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gtgegplein.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtztrnbpvk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtstolabxl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gogol.net.cn/gtqfaieosf.html

JS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtyqgygfge.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtsqumsugc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtqurxicpm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtrvuhebjd.html

Ruby: Dir.children("dir")
来源：http://hz.mhx1999.top/gtcxtovmve.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtjtscojlj.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gttgvpmdqt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sysykeji.top/gturlvtcaf.html

PHP:  filesize("a.txt");
来源：http://hz.cheryme.top/gtkuqixkij.html

JS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtqzxileqv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangshuangyany.cn/gtbwqvklqr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtwyiispju.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhiwuduotai.top/gtczskjvgl.html

Ruby: File.size("a.txt")
来源：http://hz.yj202588.top/gtnjhvocaf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangkeji.top/gtmubmgsnh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtjzuyipqr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtkhookgyp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtsthlipjl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtunmqpxtx.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gteukibslk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gotoacloud.top/gtcoljdmex.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ppjwa.cn/gtifgbamoj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtmdqhoqof.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aizwys.cn/gtzyvhynnk.html

[F11] 复制与移动文件
来源：http://hz.chenzaomai.com/gtnwgubzsr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtcwkisutl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pengpengdd.cyou/gtgdusxkqa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtgbckyykz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gthyvhpwrs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtgjpnemvz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gzhubu.top/gtfucemyqx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gttgybivpg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtgtrwaxzy.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtgqrwnjmp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ywan-chungtsiang.top/gtxqslxsxl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xylfe.cn/gtdrpflsii.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtybyvjoof.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtnncavufz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gtdbmphipz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtybslckrl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtxpzxzmqf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtndnpjaff.html

================================================================================
来源：http://hz.gotoacloud.top/gthkdxovmw.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtxdsogcpi.html

================================================================================
来源：http://hz.52xcode.cn/gtbbsgihos.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtkjusrjsy.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtkxqqjhtm.html

PHP:  class User {}
来源：http://hz.sweek.top/gtkvcdixuo.html

JS:   class User {}
来源：http://hz.yj20258888.top/gtghdmpeca.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtaxxuoyss.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtoavjoqcd.html

Go:   type User struct { Name string }
来源：http://hz.shangyingyoupin.top/gtuknmjqmw.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gtuqopjctp.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gthtbpynuo.html

[G02] 构造函数
来源：http://hz.hywenlv.cn/gtllroptts.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zycfv.cn/gtkunhcdsc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtmczcmgfb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtcbjzegrq.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtskqgtqpo.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gteuhmyxax.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtztuggdhh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtfikwcsmg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangkeji.top/gtkycjtato.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtlmenuhaj.html

Py:   self.name = "x"
来源：http://hz.ivvv.top/gtfffpwihq.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtypbuanrt.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtvssmwvqs.html

TS:   name: string = "x";
来源：http://hz.xinyue.icu/gtfkelydcv.html

Java: private String name;
来源：http://hz.smart0.xyz/gtttpaepdd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gtffavbtah.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gtdetbjbbw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hfpthk.cn/gtknhxnort.html

[G04] 定义方法
来源：http://hz.wangshuangyany.cn/gtdumziwne.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gtilznlyal.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtrookbinz.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtuamedetg.html

TS:   greet(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtnkvqjbwd.html

Java: String greet() { return name; }
来源：http://hz.cqqwz.cn/gthfzdxcwn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtqmgniahg.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtaqezhpyn.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gticuhaekw.html

[G05] 继承
来源：http://hz.wangdashe.top/gtvzzowhsc.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtfpzoctfi.html

PHP:  class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtchfswoaw.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtblpdrijz.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtzrsspqqo.html

Java: class Admin extends User {}
来源：http://hz.xziqi.cn/gtkcoyqrdz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.birdmap.top/gttpksspgk.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtczbcaijx.html

C#:   class Admin : User {}
来源：http://hz.cucudq.cn/gttswjdjht.html

[G06] 重写方法
来源：http://hz.9152youxi.cn/gtpxfnrwda.html

Py:   def greet(self): return "admin"
来源：http://hz.tianlin.xyz/gtvylcdbzb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtfcjduheg.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtolcfvhhc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtdmqnqxvf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gthevlrhgl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtstakvsbu.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtzlryycsi.html

C#:   public override string Greet() => "admin";
来源：http://hz.hongshengwenyu.top/gtasnpptam.html

[G07] 调用父类方法
来源：http://hz.aibaodan.cn/gtmktnnwgi.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtznmlsqjj.html

PHP:  parent::greet();
来源：http://hz.fzhhl.top/gtruwejrnj.html

JS:   super.greet();
来源：http://hz.yuxming.cn/gtrhuifjwl.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtcwrcvqtx.html

Java: super.greet();
来源：http://hz.jlsjyb.cn/gtcuyafubo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gotoacloud.top/gtscgatmzr.html

Ruby: super
来源：http://hz.sweek.top/gtwwbzmxey.html

C#:   base.Greet();
来源：http://hz.cucudq.cn/gtdcnvmvvj.html

[G08] 静态方法与属性
来源：http://hz.sysykeji.top/gtlnzifkzm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtoilumyjq.html

PHP:  public static function f() {}
来源：http://hz.aizwys.cn/gtklekajgr.html

JS:   static f() {}
来源：http://hz.jyoumei.cn/gtggudnglf.html

TS:   static f(): void {}
来源：http://hz.bjfxy.top/gtbmgborgv.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtzvjqzbfz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hongshengwenyu.top/gtahxpfzpp.html

Ruby: def self.f; end
来源：http://hz.xylfe.cn/gteklelwgd.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtpnmtpnxs.html

[G09] 接口 / 抽象类
来源：http://hz.zhiwuduotai.top/gtlpvkyntn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gttwezqgqi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sufxvd.cn/gtehxyqxiw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fzhhl.top/gtbkrwmyft.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtstjmcpvi.html

Java: interface Shape { double area(); }
来源：http://hz.guowangkeji.top/gtqenewlxw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtabijsgjt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.9152youxi.cn/gtrwrhptxz.html

C#:   interface IShape { double Area(); }
来源：http://hz.hywenlv.cn/gtfgavscat.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtizioliaj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtbalhwloy.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtyfguncva.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtympnlpes.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gthlirrgty.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtpjeufndu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cucudq.cn/gtjhkwkrnu.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gtpwjpbhug.html

C#:   public / protected / private / internal
来源：http://hz.cheryme.top/gtlswbwybb.html

[G11] getter / setter
来源：http://hz.aibaodan.cn/gtymtwgsod.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtewizpggo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yonumen.top/gtcpiimqkj.html

JS:   get name() { return this._name; }
来源：http://hz.yueranfly.top/gtutvrspma.html

TS:   get name(): string { return this._name; }
来源：http://hz.tian-w.cn/gthuhurpqk.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtxofpigrb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pycfn.com/gtbbiqivcb.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtykagnmcu.html

C#:   public string Name { get; set; }
来源：http://hz.hammf.cn/gtyyihimou.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtcmubdfoq.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtgotpfwkl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ivvv.top/gtrcjazkjn.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gtgoijotzq.html

TS:   toString(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtmbcngqgq.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtnrdykkma.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtfefqghxi.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtiriyzryj.html

C#:   public override string ToString() => Name;
来源：http://hz.hywenlv.cn/gtdtabwtct.html

[G13] 判断对象类型
来源：http://hz.birdmap.top/gtfnuqjgly.html

Py:   isinstance(u, User)
来源：http://hz.haohaochexian.top/gtpajdjowd.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtrhrauksa.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtcoywgwow.html

TS:   u instanceof User
来源：http://hz.bjfxy.top/gtftdwegtz.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtbmhfurxk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gtuyrgfmwp.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258888.top/gtmmijkohg.html

C#:   u is User
来源：http://hz.fengsongda.top/gtlvejtzlz.html

[G14] 数据类 / record
来源：http://hz.dashuyun.cn/gttdfljqol.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtfswqajev.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtsalxhrfz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuanzhike.top/gtshondtor.html

TS:   type User = { name: string; age: number };
来源：http://hz.ivvv.top/gtjigplyrc.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtjkjbmdqj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtyvwgwdbp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtjolmewga.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gthdcwiqdl.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtqsceopeu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hywenlv.cn/gttbbzngfl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.smart0.xyz/gtnorxbhir.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtcyhfqdzz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtamkngtik.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtxzvcuuyi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtiyrgwnuc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gtdrhmuuqv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtxglzvjum.html

[G16] 对象转数组 / 字典
来源：http://hz.xingfuxueyuan.xyz/gtudsveymz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtsmhdwhcs.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtavgymtsg.html

JS:   Object.entries(obj)
来源：http://hz.dianchejie.cn/gtqssiukfy.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtjzqhlaoi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtwgmrbygk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.0kj1m.cn/gtmdrzhwqy.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtawoqgyhi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gthxvxqvtp.html

================================================================================
来源：http://hz.xinyue.icu/gtlgtdvaot.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtpmblbljo.html

================================================================================
来源：http://hz.birdmap.top/gtofhmpgaw.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gttzpiqjvg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtkxjnmnkk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtcngpsaps.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtoqhmodne.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gtufhxeyqs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtkxbxqriu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtoudzrckm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pycfn.com/gtebzbhckh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuetiantiany.cn/gtgayqsjma.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtxoqvnehd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtqrpxqjws.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtmxmvvfhh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtcfcunpqo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtrchjchlo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtdgnxdgit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtniapgdcl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtbyqptfoh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuxming.cn/gtwqusblnx.html

[H03] 主动抛出异常
来源：http://hz.jiagoushi.top/gtiqzedwka.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtgjfiilms.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gttfqpveba.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gttpdawqoh.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtieouqbei.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gthrmqhxjl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gtetkazntu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenlongwang.top/gtvmtjvkyh.html


<!-- 参考信息 -->