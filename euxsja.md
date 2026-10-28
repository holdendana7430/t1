代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtcstpwiie.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtlpleqfne.html

Java: s.lines().toList()
来源：http://hz.jlsjyb.cn/gtohxnhwzw.html

Go:   strings.Split(s, "\n")
来源：http://hz.hammf.cn/gtvmtoliwa.html

Ruby: s.lines
来源：http://hz.guowangkeji.top/gtvkokmrco.html

C#:   s.Split('\n')
来源：http://hz.52xcode.cn/gtpzwrxnhh.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtdpcxxkqu.html

Py:   if not s:
来源：http://hz.yanxiufei.cn/gtgntcaljs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtmuookqgd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cucudq.cn/gtewwjbemz.html

TS:   if (s === "") {}
来源：http://hz.nanxinkj.top/gtokhfzszv.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtnjwkijwz.html

Go:   if s == "" {}
来源：http://hz.zycfv.cn/gtszjacyvc.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtpgwvhqzc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhoulong.xyz/gthixdxnjy.html

[E21] 超长截断加省略号
来源：http://hz.hammf.cn/gtomdsfesb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtcxpcvxfl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtwsxjdhfx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtmtbtepby.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtitgapoqe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtcwhavted.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtvusebhyi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtwujjxped.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtqkwnbuiw.html

[E22] 字节长度与字符长度
来源：http://hz.hammf.cn/gtezsriqzj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fzhhl.top/gtirybmska.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sysykeji.top/gtmdaienho.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtftjhfxez.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gteuwedmlx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtomwdjjhz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.havefunace.top/gtaptgqvwp.html

Ruby: s.bytesize;  s.length
来源：http://hz.fzhhl.top/gtvornssut.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gtfgkznfwl.html

================================================================================
来源：http://hz.yonumen.top/gtngftsavv.html

F. 文件与目录
来源：http://hz.yvedp.cn/gtriafyuug.html

================================================================================
来源：http://hz.xuanzx.com/gtlyzpegns.html

[F01] 读取整个文件
来源：http://hz.nwbrower.top/gtzbccakqk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.havefunace.top/gtujavpstg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yvedp.cn/gtdvvrmzcj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ywan-chungtsiang.top/gtzvfpslwm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gthywgvofw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtyjvkrxla.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daria6918.cn/gtdyljzapi.html

Ruby: File.read("a.txt")
来源：http://hz.zhijiandao.cn/gtyetwhrne.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cashguo.top/gtosqcdpbk.html

[F02] 逐行读取文件
来源：http://hz.gotoacloud.top/gtrdrsyaiv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenlongwang.top/gtkztbxhit.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yanxiufei.cn/gtmqamuvgm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtdkkbvrks.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtkxxpqgpg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtnuvxrcnp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gtqjsjhsmw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuanzhike.top/gtrbdzejsz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.feifeiyinyue.top/gtialhaxdi.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gtcbxmhfgx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.smart0.xyz/gtrfcyejvd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gtgbieubjy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtypsomuon.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtrhhzftmz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fzhhl.top/gtmlqkvgmv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yuanzhike.top/gtkousviaw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.bjfxy.top/gtzdzuwsgf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtqqddgikc.html

[F04] 追加写入文件
来源：http://hz.aizwys.cn/gtotuwjtfo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cdnleiting.top/gtpeicypwu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hongshengwenyu.top/gtffhdzimx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtuzpeannq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtxuseuojz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.bjfxy.top/gtwzvylugy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yangfankeji.com/gtyeaazljk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtcedfwhoc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangshuangyany.cn/gtnwobujzx.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gtnvmptvnc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtqwzrnypb.html

PHP:  file_exists("a.txt");
来源：http://hz.mhx1999.top/gtbajmwkcf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtiwaozfpl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtdsankoyv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtdahygkae.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jyoumei.cn/gtffkkapgi.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhiwuduotai.top/gtfjioesre.html

C#:   File.Exists("a.txt")
来源：http://hz.sweek.top/gtnnnqcmpf.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtnsvkvvad.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gteuulpywl.html

PHP:  unlink("a.txt");
来源：http://hz.zhengqikj.top/gtqcgszayq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtylkrovgo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtpbapgihi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtkgeavcrk.html

Go:   os.Remove("a.txt")
来源：http://hz.mhx1999.top/gtvnpriyzz.html

Ruby: File.delete("a.txt")
来源：http://hz.shzxlz.cn/gtdpgpzess.html

C#:   File.Delete("a.txt");
来源：http://hz.sufxvd.cn/gtrumuenur.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtmscqghzh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gtrlroiaay.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgfzy.top/gtqwoiaqyb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtzgbqdvcd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtadpupcal.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtjgljaxrg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gtnsphqonq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xziqi.cn/gthqziwybt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yanxiufei.cn/gtcvvgpqcm.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gthjdyeayo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtxiemqslx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtnnggeckm.html

JS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gttisfwynl.html

TS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gtxhakcybc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtjtvapwwb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tanke756.top/gtnfybvcun.html

Ruby: Dir.children("dir")
来源：http://hz.fzhhl.top/gtiqvhqiuj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xinyue.icu/gtfjfqwbet.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtudeaifmi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.iojbl.cn/gthnuclsnj.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtdfbhqqwq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtwvrltpyl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtcxtxdnuk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtqnyoafss.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtygoosdeh.html

Ruby: File.size("a.txt")
来源：http://hz.zhixingplan.top/gtqzebqyij.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ywan-chungtsiang.top/gtmxdlhtju.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhoulong.xyz/gttcawewcg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gthaacssfl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cdnleiting.top/gtvbcuflos.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtwydjreym.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtfidahdyv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhoulong.xyz/gtrrvrfbep.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nwbrower.top/gtnhwdwgza.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gthwuctjei.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gtrjprxitl.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gtgypnsezi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gthjeintgy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tian-w.cn/gtluixmyjp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtvcgxotey.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtlksyntht.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtpvwuiyru.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yangfankeji.com/gtgyaqnrjc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtfaffsrjs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtfvnsfvrm.html

[F12] CSV 读写
来源：http://hz.hongshengwenyu.top/gtdsrgfzzk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhongyouzk.top/gtwdrqtebl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sysykeji.top/gtwtyirvjc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.0kj1m.cn/gthrzehbri.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gtkoermpou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtodfoqxnh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenjidiqi.icu/gtxhdsqsuj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtvqiciutj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuanzx.com/gtjnrrwnhd.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkdqndhfk.html

G. 面向对象
来源：http://hz.yuxming.cn/gtkcmivalz.html

================================================================================
来源：http://hz.sweek.top/gttzmtbyhy.html

[G01] 定义类
来源：http://hz.havefunace.top/gtvtoyulhl.html

Py:   class User: pass
来源：http://hz.xziqi.cn/gtayjahzmi.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtvmmikylr.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtlrcialty.html

TS:   class User { name: string = ""; }
来源：http://hz.guowangkeji.top/gtqeiqqgud.html

Java: class User {}
来源：http://hz.9152youxi.cn/gtjkyixdiu.html

Go:   type User struct { Name string }
来源：http://hz.gzhubu.top/gtwxytvhrb.html

Ruby: class User; end
来源：http://hz.havefunace.top/gtykebiarh.html

C#:   class User {}
来源：http://hz.birdmap.top/gtjjjlqegx.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gtlmhatkuc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zycfv.cn/gtonyhydbx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhaomingkeji.xyz/gtnaygpyqp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtljdwzzgm.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258888.top/gtfivqyluq.html

Java: User(String name) { this.name = name; }
来源：http://hz.redwolf501.top/gtbddbumbi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtxlybcgum.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxuanxn.top/gtxvodxkyg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtwoqjkyqy.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtsizrwunu.html

Py:   self.name = "x"
来源：http://hz.sufxvd.cn/gtaclcgunj.html

PHP:  public string $name = "x";
来源：http://hz.hysaishi.cn/gtfhggxjwn.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gttlekhipk.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gtarwgpzdo.html

Java: private String name;
来源：http://hz.0kj1m.cn/gtssjtzldb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtxhukercj.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtjjzsbnua.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gtipomxafd.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtvtedzhgo.html

Py:   def greet(self): return self.name
来源：http://hz.chenjidiqi.icu/gtbjvjhuhp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtfdrqbrar.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtkjyazyqv.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj202588.top/gtcupzrump.html

Java: String greet() { return name; }
来源：http://hz.yangfankeji.com/gtjlylfyko.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tianlin.xyz/gtilabmmif.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtukgbccdz.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtivzgxwra.html

[G05] 继承
来源：http://hz.yueranfly.top/gtgnzhqxfm.html

Py:   class Admin(User): pass
来源：http://hz.hfpthk.cn/gttpbuzlqc.html

PHP:  class Admin extends User {}
来源：http://hz.c1oappe.top/gteukmhcvl.html

JS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtcdwgkfck.html

TS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtbswzrwia.html

Java: class Admin extends User {}
来源：http://hz.shzxlz.cn/gtluhflvqf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtzkhqlnct.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gtxkrwuacp.html

C#:   class Admin : User {}
来源：http://hz.sxryk.cn/gtdlnkvufn.html

[G06] 重写方法
来源：http://hz.sysykeji.top/gtejdzseqz.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gtltwbmgvt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtldsnqzbh.html

JS:   greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtszewssrb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtdiqydlak.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtwzjkciwe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtlfamxjps.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtjmnzmkby.html

C#:   public override string Greet() => "admin";
来源：http://hz.gogol.net.cn/gtfrzplzoh.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtyazgpzuh.html

Py:   super().greet()
来源：http://hz.daxiang520.top/gttmnmerph.html

PHP:  parent::greet();
来源：http://hz.svipenyu.cn/gtytrgkvqr.html

JS:   super.greet();
来源：http://hz.snrcjt.cn/gtparzorfg.html

TS:   super.greet();
来源：http://hz.yj20258888.top/gtifkwtrhm.html

Java: super.greet();
来源：http://hz.haohaochexian.top/gtgxgjzrmw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtammycswp.html

Ruby: super
来源：http://hz.hysaishi.cn/gtfkjcloej.html

C#:   base.Greet();
来源：http://hz.wangdashe.top/gtgulhypsl.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtumflgini.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shuidangran.top/gtiffcnpcb.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtilftnbwi.html

JS:   static f() {}
来源：http://hz.aibaodan.cn/gttllbtlvu.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtccxlysvc.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtzztvxmgg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtfudlazpp.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gtjmmxglys.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtdhhevtkg.html

[G09] 接口 / 抽象类
来源：http://hz.gogol.net.cn/gtfafghjem.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gttlzbtzec.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxinkj.top/gtviqpltpx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtlujublor.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtvysynxrd.html

Java: interface Shape { double area(); }
来源：http://hz.dianchejie.cn/gtnbteiwsn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gttqgduiyc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtaipezppb.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gtubmmvwru.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtnhinvsmk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigufen.top/gtgzsfmmuj.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtintkfege.html

JS:   #private 字段；其余公开
来源：http://hz.haohaochexian.top/gtqwbxjkfe.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtmocqyrfl.html

Java: public / protected / private / 默认包级
来源：http://hz.zhongyouzk.top/gtdidqxpik.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtedrfktxu.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gthyvxstvl.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtwmgmmnkf.html

[G11] getter / setter
来源：http://hz.jqgufenzy.top/gttwssjzvs.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtzzxkzkgu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtlgrvsqdq.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtffrknkrk.html

TS:   get name(): string { return this._name; }
来源：http://hz.yonumen.top/gtrlhdtilu.html

Java: public String getName() { return name; }
来源：http://hz.ppjwa.cn/gtjbqgqbhb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtvmmuxpvs.html

Ruby: attr_accessor :name
来源：http://hz.ppjwa.cn/gthzizpqug.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtrhmkcriu.html

[G12] 对象转字符串
来源：http://hz.zdqjudy.top/gtibplwjcm.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtqfwkmhzi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtqorumxql.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigfzy.top/gtqicgwudf.html

TS:   toString(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtbbbdahxh.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtrwvljsna.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guannengcc.top/gtoxymfbnw.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtthucqeod.html

C#:   public override string ToString() => Name;
来源：http://hz.svipenyu.cn/gtmsdmxtlp.html

[G13] 判断对象类型
来源：http://hz.zhongyouzk.top/gtamvslsiz.html

Py:   isinstance(u, User)
来源：http://hz.gzhubu.top/gtlhfnfadl.html

PHP:  $u instanceof User
来源：http://hz.gaohongyu789.top/gtwprjjkui.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtksytxnny.html

TS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtetpdpbpg.html

Java: u instanceof User
来源：http://hz.quarkkingdee.top/gtobnjktdv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gtlpcabnkm.html

Ruby: u.is_a?(User)
来源：http://hz.ivvv.top/gthngpexkz.html

C#:   u is User
来源：http://hz.guowangkeji.top/gtlsrbpjwl.html

[G14] 数据类 / record
来源：http://hz.ydzc1.top/gtnugarxpn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtyxmhqjno.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gaohongyu789.top/gtiymjyexz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtcbzkhchw.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gttivagqqz.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtmuixcbua.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtacxwqmvp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hywenlv.cn/gtesytqobu.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtvkolgpzm.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtvmvomhpx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhongyouzk.top/gtankguvup.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cqqwz.cn/gtzuqoiaok.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtdpkxxmda.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtcpqntore.html

Java: enum Color { RED, GREEN }
来源：http://hz.cashguo.top/gtlyfhmolc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtfoomobqe.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xylfe.cn/gtaerisxhg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtdjzplljg.html

[G16] 对象转数组 / 字典
来源：http://hz.guowangkeji.top/gtlrzknspz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtpgqxkfai.html

PHP:  get_object_vars($obj);
来源：http://hz.shuidangran.top/gtpjfogljt.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtacqmhxre.html

TS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtshnmysca.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gtqxguthzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtaxvuulos.html

Ruby: obj.instance_variables
来源：http://hz.zhijiandao.cn/gttmuzjpom.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenjidiqi.icu/gtnfycnuni.html

================================================================================
来源：http://hz.meibo888.top/gtpxxljjrl.html

H. 异常与错误处理
来源：http://hz.yangfankeji.com/gtouoyrasw.html

================================================================================
来源：http://hz.snrcjt.cn/gturwudqbp.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtdxcbzfkq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aizwys.cn/gtorbjabem.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtpfwfplal.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtgpdlzqds.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtoxzejvzc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtusfvlfxt.html


<!-- 参考信息 -->