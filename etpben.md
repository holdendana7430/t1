代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtttiahqxy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hysaishi.cn/gtkdeyjomg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gtlmjuwfif.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtfuwqvzgh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtmhtkjwwr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangdashe.top/gtlwbdvgsl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guowangkeji.top/gtmzacyxkc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtlibrpiul.html

[E22] 字节长度与字符长度
来源：http://hz.gaohongyu789.top/gtwuqmhiyl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258888.top/gtfombftmx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ivvv.top/gtfzhgyhbv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtbagraric.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtqwgruyao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtebhvxhrz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtrmqxpqtp.html

Ruby: s.bytesize;  s.length
来源：http://hz.tanke756.top/gtvvdbbnab.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtxduxeltn.html

================================================================================
来源：http://hz.xuanzx.com/gteifoglyy.html

F. 文件与目录
来源：http://hz.sweek.top/gttqksaxhx.html

================================================================================
来源：http://hz.jinqigufen.top/gtlpovqjhh.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtozjchmsc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhongyouzk.top/gtlnhgajax.html

PHP:  file_get_contents("a.txt");
来源：http://hz.svipenyu.cn/gtkvvpgxas.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shanyushiyangkeji.top/gtcmutmavy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shangyingyoupin.top/gtqpihuvrt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtwwpellad.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtpjkvisie.html

Ruby: File.read("a.txt")
来源：http://hz.yongpay.top/gtjwakhmiy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtpbgcguhm.html

[F02] 逐行读取文件
来源：http://hz.shuidangran.top/gtcrrlxasn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinghuilouyu.cn/gtxkhbqquy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yonumen.top/gtmjpylnxo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtiwzoeqbr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtaujhgwbh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtjphcsscm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtqcbnzjqn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.316326.xyz/gtuvudsbfx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hfpthk.cn/gttwxbhlrk.html

[F03] 写入文件（覆盖）
来源：http://hz.cqqwz.cn/gtgqckeidd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtpxujrjft.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sysykeji.top/gthlbowmzc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtwfnlolcw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtpdzresbt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.feifeiyinyue.top/gtimcszddv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtszqzbcoc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xylfe.cn/gtjeprbjlt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtujmemsar.html

[F04] 追加写入文件
来源：http://hz.ydzc1.top/gtryvrvevs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydzc1.top/gtywwncwwt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gtzkcxbpyk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtltqsrdus.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtwamepezc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gttuhyvwzb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cheryme.top/gtlqnqovfk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtpoewgzvf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtoxqjhgqy.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtqlgcplyq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxuanxn.top/gtnvsbsjcg.html

PHP:  file_exists("a.txt");
来源：http://hz.fzhhl.top/gtgzzigrla.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gthkhxyfsg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gthnagduuq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtqqvlvujx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hysaishi.cn/gtzabiiltb.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtrdidknmi.html

C#:   File.Exists("a.txt")
来源：http://hz.bjfxy.top/gtgpjfqspu.html

[F06] 删除文件
来源：http://hz.nwbrower.top/gtrzmzfaab.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtxbrbycin.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gtaqjdrnig.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guowangkeji.top/gtzvqkayjk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtpreuemnx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtomryidid.html

Go:   os.Remove("a.txt")
来源：http://hz.fzhhl.top/gtzwwotfiw.html

Ruby: File.delete("a.txt")
来源：http://hz.meibo888.top/gtbqgdxyqh.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtfnsqjjka.html

[F07] 创建目录（含多级）
来源：http://hz.yvedp.cn/gtzwqmzwmd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dianchejie.cn/gtpihzqnri.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtpgtgmfhp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtpxzvhuks.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtddmwzibe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jyoumei.cn/gtimoklwwh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.smart0.xyz/gtklxcaefg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jyoumei.cn/gtwllghiuz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gzhubu.top/gtnjuaspcm.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gtsvldszoo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cqqwz.cn/gtmuclmgna.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhixingplan.top/gtgwtqzvbh.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtzfcyammj.html

TS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtplmxyscl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.tian-w.cn/gtivinadvi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gtrghsyrdz.html

Ruby: Dir.children("dir")
来源：http://hz.shuidangran.top/gttdcjhjzt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtnhpdsilb.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtkoaqcgax.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xziqi.cn/gthhppxuze.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtdpgkvflt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gthkopmoag.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtmudtcolq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtbxhxgolg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenlongwang.top/gtyatzfaqf.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gttlsvlzli.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.c1oappe.top/gtwuclwnkb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xziqi.cn/gtbdflccre.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtzftriaqe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gzhubu.top/gtbzgumtee.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtcrddmduj.html

TS:   path.extname("a.txt")
来源：http://hz.jiagoushi.top/gteafqxzbt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtwjxmozvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtxxtcbeya.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gthdlfplhe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jqgfzy.top/gtznfitjze.html

[F11] 复制与移动文件
来源：http://hz.jinghuilouyu.cn/gteouhpycq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtfouzkcqs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtdlfpfmke.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtgluqglss.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtmwpugyab.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gogol.net.cn/gtbfdroejw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtdigjjyaz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtgtriomuq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.bjfxy.top/gtjjbsnnxc.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gtxspwbujq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtoxvymsca.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtqgiubgod.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gtxrycqmde.html

TS:   // 同上
来源：http://hz.shzxlz.cn/gtlrehnsmy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtbkzhbayv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gttubshsgl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtnouqlwpg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuanzhike.top/gtfatrawrg.html

================================================================================
来源：http://hz.jiagoushi.top/gtbexmdnpq.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtlngfpgbh.html

================================================================================
来源：http://hz.cucudq.cn/gtolozbwcv.html

[G01] 定义类
来源：http://hz.wangshuangyany.cn/gtkfbewreh.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtgozmzlws.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtrjmjatxi.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtuhymmpjo.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gthkqjyynu.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtshsuofbx.html

Go:   type User struct { Name string }
来源：http://hz.jqgfzy.top/gtfxurkebm.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtucuyovmq.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtzimhyugz.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gtalcpzgdu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtpjgifiat.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tanke756.top/gtufklpeuf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtkamhpfpb.html

TS:   constructor(public name: string) {}
来源：http://hz.iojbl.cn/gtnoqesylc.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtlaeljhay.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgufenzy.top/gtpmpppkha.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhixingplan.top/gtqtptftwt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jlsjyb.cn/gtnonpiyec.html

[G03] 实例属性
来源：http://hz.shanyushiyangtech.top/gtlqnsrkdd.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtpbrpzlio.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtmsrrykmj.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtuunbtvos.html

TS:   name: string = "x";
来源：http://hz.316326.xyz/gtiixzxpff.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtypnzvmov.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtvadisebc.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gtysytsxpx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.andypj.xyz/gtoentibnn.html

[G04] 定义方法
来源：http://hz.vqdsnc.cn/gtklowwwzd.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtehibkxms.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtqesggbei.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtjkjiiyqy.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtcsaeszpg.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gttaljnprm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydzc1.top/gtqorozqio.html

Ruby: def greet; @name; end
来源：http://hz.xuetiantiany.cn/gthrucsyzc.html

C#:   public string Greet() => Name;
来源：http://hz.sxryk.cn/gtajmqjvcs.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtsjfvsczx.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtbfklredq.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtqxlrhkit.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtvlvjmatm.html

TS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtxmjlhkid.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtpebxtsuq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dianchejie.cn/gtpmjiddeo.html

Ruby: class Admin < User; end
来源：http://hz.xuetiantiany.cn/gtkpanzvyh.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtrvftnklg.html

[G06] 重写方法
来源：http://hz.mhx1999.top/gtexexxajm.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtmbaudvru.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtnfqdzizk.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gthdietrtf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtnjnvbwhf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtafwoheoj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxuanxn.top/gtobcrikba.html

Ruby: def greet; "admin"; end
来源：http://hz.haohaochexian.top/gtaijfygfx.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtgszvfdma.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtcvptzonc.html

Py:   super().greet()
来源：http://hz.haohaochexian.top/gtyqyxxqvm.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtsrwtatjf.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gtphguziiu.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gtcjhbpdhr.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtdnqlgczp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ivvv.top/gtkmqemwkf.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtewnpxiuf.html

C#:   base.Greet();
来源：http://hz.yanxiufei.cn/gthwjvpima.html

[G08] 静态方法与属性
来源：http://hz.yangfankeji.com/gtlekdoeje.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtycmfvrjb.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtpyerwkfr.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtgzpqmkfd.html

TS:   static f(): void {}
来源：http://hz.zhijiandao.cn/gtgqtkyudw.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtuedqnlsn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgufenzy.top/gtnbfkyrno.html

Ruby: def self.f; end
来源：http://hz.cucudq.cn/gtolokvhjg.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtefghcrgu.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtgejcxhhy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuxming.cn/gtimyfrrya.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fengsongda.top/gtchldesus.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtzluhyzuy.html

TS:   interface Shape { area(): number; }
来源：http://hz.guowangkeji.top/gtkpdpgekl.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtomvrjkqv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cdnleiting.top/gtxcolrvuo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gtcrwtvpzu.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtimzuhrqs.html

[G10] 访问控制
来源：http://hz.wangshuangyany.cn/gtvzdbzqqo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tianlin.xyz/gtoznogovf.html

PHP:  public / protected / private
来源：http://hz.havefunace.top/gtqkontqts.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtxxzmsnkx.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtuenlmeps.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gthecjttgh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jiagoushi.top/gtcgayjjfd.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtsvhdsnhs.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gtskoseyuc.html

[G11] getter / setter
来源：http://hz.yueranfly.top/gtoanxqnfm.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtaemcbuui.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.birdmap.top/gtmkkolpby.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtumyhxowg.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtetnwlolo.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtfhjnbzmi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtxecwleis.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtophrkbmo.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gtgbzogeek.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtzaxemdhb.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gtymuwrphg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtjisfoukx.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtisscxtjl.html

TS:   toString(): string { return this.name; }
来源：http://hz.ybcxt.top/gteqsmutjl.html

Java: @Override public String toString() { return name; }
来源：http://hz.yangfankeji.com/gtsvsdecia.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ehwqpu.com/gtujjrfsyl.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtttytjtiu.html

C#:   public override string ToString() => Name;
来源：http://hz.birdmap.top/gtmygnjszh.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gtronqngbu.html

Py:   isinstance(u, User)
来源：http://hz.cdnleiting.top/gtzejwzfxy.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtvdaucxyn.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtbqpvzjtb.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtbexngjtk.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtyjvyuver.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daxiang520.top/gtqjjnhchh.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtsbjslmph.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtnjhgupzm.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtolqjzsmt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtcyasljsx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cheryme.top/gtqfqcpnje.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtxdomlnws.html

TS:   type User = { name: string; age: number };
来源：http://hz.tanke756.top/gtpklxbgqk.html

Java: record User(String name, int age) {}
来源：http://hz.hywenlv.cn/gtvegkedkv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtrpvtofha.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtcbxoykif.html

C#:   record User(string Name, int Age);
来源：http://hz.mhx1999.top/gtujdqxbba.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtsrnwhjqw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtskljdhzh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtttfqflfs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtbxxqblmc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtzkqjpwom.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtswcmnfkc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gtflxgkdvy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cdnleiting.top/gtndpclhdj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtvmixkwrd.html

[G16] 对象转数组 / 字典
来源：http://hz.guannengcc.top/gtxpmualec.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sysykeji.top/gtmvdckbox.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtzqfbdxvs.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtwbxnwgvy.html

TS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtmpjmpzoc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigufen.top/gtzkbguetx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gtzstewljl.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtsppvwwjp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtiqxihftk.html

================================================================================
来源：http://hz.pycfn.com/gteiemoyik.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtrauskreo.html

================================================================================
来源：http://hz.xinyue.icu/gtpdisedoj.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gtumbfkrkc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtrmaydrsw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nwbrower.top/gtupzjcatr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtvureshwq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aibaodan.cn/gtpigfgfhs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tian-w.cn/gtawyiwkyw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtvdcxbpfh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.snrcjt.cn/gtpopuerni.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtyyawmnaw.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtktowihbk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.andypj.xyz/gtzaogclgf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtukpudyqa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gttdcmllja.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtvqpzceet.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtgccmfchh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtuoxgfyvz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtosoofftc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.birdmap.top/gtxggxdgzf.html

[H03] 主动抛出异常
来源：http://hz.yj20258.top/gtuiqtvyez.html

Py:   raise ValueError("错误信息")
来源：http://hz.quarkkingdee.top/gtqimyrkqr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtmoihyxsa.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtxuvkwuyk.html


<!-- 参考信息 -->