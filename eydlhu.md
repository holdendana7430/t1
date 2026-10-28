代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtagnsspck.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenlongwang.top/gtxnogjxik.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtenacmwvq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangshuangyany.cn/gtcmblyizi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtfhfkizir.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gtmcturyap.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtuuuvlwcz.html

Ruby: s.bytesize;  s.length
来源：http://hz.cheryme.top/gtkddsnmfy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtjpgvnzor.html

================================================================================
来源：http://hz.xylfe.cn/gtcxbhouoq.html

F. 文件与目录
来源：http://hz.shanyushiyangtech.top/gtrfawkzrm.html

================================================================================
来源：http://hz.shzxlz.cn/gtsoqiajxk.html

[F01] 读取整个文件
来源：http://hz.tianlin.xyz/gtarsropma.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jianghu66.top/gthhjwcgie.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtbahdgzky.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.dashuyun.cn/gtwqpdniqz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cucudq.cn/gtcwihnaub.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtxfkiptgy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.wangdashe.top/gtydfbfwuh.html

Ruby: File.read("a.txt")
来源：http://hz.c1oappe.top/gtszzwsayx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtlgzylgks.html

[F02] 逐行读取文件
来源：http://hz.jqgufenzy.top/gttagbnaxx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.9152youxi.cn/gtsdtcbexj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtqirvmpqp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gttydfwqjv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtlodssmgc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtgymvvcbr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pengpengdd.cyou/gtwiwigsfw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtpvwbmxrq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hammf.cn/gtbvflrjtk.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtzuzompwb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenlongwang.top/gtscajiiml.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtktahkjxj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gturdbvxll.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtrbqoropr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtnedacane.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtjcmhlarj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gtbkguzbum.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtvutrkyau.html

[F04] 追加写入文件
来源：http://hz.aibaodan.cn/gtoersliul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cheryme.top/gtlxoorgbs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinghuilouyu.cn/gteqrbpsvc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gthegjdkvt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtgwgfgohl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.bjfxy.top/gthycqalxy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangkeji.top/gtmwdlhjwn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cucudq.cn/gtcvxmzabb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.daxiang520.top/gtfxatgjri.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxuanxn.top/gtctgwtfxr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtpvrnyhqp.html

PHP:  file_exists("a.txt");
来源：http://hz.shzxlz.cn/gtmajvvtol.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtyokmjqcs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtagyzsait.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtgtvougzj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.vqdsnc.cn/gtkzjvlwxn.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtxrnhnuso.html

C#:   File.Exists("a.txt")
来源：http://hz.hfpthk.cn/gtwkzxpioe.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gtyzqqpdiw.html

Py:   os.remove("a.txt")
来源：http://hz.hnxiangtu.top/gtvdlikppe.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gtlgrckzqo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtrdmywbdo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtfadovhbh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtbkatelkf.html

Go:   os.Remove("a.txt")
来源：http://hz.zhoulong.xyz/gtwguntlgz.html

Ruby: File.delete("a.txt")
来源：http://hz.zhoulong.xyz/gthroiqsib.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gtfkwkmmui.html

[F07] 创建目录（含多级）
来源：http://hz.gogol.net.cn/gtzkvxlmiv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gtzxofmqgj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.smart0.xyz/gtsfvyfdlc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shzxlz.cn/gtcrsqozoq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtlydravuc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.bjfxy.top/gtpkcamotr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenzaomai.com/gttqziqggd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gtjptkwnev.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj202588.top/gtabzwiybs.html

[F08] 遍历目录
来源：http://hz.smart0.xyz/gtickjynhh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtlswiijfc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hywenlv.cn/gtgfjfynaj.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtppdjzigb.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtdmrpkyjs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtjztkrzqv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtfvxsoqqy.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtxryginbr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.bjfxy.top/gtvvxphzbt.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtsfwcinrj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yueranfly.top/gtxqusccky.html

PHP:  filesize("a.txt");
来源：http://hz.hongshengwenyu.top/gtwmwnrwzw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gotoacloud.top/gtewgyqnmo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtzkqkwcyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtkbgykfac.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtqrxtkupr.html

Ruby: File.size("a.txt")
来源：http://hz.svipenyu.cn/gtpeeqkmht.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nwbrower.top/gtfgxshojf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gogol.net.cn/gtdonpvsfs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtylrgeghc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhongyouzk.top/gtazichbgg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtxvabcqnm.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtrihrohxk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtyrxaobxs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtkizicxsw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtpsnhskgt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtjnignvss.html

[F11] 复制与移动文件
来源：http://hz.gaohongyu789.top/gtbgsvmumq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gthzsgzcav.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtgjgovooc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtsfzuignx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtuqqwtnef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yangfankeji.com/gtvdfvtqqi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnxiangtu.top/gthcwyiamu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtkydysnnf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtascemyas.html

[F12] CSV 读写
来源：http://hz.zhoulong.xyz/gtpjbxlogg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtghwsgkyo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj202588.top/gtycfeigeu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gtlaimzaxe.html

TS:   // 同上
来源：http://hz.sxryk.cn/gthawqayjh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtepaadptp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangshuangyany.cn/gtmwcfvygr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ywan-chungtsiang.top/gtahryjyhu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.birdmap.top/gtbxvtosks.html

================================================================================
来源：http://hz.gaohongyu789.top/gtedrjfhrv.html

G. 面向对象
来源：http://hz.meibo888.top/gtbikeycle.html

================================================================================
来源：http://hz.yj202588.top/gttllmkkvv.html

[G01] 定义类
来源：http://hz.ydzc1.top/gtacbtamxy.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtsmegkuxm.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtmrrytlaf.html

JS:   class User {}
来源：http://hz.aizwys.cn/gtdvgpwuyo.html

TS:   class User { name: string = ""; }
来源：http://hz.aibaodan.cn/gtuqjfxaiv.html

Java: class User {}
来源：http://hz.yj20258.top/gtmrosgnpd.html

Go:   type User struct { Name string }
来源：http://hz.quarkkingdee.top/gtmoxcknwt.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gttjgxkwrv.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtjexrltqb.html

[G02] 构造函数
来源：http://hz.zhongyouzk.top/gtobrwoorq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtvxgvtput.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.316326.xyz/gtzqatynko.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtlhqkmert.html

TS:   constructor(public name: string) {}
来源：http://hz.ybcxt.top/gtmyeajqqu.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gthpusrqgu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nwbrower.top/gtrduknafv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgfzy.top/gthhrrsgty.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtmsgvjipf.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtymmwvjon.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtldssjkgc.html

PHP:  public string $name = "x";
来源：http://hz.yuanzhike.top/gtbjfyrdie.html

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gtveyrfvam.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtlmvbglvl.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtqmitmpoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gthsdnsnhg.html

Ruby: @name = "x"
来源：http://hz.zhongyouzk.top/gtjhgxtibp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gthxmivnaw.html

[G04] 定义方法
来源：http://hz.guowangkeji.top/gtufxxdnbl.html

Py:   def greet(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtkvlfqrjb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtogrfszsa.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtdsyxytpe.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtbvjwexgs.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtggslwqhy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hywenlv.cn/gtwxhlxvkh.html

Ruby: def greet; @name; end
来源：http://hz.9152youxi.cn/gtuvpvmaxe.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtxcdqnntb.html

[G05] 继承
来源：http://hz.aibaodan.cn/gtjyjdmukl.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtcyjasezk.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gttzwqjgsq.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtelokosfl.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtqxduawyi.html

Java: class Admin extends User {}
来源：http://hz.zdqjudy.top/gtlkavvsbf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtiwvvrgqj.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gteywctuok.html

C#:   class Admin : User {}
来源：http://hz.xinyue.icu/gtmintqybl.html

[G06] 重写方法
来源：http://hz.daria6918.cn/gtywkloprs.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtinyzaoqt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtzojrttkk.html

JS:   greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtylriwbub.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtunsnagty.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtxjivzcya.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yongpay.top/gthmywhjfb.html

Ruby: def greet; "admin"; end
来源：http://hz.yuanzhike.top/gtceflbhvv.html

C#:   public override string Greet() => "admin";
来源：http://hz.fengsongda.top/gtdfplfsxk.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtdfpptzxv.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gttrbqzmjs.html

PHP:  parent::greet();
来源：http://hz.fzhhl.top/gtfktimpcp.html

JS:   super.greet();
来源：http://hz.xinyue.icu/gtcosefnwj.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gtwdtebdru.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtewsjglpw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jianghu66.top/gttsderfrj.html

Ruby: super
来源：http://hz.chenjidiqi.icu/gtyjesvrsx.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtyouzfqgu.html

[G08] 静态方法与属性
来源：http://hz.zhixingplan.top/gtyujqihlz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtignluvjf.html

PHP:  public static function f() {}
来源：http://hz.zhijiandao.cn/gtlzvqhqhv.html

JS:   static f() {}
来源：http://hz.zdqjudy.top/gtuddrienw.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtmyvgudei.html

Java: static void f() {}
来源：http://hz.jinqigfzy.top/gtexzgmjvv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhaomingkeji.xyz/gtydrhvhug.html

Ruby: def self.f; end
来源：http://hz.ydzc1.top/gtuapuezfs.html

C#:   public static void F() {}
来源：http://hz.snrcjt.cn/gthyyznyqq.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtuapuzxnz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtcpdxjdtt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtpayiywkq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.316326.xyz/gtoatpkqox.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtfvmdyuac.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gtlsdjqzhu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yvedp.cn/gtfwgvujxv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zycfv.cn/gtzajieqqt.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtqlsdtlgx.html

[G10] 访问控制
来源：http://hz.ybcxt.top/gttzfydwaz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tianlin.xyz/gtrowfkynb.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtbbanaiet.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtmhpnnmlh.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtoyukcrvk.html

Java: public / protected / private / 默认包级
来源：http://hz.hysaishi.cn/gtjeafrrge.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zdqjudy.top/gtcnzmxfyg.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtnbvedgun.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gtbmbfbcpr.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gttjbtsncr.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtrjtxhimk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yonumen.top/gtngqopbbu.html

JS:   get name() { return this._name; }
来源：http://hz.dashuyun.cn/gtkbvyoqwr.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gtuxkveykh.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtlcsuzmqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.316326.xyz/gtoxmnsniv.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtmhvkqzmb.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gtbqauqklr.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtapewcxmx.html

Py:   def __str__(self): return self.name
来源：http://hz.feifeiyinyue.top/gtvkshmllw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtphxaueud.html

JS:   toString() { return this.name; }
来源：http://hz.cucudq.cn/gtgjqlvbta.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gthddxwnux.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtgneyueka.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ppjwa.cn/gtqwynotsf.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtfownxgif.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtkoyogqqk.html

[G13] 判断对象类型
来源：http://hz.gogol.net.cn/gtlrfvalbc.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gtmuvzwifi.html

PHP:  $u instanceof User
来源：http://hz.zhiwuduotai.top/gtlgwgyhrr.html

JS:   u instanceof User
来源：http://hz.shuidangran.top/gtbwjzdbkc.html

TS:   u instanceof User
来源：http://hz.shuidangran.top/gtshxbknsi.html

Java: u instanceof User
来源：http://hz.gzhubu.top/gtektxmhqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtbncpidnq.html

Ruby: u.is_a?(User)
来源：http://hz.jinghuilouyu.cn/gtlayhxqvv.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gthpahugiw.html

[G14] 数据类 / record
来源：http://hz.daxiang520.top/gtbwfxdihs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gaohongyu789.top/gtdiqgrylk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhengqikj.top/gtvdwrqsqx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtytkbjxcl.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtggcqkzll.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtadpqljgb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pycfn.com/gtteoqzmdc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gttodjpjjs.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtlqsklytx.html

[G15] 枚举
来源：http://hz.sysykeji.top/gtvmoizclt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gtiwhhafxb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtbqwinzlh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gtdvhzktxc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtkjlhtcly.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gtoqyfemkq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtmnaqbice.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ivvv.top/gtnwwewujt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtgjirklfe.html

[G16] 对象转数组 / 字典
来源：http://hz.xuanzx.com/gtbektjfhk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtknnfftvz.html

PHP:  get_object_vars($obj);
来源：http://hz.chenjidiqi.icu/gtgnuriupv.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtgvimjvkb.html

TS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtssusdyxx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtymmujdeg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtkxewmfcu.html

Ruby: obj.instance_variables
来源：http://hz.quarkkingdee.top/gtlbogjlrk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtgcudofuj.html

================================================================================
来源：http://hz.xinyue.icu/gtbuyqkuba.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtyiaoxrfr.html

================================================================================
来源：http://hz.zhixingplan.top/gtyiphoywc.html

[H01] try / catch 基础
来源：http://hz.daxiang520.top/gttminafhe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gturzndpvu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guannengcc.top/gtltyrkotv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gttxznpflu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gtatzrecyf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtlbaphwvl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jyoumei.cn/gtrqbkajmu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtrjsoqdow.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigufen.top/gtpoawwkmj.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtrvffmlgr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtwzegcxlg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtpqcfeqbg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gteracgrbr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtbfgshlua.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtfmsegjeq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj202588.top/gthzegtxud.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtjhbgkbeu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daxiang520.top/gtxrxdvbbq.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtfrmosnyt.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangkeji.top/gtfwudjuxg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtctmlpyet.html

JS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtarrcauxv.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtqolrcniu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtkhkchjxk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtzrsyijko.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ybcxt.top/gtvdlvlwdb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gttcesigcc.html

[H04] 自定义异常类型
来源：http://hz.snrcjt.cn/gtmnifhewl.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gtxdeequzg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtmpbbldcp.html


<!-- 参考信息 -->