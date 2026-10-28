代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yongpay.top/gtzbzydacj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhijiandao.cn/gtulllkbxa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gthzfqpmex.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtrevdstwd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtymhyppgh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtxejjhfrv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhiwuduotai.top/gtlxdazvsh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cqqwz.cn/gtmapadmpx.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gtfxpdwldp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gthmbtgjrp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtdktbaydw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtpqrfqlhc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtzajbcofa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guannengcc.top/gtaquhfxrr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtyeuclbch.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gtenrilfyq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.svipenyu.cn/gtzwuhlzyw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtieidhvjl.html

F. 文件与目录
来源：http://hz.cqqwz.cn/gtobjgpfvj.html

================================================================================
来源：http://hz.hnqzz.top/gtvbuvudxy.html

[F01] 读取整个文件
来源：http://hz.jianghu66.top/gtqjwzbgnx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xziqi.cn/gthlccwxwp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtswxksehl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cheryme.top/gttdlsxvak.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jlsjyb.cn/gtkzkndfqr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtximymalb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jinghuilouyu.cn/gtutckxgvm.html

Ruby: File.read("a.txt")
来源：http://hz.zhixingplan.top/gtwykndupp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtyqjyibkn.html

[F02] 逐行读取文件
来源：http://hz.jianghu66.top/gtrpmssjfh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hywenlv.cn/gtjfufjurd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xingfuxueyuan.xyz/gtczvimjjt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gtnpaabpmf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtqgewpbmy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtzsqqqgln.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fengsongda.top/gtpeihwoid.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtelczmvdo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtvcebzbgy.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gtinvmcekg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ivvv.top/gtmxhjrmgo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenzaomai.com/gtflefenwp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtqfyiixyo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gttjfwldzh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gtstdwbkkw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtgzwllsuh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gtgblekcvl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtilkbpetb.html

[F04] 追加写入文件
来源：http://hz.0kj1m.cn/gtemauovlt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gttnzcifeg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtewmtiiir.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtczroifmy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtozkojrru.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtqdlljvje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shangyingyoupin.top/gtxsudmopa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guannengcc.top/gtrfcifaql.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtteiniscj.html

[F05] 判断文件或目录是否存在
来源：http://hz.yvedp.cn/gttxxztnyo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtcvlsqygo.html

PHP:  file_exists("a.txt");
来源：http://hz.bjfxy.top/gtedhmwkms.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtuykkmfzg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtjshmbsdh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtukuressg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jlsjyb.cn/gtwskfbvqc.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtrnghizse.html

C#:   File.Exists("a.txt")
来源：http://hz.52xcode.cn/gttmnaudxb.html

[F06] 删除文件
来源：http://hz.ehwqpu.com/gtoponojbw.html

Py:   os.remove("a.txt")
来源：http://hz.316326.xyz/gtsjyekejc.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gtgjvckgmw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtdfdhawgm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.316326.xyz/gtmzhynwom.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtsuccjeum.html

Go:   os.Remove("a.txt")
来源：http://hz.ehwqpu.com/gtnhssznjh.html

Ruby: File.delete("a.txt")
来源：http://hz.dianchejie.cn/gtypkuvnhi.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtzldturgv.html

[F07] 创建目录（含多级）
来源：http://hz.hongshengwenyu.top/gtdtuciidl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cucudq.cn/gtkxlxuvwe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yonumen.top/gtpzhgifif.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guowangkeji.top/gtwrrkbhfw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gttatpvajl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gttvhuiidu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtuqxqnhwg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtlcujklvh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangshuangyany.cn/gtevvzqgwq.html

[F08] 遍历目录
来源：http://hz.yanxiufei.cn/gtgoiovrpx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhoulong.xyz/gtbbfjsnuh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gtbtabbxhf.html

JS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtfxipixnf.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtkwjldkqs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtdvlfhwhd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtgxtqpyga.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtvibeefqo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sysykeji.top/gtwaggyahx.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gthexzqtvm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nwbrower.top/gtblmcezvl.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtediejymq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtlqmryakw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtalzulimf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtxkgkpqvp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtfjkraxgy.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtenplucxi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gteaelvjju.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jlsjyb.cn/gtqtsyspkg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtbrjtmmkc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuxming.cn/gtqqyvexqn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtmqgirqdo.html

TS:   path.extname("a.txt")
来源：http://hz.gogol.net.cn/gtygmxkihl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtfkunzbfo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cdnleiting.top/gtngxnwfvs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtuwvvgmse.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yangfankeji.com/gtjvbinyim.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gtqpqnhpwn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtmztbcigt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tian-w.cn/gtkdlzhdot.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtpdtqgdsv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtihujtlkt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gtuuuxefel.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xinyue.icu/gtgomlzlot.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtjuqbqucp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cucudq.cn/gtauwpbwcg.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtldorcttj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sweek.top/gtynucdjai.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtgmwdpwpa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.9152youxi.cn/gtziuagtiy.html

TS:   // 同上
来源：http://hz.zhiwuduotai.top/gtxqrfguiq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.feifeiyinyue.top/gtbkwfqejz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xziqi.cn/gtlhthizae.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sysykeji.top/gtkityqbdi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtiepniccz.html

================================================================================
来源：http://hz.sufxvd.cn/gtnvxhrkbt.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gtwxshnakx.html

================================================================================
来源：http://hz.nwbrower.top/gtpuvkdmss.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtfmltxgeg.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtoaxhhqui.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtiwpbkuqv.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtngnvohlh.html

TS:   class User { name: string = ""; }
来源：http://hz.yonumen.top/gtpilibvao.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtzopaixid.html

Go:   type User struct { Name string }
来源：http://hz.jyoumei.cn/gtnhiopnko.html

Ruby: class User; end
来源：http://hz.shanyushiyangkeji.top/gtipwxygxw.html

C#:   class User {}
来源：http://hz.zhijiandao.cn/gtezkxdjfa.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtwurzvzmk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtpqenyxhg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgufenzy.top/gtaffhqiob.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtcbjjkjls.html

TS:   constructor(public name: string) {}
来源：http://hz.daxiang520.top/gttfnipvbc.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtiyawhoei.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtnprwshzc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gtngabeqhr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtfbpubvfp.html

[G03] 实例属性
来源：http://hz.sweek.top/gtjepawyfi.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtzbjloedd.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtkkifnhdw.html

JS:   this.name = "x";
来源：http://hz.jiagoushi.top/gtmkxghcdd.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtktndliss.html

Java: private String name;
来源：http://hz.gogol.net.cn/gtnafvfhbh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jyoumei.cn/gtciqdppqh.html

Ruby: @name = "x"
来源：http://hz.nanxinkj.top/gtlvxdnlmv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangshuangyany.cn/gtrioaghfd.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtlbyvdwlw.html

Py:   def greet(self): return self.name
来源：http://hz.jqgufenzy.top/gtzrdcetqo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtfsukiaqo.html

JS:   greet() { return this.name; }
来源：http://hz.kuanghao11.cn/gthofioixi.html

TS:   greet(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtopddhyfd.html

Java: String greet() { return name; }
来源：http://hz.birdmap.top/gtqcowmsfq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtyewxingq.html

Ruby: def greet; @name; end
来源：http://hz.yanxiufei.cn/gtwijypnkp.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gtqkheuasu.html

[G05] 继承
来源：http://hz.gaohongyu789.top/gtxipcqjof.html

Py:   class Admin(User): pass
来源：http://hz.hnxiangtu.top/gthpqjibbf.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtezncvejk.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtmclerxbr.html

TS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtdopyibgq.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtjskzhpih.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtctryqbyq.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtcwaeogwm.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gtjjdhxams.html

[G06] 重写方法
来源：http://hz.zhoulong.xyz/gtxsliakah.html

Py:   def greet(self): return "admin"
来源：http://hz.iojbl.cn/gtumvjbqre.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtdrwxamkk.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtmwyeyohq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtrxtkjxau.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtcwquxfsl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.birdmap.top/gtqaeumffx.html

Ruby: def greet; "admin"; end
来源：http://hz.hongshengwenyu.top/gtuzgyofdb.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtbzjpvphl.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtmekzmxqv.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtpcgspwal.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtxhkjksgu.html

JS:   super.greet();
来源：http://hz.gogol.net.cn/gtpvvpnlpb.html

TS:   super.greet();
来源：http://hz.pycfn.com/gtmuoxzdwo.html

Java: super.greet();
来源：http://hz.gaohongyu789.top/gtwnspfrda.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gtitvcndxx.html

Ruby: super
来源：http://hz.yvedp.cn/gtpgasjybt.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtrsuvfvqc.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gtjwuhdjzf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtiuqfjiuk.html

PHP:  public static function f() {}
来源：http://hz.c1oappe.top/gtmsbbzvqk.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtvfljhmqm.html

TS:   static f(): void {}
来源：http://hz.snrcjt.cn/gtzkrghelt.html

Java: static void f() {}
来源：http://hz.cashguo.top/gtyaxrwduk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangdashe.top/gtayirtxfp.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gthzduhadc.html

C#:   public static void F() {}
来源：http://hz.sweek.top/gtmmstjzof.html

[G09] 接口 / 抽象类
来源：http://hz.andypj.xyz/gtmgdzezcn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtalfhpvqu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxinkj.top/gthmmleljo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shuidangran.top/gttwbombij.html

TS:   interface Shape { area(): number; }
来源：http://hz.vqdsnc.cn/gtwcibuzbw.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtsigfzjun.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtjalntpdk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtamsqjlug.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtjywdtjtp.html

[G10] 访问控制
来源：http://hz.zhiwuduotai.top/gtkfmszymx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtpsdzikod.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtekowmyqw.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtkyngwnir.html

TS:   public / protected / private
来源：http://hz.jyoumei.cn/gtyhoftsxz.html

Java: public / protected / private / 默认包级
来源：http://hz.vqdsnc.cn/gtpgpoghkf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtuhmkvalt.html

Ruby: public / protected / private
来源：http://hz.wangdashe.top/gtenqxynle.html

C#:   public / protected / private / internal
来源：http://hz.snrcjt.cn/gttpjugfmd.html

[G11] getter / setter
来源：http://hz.yuanzhike.top/gtbglrevzx.html

Py:   @property 与 @x.setter
来源：http://hz.shzxlz.cn/gtyjqgajix.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtircsyuym.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtlyebzqsl.html

TS:   get name(): string { return this._name; }
来源：http://hz.xinyue.icu/gtzlcblzml.html

Java: public String getName() { return name; }
来源：http://hz.yuanzhike.top/gtwatkidji.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xziqi.cn/gtthmhuisr.html

Ruby: attr_accessor :name
来源：http://hz.sufxvd.cn/gtufjmmyhh.html

C#:   public string Name { get; set; }
来源：http://hz.chenjidiqi.icu/gtmqdehxrr.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gttmmhcrxt.html

Py:   def __str__(self): return self.name
来源：http://hz.zhengqikj.top/gtjhpzdrzg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtkjkbnzls.html

JS:   toString() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtrrdjhvpq.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtbutlihuv.html

Java: @Override public String toString() { return name; }
来源：http://hz.tianlin.xyz/gtigrifilw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtdimmaign.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gticpjnwlh.html

C#:   public override string ToString() => Name;
来源：http://hz.jlsjyb.cn/gtwamldhwm.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtlfdjyela.html

Py:   isinstance(u, User)
来源：http://hz.kuanghao11.cn/gtwrhspmdp.html

PHP:  $u instanceof User
来源：http://hz.jyoumei.cn/gtpbofvkwi.html

JS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtsttqmyvw.html

TS:   u instanceof User
来源：http://hz.hfpthk.cn/gtjybynheo.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtdevrbxdg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tianlin.xyz/gtlofvcfcu.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtlashhvxz.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtzygvmnvj.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtxkicvbxl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtwxwgtnsr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.quarkkingdee.top/gthoagrefr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gtldsbtgqp.html

TS:   type User = { name: string; age: number };
来源：http://hz.cqqwz.cn/gtccxqgscv.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtjdtrrxii.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gttdjcabtr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yangfankeji.com/gteskvyjfk.html

C#:   record User(string Name, int Age);
来源：http://hz.tianlin.xyz/gthlawjuhc.html

[G15] 枚举
来源：http://hz.feifeiyinyue.top/gtimnwmnvv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtxkfidsjh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.iojbl.cn/gtmmcotupl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gtwaybvhpf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtlimstdtu.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gtyhmhdfpv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtvmjpufpc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtlnxjxakx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtrqnbmbei.html

[G16] 对象转数组 / 字典
来源：http://hz.snrcjt.cn/gtwqjleiyf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtetuxezmv.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtxahtftok.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtrofboidv.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtkwgjjyck.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.316326.xyz/gtoomvwcbl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtpmtljhnk.html

Ruby: obj.instance_variables
来源：http://hz.birdmap.top/gtzvzznkjc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhongyouzk.top/gtxyylxfyh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbdowwdbc.html

H. 异常与错误处理
来源：http://hz.jqgfzy.top/gtcebmvrng.html

================================================================================
来源：http://hz.ivvv.top/gtitpixgrl.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtelkugeox.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gttpljnmun.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtjrzcrlat.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtkshixgph.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cashguo.top/gtflguztco.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtlfkroges.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtptvfbljc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yanxiufei.cn/gttyprfmyh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtpoepqmcu.html

[H02] finally / ensure 收尾
来源：http://hz.smart0.xyz/gtclwpmvoi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtahzxysjf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtwpcdfufq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtsugnfegm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtzjdftuxg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtbuqutlyo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtnpugxvvo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtlaqdbvuo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hysaishi.cn/gtgndudfmb.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gthdvalbnn.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuetiantiany.cn/gtxgbnafla.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtefhtzlag.html

JS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtjldxloxg.html


<!-- 参考信息 -->