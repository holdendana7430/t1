代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.gogol.net.cn/gtczrvejpx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.snrcjt.cn/gtwqiciihe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigufen.top/gtjkaxggwy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yueranfly.top/gtviuvhgmz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gttchzksqi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sysykeji.top/gteymfpsde.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinyuanbaomall.cn/gtfxbbnawd.html

Ruby: s.bytesize;  s.length
来源：http://hz.0kj1m.cn/gtbdznomvo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gtaoqdasxy.html

================================================================================
来源：http://hz.yj20258888.top/gtfumwrxcw.html

F. 文件与目录
来源：http://hz.daria6918.cn/gtzrtylpag.html

================================================================================
来源：http://hz.yueranfly.top/gtuugpghpq.html

[F01] 读取整个文件
来源：http://hz.nwbrower.top/gtgojvsdxx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhixingplan.top/gtxfsupdph.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtferprgdt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gthjfylzky.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ybcxt.top/gtiilmxfuc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtklvtpvim.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tanke756.top/gtxwdfinco.html

Ruby: File.read("a.txt")
来源：http://hz.hongshengwenyu.top/gtnqkdqzya.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtshsrkymm.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtwdoeehld.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.haohaochexian.top/gtcmhgymeq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shuidangran.top/gtbygqovbk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtovziflpr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtivajotbk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtlzkbvpyx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.havefunace.top/gtgpdmjguo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.havefunace.top/gtiqrcckqa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gteirbhnbs.html

[F03] 写入文件（覆盖）
来源：http://hz.chenlongwang.top/gtdjwmmddv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yanxiufei.cn/gttsyjjivj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jianghu66.top/gtkzurdlqw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtvuqbeljm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtsmwozybv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.guowangkeji.top/gtshjcvjxr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtbdsivpog.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnqzz.top/gtxzmjeeqi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hnxiangtu.top/gtqxtvrzcq.html

[F04] 追加写入文件
来源：http://hz.yuanzhike.top/gtwduuegia.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtjrkrbzbf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jiagoushi.top/gtizbusnuv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtdrfbxylb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtenqtvtkf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.feifeiyinyue.top/gtthmbhajx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.kuanghao11.cn/gtebftqkqo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtqxurfujn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.feifeiyinyue.top/gtgyheejzk.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydjk.org.cn/gtfvrtnfry.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtclewhzms.html

PHP:  file_exists("a.txt");
来源：http://hz.chenzaomai.com/gtondlpqfq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtrthaxwcx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtvakewwwh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtekxqfulz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nwbrower.top/gtyrkivowf.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtkhzfbmtw.html

C#:   File.Exists("a.txt")
来源：http://hz.cdnleiting.top/gtkquwnjqv.html

[F06] 删除文件
来源：http://hz.haohaochexian.top/gtgvvpjkyc.html

Py:   os.remove("a.txt")
来源：http://hz.gotoacloud.top/gtirnjyfiz.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtzdigacyg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtrlirlgnj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtebwsrdnf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtjtvahfrq.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtlciouooj.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtpfozflsw.html

C#:   File.Delete("a.txt");
来源：http://hz.quarkkingdee.top/gtvyfbwkua.html

[F07] 创建目录（含多级）
来源：http://hz.gzhubu.top/gtgfxrhqmx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtrzqbggvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cashguo.top/gtydwttdmp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtzjmasjvv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtnmotaqjm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhixingplan.top/gtvxxqibid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tanke756.top/gtukqvtziy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenjidiqi.icu/gtpbcqydrv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinyuanbaomall.cn/gtyrqqesms.html

[F08] 遍历目录
来源：http://hz.ybcxt.top/gtoqfflxsw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yanxiufei.cn/gtynjfrjfj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtoilfkhpb.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtaymhiicn.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtuzclmcpg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtjfsyttgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtumlzchmx.html

Ruby: Dir.children("dir")
来源：http://hz.sysykeji.top/gtnaqohjsy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gaohongyu789.top/gtnhwriuxy.html

[F09] 获取文件大小
来源：http://hz.xingfuxueyuan.xyz/gtxztgitgj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.vqdsnc.cn/gtkvdaicps.html

PHP:  filesize("a.txt");
来源：http://hz.snrcjt.cn/gtsjiqeipz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gtsaqqtkxe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtywkxtflm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gttpegnomq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cdnleiting.top/gtwjmixbqh.html

Ruby: File.size("a.txt")
来源：http://hz.snrcjt.cn/gtnlgpgsyq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtmsajhoaw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gtyoqihjte.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtwbrbqdzq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.0kj1m.cn/gtngyystya.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtwkfcscza.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtbzscbdng.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtfywcqqaa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtadvvxnuu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtbzsvnhin.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gtjzemifxo.html

[F11] 复制与移动文件
来源：http://hz.daxiang520.top/gtbeoucexa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gteyxrckzi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtwdsheacx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtrprtiput.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtgmbgvtrh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtasjuibpu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinqigfzy.top/gthzsrkijg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtigejjcsj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtoosgtihq.html

[F12] CSV 读写
来源：http://hz.snrcjt.cn/gtunulkxmn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hysaishi.cn/gtunzjjbdu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhoulong.xyz/gtplpsotww.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtlipmkrpa.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtbbjkabix.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtpfxizoda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ppjwa.cn/gtmrkxsuvl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtgfnqspnt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtlhbzgjkm.html

================================================================================
来源：http://hz.yongpay.top/gtnqziqmcm.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtkreqrzwq.html

================================================================================
来源：http://hz.hywenlv.cn/gtpspjwcdl.html

[G01] 定义类
来源：http://hz.xinyue.icu/gtyuojjgtx.html

Py:   class User: pass
来源：http://hz.xuetiantiany.cn/gtvutzvjrv.html

PHP:  class User {}
来源：http://hz.mhx1999.top/gtrrtpqaho.html

JS:   class User {}
来源：http://hz.feifeiyinyue.top/gtfnqsxzlt.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gthfcoctaq.html

Java: class User {}
来源：http://hz.gotoacloud.top/gtfklnmuuc.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtsqekbuaq.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtrlfyvdsy.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtdqynxpms.html

[G02] 构造函数
来源：http://hz.yuxming.cn/gtftulvfzx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yangfankeji.com/gtgxwahmvf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtfxqnkeoc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yueranfly.top/gtnvqkpmlt.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtpcrsporz.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtffejmuuo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtotjccesc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtoetpggef.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtwmlnganw.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtxhvlpwjs.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtsiywrxbt.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtmccebhnu.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gthgvasuom.html

TS:   name: string = "x";
来源：http://hz.zycfv.cn/gtwxmnjplg.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtbabpkvqn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ybcxt.top/gtxrurrjsj.html

Ruby: @name = "x"
来源：http://hz.hnqzz.top/gtgpgmfdzo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtpzdgrhhq.html

[G04] 定义方法
来源：http://hz.jinqigufen.top/gtlhekoiix.html

Py:   def greet(self): return self.name
来源：http://hz.pycfn.com/gtlytxapnq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtopfbkzad.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtgicmxizg.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtrbnetsfq.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gtgqcqqppn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gteobkagsl.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtodrfnuzn.html

C#:   public string Greet() => Name;
来源：http://hz.yuanzhike.top/gtsewsgrfc.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtjaeeugip.html

Py:   class Admin(User): pass
来源：http://hz.iojbl.cn/gtfetbtrhx.html

PHP:  class Admin extends User {}
来源：http://hz.zhengqikj.top/gtqgbggrqw.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gthrzooiad.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtmrqsinfj.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtcsuzqofz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gtmadzrnsi.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtbbxwzqiu.html

C#:   class Admin : User {}
来源：http://hz.jinyuanbaomall.cn/gtksooqfrs.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gtuslqyenf.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtvwmcoypg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtwhiqvbgv.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtomxjykud.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtasltgkfe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtrselgmsi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ybcxt.top/gttqagkqpd.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtemxcjcnb.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhongyouzk.top/gtltqwkebh.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtiwzgfgcr.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtckupoxev.html

PHP:  parent::greet();
来源：http://hz.aibaodan.cn/gtkwnwhxww.html

JS:   super.greet();
来源：http://hz.yuxming.cn/gtlpzjnjyb.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtnugfqqhz.html

Java: super.greet();
来源：http://hz.zhijiandao.cn/gteonsyldm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sufxvd.cn/gthrdflxpp.html

Ruby: super
来源：http://hz.ywan-chungtsiang.top/gtfxrkujor.html

C#:   base.Greet();
来源：http://hz.kuanghao11.cn/gteipxtrtz.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gttcdqslfi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtbhukedpr.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtdsyfzutm.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtpodplnqx.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtbwddllae.html

Java: static void f() {}
来源：http://hz.jqgfzy.top/gtqvuhokee.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtdxatpgyj.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtwzuwfoyl.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtekjhymjc.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtsyabyjrf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gtuamqimth.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtukrzyffh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnxiangtu.top/gtpptokfdl.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtceloltmd.html

Java: interface Shape { double area(); }
来源：http://hz.ydjk.org.cn/gtjdbteyjl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gthslqzbqr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhengqikj.top/gtgemnrewr.html

C#:   interface IShape { double Area(); }
来源：http://hz.ppjwa.cn/gtgihpkygh.html

[G10] 访问控制
来源：http://hz.ivvv.top/gtsxyugpng.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtyicsiczc.html

PHP:  public / protected / private
来源：http://hz.hysaishi.cn/gtkdjbrmof.html

JS:   #private 字段；其余公开
来源：http://hz.hfpthk.cn/gturbffqdx.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtyxuwdmxq.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtwoxolyqj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtyeyrnnuh.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gtmwzctgyj.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtuehwatgc.html

[G11] getter / setter
来源：http://hz.gotoacloud.top/gtcycqqlqx.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtxgonuepz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtmacamfrw.html

JS:   get name() { return this._name; }
来源：http://hz.sysykeji.top/gttxdcuhtp.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxinkj.top/gtnhgzlvzj.html

Java: public String getName() { return name; }
来源：http://hz.yonumen.top/gtfoadkvpj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuanzx.com/gtyiolnsgy.html

Ruby: attr_accessor :name
来源：http://hz.zhengqikj.top/gtxgvgjfyg.html

C#:   public string Name { get; set; }
来源：http://hz.daria6918.cn/gtwungcmua.html

[G12] 对象转字符串
来源：http://hz.yuxming.cn/gtiffnrgpr.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gtpsdaylud.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtmmthrity.html

JS:   toString() { return this.name; }
来源：http://hz.guowangkeji.top/gtvacmtbub.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtesgdqwur.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtbchbhfjl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtedcjgfbm.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigfzy.top/gtreureokh.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtmywwgezw.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gteawzkgjg.html

Py:   isinstance(u, User)
来源：http://hz.yj20258.top/gtudolzejq.html

PHP:  $u instanceof User
来源：http://hz.gotoacloud.top/gtmswcryuz.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtmvczqazq.html

TS:   u instanceof User
来源：http://hz.bjfxy.top/gtmbjhmvgm.html

Java: u instanceof User
来源：http://hz.jinqigfzy.top/gtyqqmbvaq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhengqikj.top/gtlsxibxke.html

Ruby: u.is_a?(User)
来源：http://hz.andypj.xyz/gtfunbdmfr.html

C#:   u is User
来源：http://hz.andypj.xyz/gtevvthmue.html

[G14] 数据类 / record
来源：http://hz.yj202588.top/gthniazgig.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xinyue.icu/gtdkbntznp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hfpthk.cn/gtqjyvztcn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtfkkoryeo.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtwoxncjuv.html

Java: record User(String name, int age) {}
来源：http://hz.xuanzx.com/gtjxhfbeom.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtvetrtifu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtfpwphydt.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtwdwsknco.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gthjqxrqyj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gtdhyevrfh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinyuanbaomall.cn/gtrlcalyza.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtrxtlffhm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtblymicgu.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtmuogxnzi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jianghu66.top/gtybclyvfa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gttctwgtbd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gthdsyhddb.html

[G16] 对象转数组 / 字典
来源：http://hz.nwbrower.top/gtieexkabz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.52xcode.cn/gthvlqslok.html

PHP:  get_object_vars($obj);
来源：http://hz.ydzc1.top/gtmwmevvpn.html

JS:   Object.entries(obj)
来源：http://hz.yuanzhike.top/gturwihgsm.html

TS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtdekjrkoj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnxiangtu.top/gtviqidouo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtlewqihyz.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtpqdmoigl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gtnmauhoes.html

================================================================================
来源：http://hz.gogol.net.cn/gtzweihnzu.html

H. 异常与错误处理
来源：http://hz.havefunace.top/gtljegvffs.html

================================================================================
来源：http://hz.snrcjt.cn/gtuyutbwkc.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtlozrdvgd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangdashe.top/gtgffwjcif.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhijiandao.cn/gtmxzkvmel.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtautnqvds.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gtlqdpbunx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gteuelyvji.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtaqeletpg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gteuvpnxlm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtgczcpudu.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtaedlxawj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnqzz.top/gtvcnuuoou.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtxddregrc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtausyrmur.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtcrzwwxpf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtkeetpbqo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtztvgrthc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gzhubu.top/gttgmehupz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.mhx1999.top/gttykvzqqk.html

[H03] 主动抛出异常
来源：http://hz.dashuyun.cn/gtserxyhba.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gttqkvgejc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtahoniwqr.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtdlhlbzvx.html

TS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtbgkmksjs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtppddavcv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gthcesvrul.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.vqdsnc.cn/gtwlgrjjzp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtjrtemxil.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gtjsmeqmbw.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtyouirssn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtggifjlxv.html


<!-- 参考信息 -->