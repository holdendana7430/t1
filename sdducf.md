代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtzclkpcgm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ybcxt.top/gtlzwzviff.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtfzwnjbzc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtefmjqvwi.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gtxpxbftpo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.redwolf501.top/gtkxvsbegm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtoakjouym.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtcivfkepw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtrorzzhev.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtuizfbbru.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.tian-w.cn/gtjnhuyzkt.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhengqikj.top/gtyhilcbef.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.haohaochexian.top/gtqwmstfsz.html

================================================================================
来源：http://hz.yangfankeji.com/gthpmgmsul.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gtsbgvnjsj.html

================================================================================
来源：http://hz.chenlongwang.top/gtdqsrqdyw.html

[F01] 读取整个文件
来源：http://hz.gogol.net.cn/gtpsgrufdi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yonumen.top/gtcjapmaox.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydzc1.top/gtapqakgbd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gthxiuclga.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gtdpavaygp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtvtrfwbfr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.redwolf501.top/gtzyokqufn.html

Ruby: File.read("a.txt")
来源：http://hz.hnqzz.top/gtcbvekovq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtbrxzvxvr.html

[F02] 逐行读取文件
来源：http://hz.chenjidiqi.icu/gttginxzam.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zdqjudy.top/gthsfsvhfj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtphradpqx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtxvxtwawe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenzaomai.com/gtxcykcfdw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtwcbapyay.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnxiangtu.top/gtsqfglpei.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangdashe.top/gtifsttygw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guowangkeji.top/gtbktwhwiq.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtffhgxtbx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigfzy.top/gtaenqydlt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258.top/gtmepkqfhq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtmctptkgl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gthbvsbbzr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtazyjqgsu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.kuanghao11.cn/gttzpeegxh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtepslqdds.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yonumen.top/gtgphmjepi.html

[F04] 追加写入文件
来源：http://hz.sufxvd.cn/gtnuoxofyd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gtfwupavpr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.52xcode.cn/gtkssofaic.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.0kj1m.cn/gthvdpnywq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gtpxwwtbgd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtvyvqlwdh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj202588.top/gtsyumsznx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtsvneggse.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zdqjudy.top/gtavvoucmk.html

[F05] 判断文件或目录是否存在
来源：http://hz.haohaochexian.top/gtqgrtegsg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtjqnttxne.html

PHP:  file_exists("a.txt");
来源：http://hz.0kj1m.cn/gttgyigjfv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gtpxqpzski.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtdwgxdmfx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gthehjzbzl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenlongwang.top/gtbmuaxzae.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuanzx.com/gtyvsctdiv.html

C#:   File.Exists("a.txt")
来源：http://hz.birdmap.top/gtsgvaoxbh.html

[F06] 删除文件
来源：http://hz.nanxinkj.top/gtbunugfbw.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtapaotphs.html

PHP:  unlink("a.txt");
来源：http://hz.fengsongda.top/gtpujmrvqd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.c1oappe.top/gtbuznfoqq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtcsxmckcq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fengsongda.top/gtfatcfwyv.html

Go:   os.Remove("a.txt")
来源：http://hz.fengsongda.top/gthvbvebds.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtzxaptebv.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtvupxyyts.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtemvwnrjl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtoumlrbij.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtvaxkzxbb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gteeiwlgwo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gthbgfjebs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangkeji.top/gtjyjvxieh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cucudq.cn/gtxutczhyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daxiang520.top/gtczgrbqjj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.aibaodan.cn/gtehucdhjx.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gteoxflgye.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ppjwa.cn/gtlhrbnagc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cucudq.cn/gtvhgjxvns.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gttxfcgexi.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtfdfwkkwg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtcfrcgbmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xuanzx.com/gtwzyxmffw.html

Ruby: Dir.children("dir")
来源：http://hz.sysykeji.top/gtczhzmaqf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gtkabbdcdq.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtvvwksgwe.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtzbsqedfn.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtbjlwksuv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtgaqzqykn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtcxzyeiry.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtmlwckeis.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tian-w.cn/gtasghmlxq.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtfgfnqjun.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtquaylkby.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gtjdstaepi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtdnohkhfk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtdtsyzeio.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtfgwihddi.html

TS:   path.extname("a.txt")
来源：http://hz.xuanzx.com/gtfihufgay.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.c1oappe.top/gtolbtmdoy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xylfe.cn/gtaovjpvkj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtotghemrw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtlmgtvuhk.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtpkuegxxd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtgwwznadf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tanke756.top/gtwrlgnohp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtkigulyzg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtiyinrnui.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guannengcc.top/gtdlxnumrg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtgxagvahe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtybxoilpp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtdvixxixp.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gthukmbajs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.52xcode.cn/gtujrogclo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtljjpkonr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sweek.top/gtuxzwyshi.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtpysavplu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gthaowtboi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hongshengwenyu.top/gtcitzuaxw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.meibo888.top/gtluogmgdc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtbitcuqnw.html

================================================================================
来源：http://hz.sweek.top/gtktlhmfjn.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtyaskbqnr.html

================================================================================
来源：http://hz.jinqigufen.top/gtubquyofd.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gtvinigthx.html

Py:   class User: pass
来源：http://hz.smart0.xyz/gtrqahjpwc.html

PHP:  class User {}
来源：http://hz.c1oappe.top/gtnkzgaexd.html

JS:   class User {}
来源：http://hz.meibo888.top/gtnhkrmglw.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgfzy.top/gtcqzidsdq.html

Java: class User {}
来源：http://hz.cucudq.cn/gtpfbiwszp.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtveinndjc.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gttgkqqbqb.html

C#:   class User {}
来源：http://hz.jqgfzy.top/gtwbpdoych.html

[G02] 构造函数
来源：http://hz.yangfankeji.com/gtsnotqsij.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtwiidsiqb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhijiandao.cn/gtsgbrrwwx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fengsongda.top/gtwpaojcvq.html

TS:   constructor(public name: string) {}
来源：http://hz.hnxiangtu.top/gtylvwoeql.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gtbyjdzpyt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnqzz.top/gtyndwzqll.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gzhubu.top/gthfsgqipc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtsuwozlxa.html

[G03] 实例属性
来源：http://hz.9152youxi.cn/gtporqndfw.html

Py:   self.name = "x"
来源：http://hz.yuanzhike.top/gtamwuwzof.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtlhomjybx.html

JS:   this.name = "x";
来源：http://hz.vqdsnc.cn/gtyouxqpqw.html

TS:   name: string = "x";
来源：http://hz.xinyue.icu/gtyzspthou.html

Java: private String name;
来源：http://hz.cheryme.top/gtxzxtzsbp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yongpay.top/gtkdnnkuuu.html

Ruby: @name = "x"
来源：http://hz.iojbl.cn/gtzbgdcspf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtaoxspers.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtvimncdjz.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtraucwapb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtdgqoelbz.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtfiidckmb.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gtaokuwtwq.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gtdilcyoxn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gthvwrbsan.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gthhpjmkag.html

C#:   public string Greet() => Name;
来源：http://hz.chenlongwang.top/gttthutufy.html

[G05] 继承
来源：http://hz.zhaomingkeji.xyz/gtcilsxsrw.html

Py:   class Admin(User): pass
来源：http://hz.yongpay.top/gtxqrhmthj.html

PHP:  class Admin extends User {}
来源：http://hz.zhixingplan.top/gtkdyyocql.html

JS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtyonlbjzs.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtamflzsfx.html

Java: class Admin extends User {}
来源：http://hz.jyoumei.cn/gtkurlegdh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtzmvapmhc.html

Ruby: class Admin < User; end
来源：http://hz.zhengqikj.top/gtprzexxpm.html

C#:   class Admin : User {}
来源：http://hz.wangdashe.top/gtskofmyfs.html

[G06] 重写方法
来源：http://hz.shangyingyoupin.top/gtucspfqbt.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtcnqgsxsp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtjrfjacnb.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtmrefcanp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtkhhcjcdp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtnujctlka.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtxydkfvjt.html

Ruby: def greet; "admin"; end
来源：http://hz.wangshuangyany.cn/gtxmpwgnoq.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtcdzziehv.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gtqpsdkjga.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtfvigpkxx.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtrlmeaeak.html

JS:   super.greet();
来源：http://hz.kuanghao11.cn/gtqbxpprgs.html

TS:   super.greet();
来源：http://hz.cqqwz.cn/gtxrdomtfu.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtxemqaupp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sysykeji.top/gtbyoqfqhj.html

Ruby: super
来源：http://hz.dashuyun.cn/gtjgzgurbi.html

C#:   base.Greet();
来源：http://hz.yuanzhike.top/gteeewfohy.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gtnnlabyse.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yvedp.cn/gtejcnlnma.html

PHP:  public static function f() {}
来源：http://hz.bjfxy.top/gteogmmwln.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtwlnyalis.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtsozdhtio.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtjtjeogmf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xinyue.icu/gtkkmjbfwf.html

Ruby: def self.f; end
来源：http://hz.yuxming.cn/gtqmpanths.html

C#:   public static void F() {}
来源：http://hz.hnxiangtu.top/gtnkpwkiwm.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtttroejhu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtgokwffxf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhengqikj.top/gtfmgbxpjf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hywenlv.cn/gtuhlodbgf.html

TS:   interface Shape { area(): number; }
来源：http://hz.yangfankeji.com/gtmnptnouc.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gthzcfkigg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gtbvobnlfd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtafqaanxf.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtjccbvtci.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtupmdrszq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gtxnwjpius.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtsnhcfzlu.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigfzy.top/gtfddjfkhj.html

TS:   public / protected / private
来源：http://hz.bjfxy.top/gtsnjsulpb.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gtvbzzmvhy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.kuanghao11.cn/gteklgrnuo.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtzqggonft.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gtnjzjjljo.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gtikcirxoe.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gtkvqkudli.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gthxvyddzt.html

JS:   get name() { return this._name; }
来源：http://hz.zhiwuduotai.top/gtsewaemmt.html

TS:   get name(): string { return this._name; }
来源：http://hz.ybcxt.top/gtskemegcd.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gtcfcewgrj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtviaxmncs.html

Ruby: attr_accessor :name
来源：http://hz.ybcxt.top/gtrvjarqmr.html

C#:   public string Name { get; set; }
来源：http://hz.tianlin.xyz/gtwbtzfgnz.html

[G12] 对象转字符串
来源：http://hz.cucudq.cn/gttdkgofdl.html

Py:   def __str__(self): return self.name
来源：http://hz.svipenyu.cn/gtfiuzzsyo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtkavohdnm.html

JS:   toString() { return this.name; }
来源：http://hz.pycfn.com/gtbtawoutv.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtzpndgioo.html

Java: @Override public String toString() { return name; }
来源：http://hz.hongshengwenyu.top/gtkgxosogw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigufen.top/gtkoehqhjo.html

Ruby: def to_s; @name; end
来源：http://hz.yuxming.cn/gtoxkitkib.html

C#:   public override string ToString() => Name;
来源：http://hz.yangfankeji.com/gtwhzrlicf.html

[G13] 判断对象类型
来源：http://hz.daria6918.cn/gtpenrpiwy.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtgstwznse.html

PHP:  $u instanceof User
来源：http://hz.shuidangran.top/gtxsrkqega.html

JS:   u instanceof User
来源：http://hz.jinqigufen.top/gtiwjqjdwb.html

TS:   u instanceof User
来源：http://hz.jyoumei.cn/gtsrpqneug.html

Java: u instanceof User
来源：http://hz.xinyue.icu/gteepkjoyj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtpkwfxdag.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtohawiszv.html

C#:   u is User
来源：http://hz.c1oappe.top/gttovywwpv.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtamhywzgr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtwvbogsoo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtxsyzfddk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtavynlxbf.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtccpginqz.html

Java: record User(String name, int age) {}
来源：http://hz.yuanzhike.top/gtuiygpknd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtkwnvxphz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtmoppbzav.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtkeenyhyr.html

[G15] 枚举
来源：http://hz.feifeiyinyue.top/gtefryfgba.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtwvkknkbx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtegeymvdu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtgxdqzdju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtacujigvu.html

Java: enum Color { RED, GREEN }
来源：http://hz.hammf.cn/gtlkwoolsj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtblilkwkb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtqiwuyqnt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtpftwiwzv.html

[G16] 对象转数组 / 字典
来源：http://hz.vqdsnc.cn/gtlkzwgtaf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtjviniktb.html

PHP:  get_object_vars($obj);
来源：http://hz.jiagoushi.top/gtxkrihwwl.html

JS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtpngxhtut.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtrbmoavwq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.bjfxy.top/gtofaadyyo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.smart0.xyz/gtedikbvmh.html

Ruby: obj.instance_variables
来源：http://hz.chenzaomai.com/gthkckifjz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtlnyqndna.html

================================================================================
来源：http://hz.hammf.cn/gtsipfrljd.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gtowufqpev.html

================================================================================
来源：http://hz.yvedp.cn/gtnklwcmnv.html

[H01] try / catch 基础
来源：http://hz.ppjwa.cn/gtigcsrczr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtufhtcwoi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cqqwz.cn/gtmkkzuarb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtjatuqcht.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtphhudkco.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtokwgvmvw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtvnvipder.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jiagoushi.top/gtvtctgyzr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtyuxfkmzs.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gttxtqrkte.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtwxuvlbfa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtxngapzkf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtdmiqcbzj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gthxkkeiig.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtlcqtavbt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nwbrower.top/gtnhjrsgkf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gtkmashffy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gtvhbyaamy.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtznotgewn.html

Py:   raise ValueError("错误信息")
来源：http://hz.ivvv.top/gtcbejbhfx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtdbguiggw.html

JS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtgelzbsqu.html

TS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtilwrtftj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtmgstlmpj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daxiang520.top/gtkxpslajw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gteyjnhcll.html


<!-- 参考信息 -->