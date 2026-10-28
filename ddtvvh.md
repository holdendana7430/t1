代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtxhezddkg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtmrqdpxza.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gtykdhqftf.html

Java: if (s.isEmpty()) {}
来源：http://hz.bjfxy.top/gtwuzyigsc.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gtqriwxldb.html

Ruby: if s.empty?
来源：http://hz.zdqjudy.top/gtfgyzobit.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.haohaochexian.top/gtufupemxm.html

[E21] 超长截断加省略号
来源：http://hz.cashguo.top/gttdanphgm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhixingplan.top/gtqocurkwf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ydzc1.top/gtrvcfmpih.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtjcytpfuj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtplmhstwo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtujkxrtub.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhijiandao.cn/gtnqlecxpa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuanzx.com/gtvuhiijnv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.aizwys.cn/gtjfnrzwty.html

[E22] 字节长度与字符长度
来源：http://hz.zhoulong.xyz/gtykoorndq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtdrhevzin.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtdprikrbj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtmsxdrtnt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gticjahcrb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtnljuuzgg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtcuhuwibs.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtuyyjkdyq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.52xcode.cn/gtijxdiqrb.html

================================================================================
来源：http://hz.birdmap.top/gtcfkhaxsh.html

F. 文件与目录
来源：http://hz.jyoumei.cn/gtgfpssssb.html

================================================================================
来源：http://hz.gogol.net.cn/gtpcibxmlr.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gtkrcxdzlq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.haohaochexian.top/gteppxvjob.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenlongwang.top/gtojngignu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtisknggom.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtkudrrvfy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtkojbilwp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sxryk.cn/gtmjrgpnsw.html

Ruby: File.read("a.txt")
来源：http://hz.jyoumei.cn/gtfgazkjjj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cucudq.cn/gtkfzrijgy.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtwdgeivle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sufxvd.cn/gtkaalnzck.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtthuqatxk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtelqwivik.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtghhccvhn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtmitycrvj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gthlwwupqc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtpgqohifw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.mhx1999.top/gtjpamfowt.html

[F03] 写入文件（覆盖）
来源：http://hz.hnxiangtu.top/gtxxrqfgzm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guowangkeji.top/gtmfqiimba.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aizwys.cn/gttkkirhqu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtlebzlzjq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtiungtmgz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gogol.net.cn/gtvhdksfxi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.haohaochexian.top/gttuixoeji.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nwbrower.top/gtyfhhfzln.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtriwxoglk.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtrjbliead.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ywan-chungtsiang.top/gtbtzgqsdc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtnsshxjgt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtbmqouoxu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtzsdzmoiy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xylfe.cn/gtmdaoxdpb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gttqbpwflj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhiwuduotai.top/gtwjpjmyey.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sysykeji.top/gtfryyqvyb.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgufenzy.top/gtrjpfkmyc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gtkkwxpbjw.html

PHP:  file_exists("a.txt");
来源：http://hz.52xcode.cn/gtacqvhbom.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtfzkflgal.html

TS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtsykxieot.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtjtuxucqn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinghuilouyu.cn/gtsnzxhunp.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtmjcaodvu.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gtfzxjtdba.html

[F06] 删除文件
来源：http://hz.yanxiufei.cn/gtpsupehcc.html

Py:   os.remove("a.txt")
来源：http://hz.gaohongyu789.top/gtdrymfmyn.html

PHP:  unlink("a.txt");
来源：http://hz.mhx1999.top/gtsbxqnpkz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gthjhftiam.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtsrcqydny.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtdrolhwzs.html

Go:   os.Remove("a.txt")
来源：http://hz.fzhhl.top/gttysyotwt.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtdaterplv.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtexxyobyt.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258.top/gtiwuararb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtuugnswiq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hongshengwenyu.top/gtbjsmnjeo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtyjpnazvy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gthehqrjcp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnqzz.top/gtkqxtetqs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.bjfxy.top/gtbqzipqyo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.316326.xyz/gtbmttpapq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtvzyqtasr.html

[F08] 遍历目录
来源：http://hz.aizwys.cn/gtpewjustw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gogol.net.cn/gtnjamvfoi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtqvpecuvf.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtfbjjwspj.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtgssbashu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtwvsmwfjg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yanxiufei.cn/gtrazfidbo.html

Ruby: Dir.children("dir")
来源：http://hz.tanke756.top/gtlksvaglc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinyuanbaomall.cn/gtcmlatdrw.html

[F09] 获取文件大小
来源：http://hz.shzxlz.cn/gtztgcnvby.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhengqikj.top/gtomdikmep.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gtlcnsefax.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtbwinlugh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtdvxialcg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtawvtwdgu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtbcrgrxtm.html

Ruby: File.size("a.txt")
来源：http://hz.wangshuangyany.cn/gtfixwplyv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtvkqangme.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gttlwmirlb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtwyfcxaig.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinghuilouyu.cn/gthnnkifkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtvwjgyyem.html

TS:   path.extname("a.txt")
来源：http://hz.xuanzx.com/gtltpvfxnx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxinkj.top/gtbizjtnnq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hywenlv.cn/gtgoiqbdlg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtuwvbkvoc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gtgxmeabyo.html

[F11] 复制与移动文件
来源：http://hz.havefunace.top/gtlnolwfhs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtasfncftp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daxiang520.top/gtaitpalmm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtljvyyphb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtmvebzwes.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gotoacloud.top/gticesehuv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtldgltmmr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtsokzpkub.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gtvcshukwg.html

[F12] CSV 读写
来源：http://hz.nwbrower.top/gtlfsnmgaa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtywjmnbgq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cqqwz.cn/gtjnwccras.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtjkmqurel.html

TS:   // 同上
来源：http://hz.xingfuxueyuan.xyz/gtdltmnmfc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtcnanvpsx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gttdzmqyug.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtplpgtcsq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhengqikj.top/gtyyntlbto.html

================================================================================
来源：http://hz.yuxming.cn/gtezazwfbk.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gthxnmilih.html

================================================================================
来源：http://hz.xziqi.cn/gtghwffmrm.html

[G01] 定义类
来源：http://hz.52xcode.cn/gtabvzpecs.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtnsbzcpyz.html

PHP:  class User {}
来源：http://hz.cheryme.top/gtznayytpt.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtiqutsogj.html

TS:   class User { name: string = ""; }
来源：http://hz.yueranfly.top/gtjzkdienq.html

Java: class User {}
来源：http://hz.gotoacloud.top/gtsihqzdyt.html

Go:   type User struct { Name string }
来源：http://hz.xziqi.cn/gthfbluvrj.html

Ruby: class User; end
来源：http://hz.xinyue.icu/gtdvqemjyv.html

C#:   class User {}
来源：http://hz.iojbl.cn/gtjxoabrtt.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtqhahlheh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtgacpcrpu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yueranfly.top/gtfnzzupke.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gtkcjulsjp.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gtcaoiilcn.html

Java: User(String name) { this.name = name; }
来源：http://hz.xinyue.icu/gttdbrwyir.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ybcxt.top/gtevvvfude.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gtxxiaewie.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gtnxxbbpfk.html

[G03] 实例属性
来源：http://hz.jinghuilouyu.cn/gtmgsywzaq.html

Py:   self.name = "x"
来源：http://hz.zhongyouzk.top/gtnlbhagku.html

PHP:  public string $name = "x";
来源：http://hz.tanke756.top/gttnjylgmx.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtllehekoe.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtnrgjimnu.html

Java: private String name;
来源：http://hz.zhixingplan.top/gtkrjxxcpw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gtbnchhity.html

Ruby: @name = "x"
来源：http://hz.cqqwz.cn/gtcnhozxys.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ehwqpu.com/gtosphjwdc.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtoxszqdor.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtcdmpatnx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtygjrofvd.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtcellawef.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gthyfxwrrr.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtmptslxuc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtsbqbdlhr.html

Ruby: def greet; @name; end
来源：http://hz.jinqigfzy.top/gtujdaqdur.html

C#:   public string Greet() => Name;
来源：http://hz.ywan-chungtsiang.top/gthhjixkqx.html

[G05] 继承
来源：http://hz.xziqi.cn/gtdnpzyomi.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtpeglhflu.html

PHP:  class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtnrmaisyk.html

JS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gtoczmmlgu.html

TS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtmtztkogh.html

Java: class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtzfcapmll.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigfzy.top/gtisrzlrvt.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtvjiyfiap.html

C#:   class Admin : User {}
来源：http://hz.sxryk.cn/gtwqzqddyf.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gtrqxqnqqw.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtietafscq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtjznphnhb.html

JS:   greet() { return "admin"; }
来源：http://hz.meibo888.top/gtwpggdkvn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtlseytowj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtomaywqsm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtbooztxdd.html

Ruby: def greet; "admin"; end
来源：http://hz.jiagoushi.top/gtshfjwlgr.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtzobkcess.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtfxmjmvsk.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gthozhcysj.html

PHP:  parent::greet();
来源：http://hz.hnqzz.top/gtbfaplknq.html

JS:   super.greet();
来源：http://hz.xziqi.cn/gtaefgfedy.html

TS:   super.greet();
来源：http://hz.hammf.cn/gtmiqclmek.html

Java: super.greet();
来源：http://hz.chenlongwang.top/gtixoshjtk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.0kj1m.cn/gtqvvqcbsg.html

Ruby: super
来源：http://hz.mhx1999.top/gtbpscyhem.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtxuckspgm.html

[G08] 静态方法与属性
来源：http://hz.xingfuxueyuan.xyz/gtmrbvbgrm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zdqjudy.top/gtwsjrcvpd.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtgypbodmc.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gtmxfbguwo.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gthnbseopr.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtaqsjdvdz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtnqmockiw.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtmnjobskb.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gtwfuhijop.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtxpenaeck.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.redwolf501.top/gtyscdqsqg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gogol.net.cn/gtzltscyvi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtkwambsdd.html

TS:   interface Shape { area(): number; }
来源：http://hz.haohaochexian.top/gtqdponhvv.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtsirkobbe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtpwvufnhk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtjznflesh.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtihvzmrev.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtelgqhagg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.havefunace.top/gtykugjuhp.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gttdedzaby.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtdzxfrjaa.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtzppsyozb.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtqbpszlgl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtiexecqgd.html

Ruby: public / protected / private
来源：http://hz.daria6918.cn/gtqvhnqzfh.html

C#:   public / protected / private / internal
来源：http://hz.fengsongda.top/gtkjanijnd.html

[G11] getter / setter
来源：http://hz.yonumen.top/gttzdlxjey.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtswdiswoy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtuapfpxxf.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtvonxlhiy.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gtouzlfnim.html

Java: public String getName() { return name; }
来源：http://hz.jinqigufen.top/gtwgfkdisd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtvtsegugx.html

Ruby: attr_accessor :name
来源：http://hz.xylfe.cn/gtsgtgjare.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtmwykbnwz.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtwfrpavjt.html

Py:   def __str__(self): return self.name
来源：http://hz.nwbrower.top/gtpalaarnl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtncphbskg.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtkpnqwjep.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtexvibhfh.html

Java: @Override public String toString() { return name; }
来源：http://hz.quarkkingdee.top/gtjquttben.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtnjqauytx.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtvesubbzx.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtjwtxgmym.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gtaeoxfeut.html

Py:   isinstance(u, User)
来源：http://hz.cdnleiting.top/gtusudmcvu.html

PHP:  $u instanceof User
来源：http://hz.yuanzhike.top/gtkpfdsjjy.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtphuheqsx.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gthyyyjsgr.html

Java: u instanceof User
来源：http://hz.feifeiyinyue.top/gtvndgodsu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.andypj.xyz/gtbdkhosfk.html

Ruby: u.is_a?(User)
来源：http://hz.svipenyu.cn/gtgpudcwtd.html

C#:   u is User
来源：http://hz.hongshengwenyu.top/gtmvaeloov.html

[G14] 数据类 / record
来源：http://hz.xingfuxueyuan.xyz/gtiufquhxh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xinyue.icu/gtsjmlnnfi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhongyouzk.top/gtnofntvtp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtrylxzabb.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangtech.top/gtrowwegho.html

Java: record User(String name, int age) {}
来源：http://hz.zdqjudy.top/gtevlumypm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtttdkltux.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtzfhofniu.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtdnfxfotw.html

[G15] 枚举
来源：http://hz.andypj.xyz/gthyvlzlvf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxuanxn.top/gtbdwstvte.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtcukycgub.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtfxeupjah.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gthymrtuyk.html

Java: enum Color { RED, GREEN }
来源：http://hz.fengsongda.top/gthnbhsxgr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangkeji.top/gtssoxsbxt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtnhcqgcml.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtjzcqijhk.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxinkj.top/gtotpcebrl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sxryk.cn/gtzqqqtlus.html

PHP:  get_object_vars($obj);
来源：http://hz.hysaishi.cn/gtwgxdfofh.html

JS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtfyebkznq.html

TS:   Object.entries(obj)
来源：http://hz.birdmap.top/gtynpaxiiw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtycgaxdzh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhixingplan.top/gtbzujmwfw.html

Ruby: obj.instance_variables
来源：http://hz.yongpay.top/gtqqthwunc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtovbofsru.html

================================================================================
来源：http://hz.ivvv.top/gtilxeagfx.html

H. 异常与错误处理
来源：http://hz.pengpengdd.cyou/gtnacrliyv.html

================================================================================
来源：http://hz.sysykeji.top/gtqwativkd.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtaibeludk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ppjwa.cn/gtjtyxshrr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigufen.top/gtdvvfiikw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtbxrtedfu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtmojjpazt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yvedp.cn/gtsqzgeysw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtwdcsjphc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ivvv.top/gtyqwxihcg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtvcrtlirp.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtluzbdvxr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtmiwwnuqj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtasupkgbd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtbuvzwoqk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtfuibvimb.html


<!-- 参考信息 -->