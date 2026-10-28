代发 wailian999

Ruby: s.lines
来源：http://hz.wangdashe.top/gtzyaxslox.html

C#:   s.Split('\n')
来源：http://hz.xziqi.cn/gtcixublbn.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gteiagwjci.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtfsqqcxdg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aizwys.cn/gtmoljexkj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gteqhyiuvg.html

TS:   if (s === "") {}
来源：http://hz.yvedp.cn/gtingofspk.html

Java: if (s.isEmpty()) {}
来源：http://hz.mhx1999.top/gthxmxbpht.html

Go:   if s == "" {}
来源：http://hz.jinqigfzy.top/gtmgzpbdfg.html

Ruby: if s.empty?
来源：http://hz.xuetiantiany.cn/gtubtyvvke.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cheryme.top/gtctayhlci.html

[E21] 超长截断加省略号
来源：http://hz.iojbl.cn/gtmidkxnqi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhengqikj.top/gtgxazieze.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtzojwjxoc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtupikukci.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gtpxiidufi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtqoznjvrr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gthqljwgzx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.mhx1999.top/gtbujzmewy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shuidangran.top/gtmnxovjrp.html

[E22] 字节长度与字符长度
来源：http://hz.zhengqikj.top/gtrubvzski.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuetiantiany.cn/gthfayegri.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtogjjdvkp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtrtuygywy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtsbblqjke.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hfpthk.cn/gtbjdhiwnq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtqaajqmrj.html

Ruby: s.bytesize;  s.length
来源：http://hz.hnqzz.top/gtllatdgqw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtfuialbil.html

================================================================================
来源：http://hz.wangdashe.top/gtpfhbvoaw.html

F. 文件与目录
来源：http://hz.gzhubu.top/gtilzsccir.html

================================================================================
来源：http://hz.hammf.cn/gtncgrxtqn.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtodhxjtra.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnxiangtu.top/gtgelddvjo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gtfgnrputs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtdzllbbuj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.kuanghao11.cn/gttvxyvdih.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtxubrtmwl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gtycucruor.html

Ruby: File.read("a.txt")
来源：http://hz.jiagoushi.top/gthxqnaagx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shangyingyoupin.top/gtaqdcwthe.html

[F02] 逐行读取文件
来源：http://hz.tianlin.xyz/gtfuyzytjq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtdwxwvzjm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenlongwang.top/gthtqlletw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtrqwluapb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daxiang520.top/gthwixrahl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtnlbgpoxu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aizwys.cn/gtrafvctxr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shzxlz.cn/gtmmzmexge.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gttsdbwuiv.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gttcsljprv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guannengcc.top/gtrtwpchep.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtvrvbeogd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtmwgxpind.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtoxlxlpqw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.vqdsnc.cn/gtgoecjteo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aizwys.cn/gtzlsxziij.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jiagoushi.top/gterqwoecp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.52xcode.cn/gtifitlazy.html

[F04] 追加写入文件
来源：http://hz.hfpthk.cn/gtlnpvylyf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gthpxijefz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtjcfquhcl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtgwtixqtx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtnhoeuhze.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtzuewuijm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtiekfgiln.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pycfn.com/gttjjgcqap.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenzaomai.com/gtepehkuxw.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhixingplan.top/gtnxednsuu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jianghu66.top/gtvettmzgn.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtqhzjzdws.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gteelupcpp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gttsdfdkcq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtdqvnriks.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gterjnxayp.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gtyxwmfuwr.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigfzy.top/gtmkzhnbob.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtiolgcsnj.html

Py:   os.remove("a.txt")
来源：http://hz.gogol.net.cn/gtukufpkpj.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gtubxsazbk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zdqjudy.top/gtjssluika.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtwjqncjyz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtnadinexh.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtcfqorxbh.html

Ruby: File.delete("a.txt")
来源：http://hz.shuidangran.top/gtxmtfswiy.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gtwqzxhgaz.html

[F07] 创建目录（含多级）
来源：http://hz.shangyingyoupin.top/gtabhftgqe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cdnleiting.top/gtiqujyaed.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gtpwfpnpyp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gteopxvmgl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtlvzmkqhp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtmjsfrang.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hywenlv.cn/gtitweylaw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cqqwz.cn/gtxmnifjqf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtfjpsjsuc.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtrpnerwfe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtzqysjbul.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtfsfndbaj.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtkguxozhz.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtgqoouzun.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtmwsnghzw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtpewgftoi.html

Ruby: Dir.children("dir")
来源：http://hz.ehwqpu.com/gtrciekphe.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gtolaucqvq.html

[F09] 获取文件大小
来源：http://hz.hnxiangtu.top/gtonoijuso.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinghuilouyu.cn/gthveyfnza.html

PHP:  filesize("a.txt");
来源：http://hz.xuanzx.com/gthnihdina.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtukuhdoim.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtmspraepm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtfctezphp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258.top/gtvnvphrgf.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtlpwfguxj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtspmnmqob.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ehwqpu.com/gtesyizxsc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtbyxynydx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zdqjudy.top/gtaqiwazgu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtedvlmjcp.html

TS:   path.extname("a.txt")
来源：http://hz.yonumen.top/gttblqhuzr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gthcbvtojt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daxiang520.top/gttzzexywu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtthdnfkmn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pycfn.com/gtdatyosou.html

[F11] 复制与移动文件
来源：http://hz.zycfv.cn/gtqjzxegyo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtbwxdwtyi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ppjwa.cn/gtsliimzwu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gttknffgxe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtboerydbi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtsloehkfs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangtech.top/gtypvvvkef.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sweek.top/gtbkmmpuoy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jlsjyb.cn/gtghycvget.html

[F12] CSV 读写
来源：http://hz.zycfv.cn/gtdoozcyef.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hfpthk.cn/gtpzkxrrlz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtujeizrwz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gtykmybqon.html

TS:   // 同上
来源：http://hz.smart0.xyz/gtwvujqwds.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hammf.cn/gtfeffsqiq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtjnuzpgor.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hywenlv.cn/gtqwkpqmtk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangkeji.top/gtxiazwtmg.html

================================================================================
来源：http://hz.ydzc1.top/gtihzsshna.html

G. 面向对象
来源：http://hz.gzhubu.top/gtkdjmbsor.html

================================================================================
来源：http://hz.zhengqikj.top/gtjqfxfqry.html

[G01] 定义类
来源：http://hz.zhongyouzk.top/gtopvxbufo.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtpmdpsmtj.html

PHP:  class User {}
来源：http://hz.dashuyun.cn/gtoqllluto.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gtlxousinz.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtexmlblmi.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtwqepozri.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtyfhciqfc.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtpyjlmvuk.html

C#:   class User {}
来源：http://hz.chenzaomai.com/gtvkdmddda.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtjlfvaepq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtquxowdif.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fzhhl.top/gtwtravlph.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhijiandao.cn/gttgknorcn.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gthuoskjqt.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gtqhstnsiv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuxming.cn/gtnwgexghk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhixingplan.top/gtygltsnfr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj202588.top/gtzqhsqhhe.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtcbcxmcui.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtmkbnsuta.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtotbtzzos.html

JS:   this.name = "x";
来源：http://hz.bjfxy.top/gtaqsvukiy.html

TS:   name: string = "x";
来源：http://hz.chenzaomai.com/gtnsygqraj.html

Java: private String name;
来源：http://hz.yueranfly.top/gtqvmgrkuk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.snrcjt.cn/gtyfawaotq.html

Ruby: @name = "x"
来源：http://hz.birdmap.top/gtcbfpipei.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hongshengwenyu.top/gtefclqwjr.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtepiocsnc.html

Py:   def greet(self): return self.name
来源：http://hz.yuxming.cn/gtbqaawhuh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ivvv.top/gtxahlzxyw.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtugkmkwlb.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtcmtjbtni.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtrekqyotl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gthnflraon.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gtqtoafqxe.html

C#:   public string Greet() => Name;
来源：http://hz.mhx1999.top/gttrymmrje.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtxpsvsuvx.html

Py:   class Admin(User): pass
来源：http://hz.zhongyouzk.top/gtwzazumhp.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gtzqidlvmt.html

JS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtocrxwvhn.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtszvsgwfy.html

Java: class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtgpjvemyh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gteyuhiuih.html

Ruby: class Admin < User; end
来源：http://hz.jianghu66.top/gtmurwgmgs.html

C#:   class Admin : User {}
来源：http://hz.vqdsnc.cn/gtuldisgcl.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gtanhbnfut.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtxtpmtkpq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtkivnjfpw.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtbtebcnfa.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtzwcwjhvh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtmgmwthcn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tian-w.cn/gtmbgrvpyj.html

Ruby: def greet; "admin"; end
来源：http://hz.yueranfly.top/gttvymrhqi.html

C#:   public override string Greet() => "admin";
来源：http://hz.ppjwa.cn/gtgpnxpxuu.html

[G07] 调用父类方法
来源：http://hz.iojbl.cn/gtabnewbup.html

Py:   super().greet()
来源：http://hz.yj20258.top/gtvmqtbddc.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtpobqdcpy.html

JS:   super.greet();
来源：http://hz.nwbrower.top/gtzijbfqxz.html

TS:   super.greet();
来源：http://hz.0kj1m.cn/gthrxctgzk.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gttbnflhwq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtujuxhefk.html

Ruby: super
来源：http://hz.guowangkeji.top/gttdfgstcc.html

C#:   base.Greet();
来源：http://hz.yvedp.cn/gtsqjuxwjo.html

[G08] 静态方法与属性
来源：http://hz.nanxinkj.top/gtujhvgmzv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtgkozmsnp.html

PHP:  public static function f() {}
来源：http://hz.aibaodan.cn/gtnknolbjk.html

JS:   static f() {}
来源：http://hz.c1oappe.top/gtmbrtjvvu.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtnusjveky.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtuyndytoa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenjidiqi.icu/gtfgbnrajf.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtsbynoelx.html

C#:   public static void F() {}
来源：http://hz.sufxvd.cn/gtlmjesros.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtfacxromp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtqvfbqyyy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gaohongyu789.top/gtrpjrhihm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtwdbyqkay.html

TS:   interface Shape { area(): number; }
来源：http://hz.aizwys.cn/gtqtfcsnpf.html

Java: interface Shape { double area(); }
来源：http://hz.jlsjyb.cn/gtdncbzlia.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtkiybbjkb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydjk.org.cn/gtekryopda.html

C#:   interface IShape { double Area(); }
来源：http://hz.xylfe.cn/gtgnkazyef.html

[G10] 访问控制
来源：http://hz.ehwqpu.com/gttbivjspw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hongshengwenyu.top/gtkftvykbr.html

PHP:  public / protected / private
来源：http://hz.zycfv.cn/gtzijktmwm.html

JS:   #private 字段；其余公开
来源：http://hz.mhx1999.top/gtnobomjkl.html

TS:   public / protected / private
来源：http://hz.jlsjyb.cn/gtpfeedmwf.html

Java: public / protected / private / 默认包级
来源：http://hz.zhaomingkeji.xyz/gtingamvbd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258888.top/gtnmklgict.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtvavtbkzh.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtyspcjazm.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gtsprqaftl.html

Py:   @property 与 @x.setter
来源：http://hz.chenzaomai.com/gteoazfvzd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtmvbqzgsp.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtwfgjrqku.html

TS:   get name(): string { return this._name; }
来源：http://hz.aizwys.cn/gtrnjjcrpv.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtgfupnequ.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtfdjmolrz.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gttvfwdixy.html

C#:   public string Name { get; set; }
来源：http://hz.fzhhl.top/gtjyouwzwj.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtvajdmimt.html

Py:   def __str__(self): return self.name
来源：http://hz.ivvv.top/gtwhsxivse.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtbppnxfqg.html

JS:   toString() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtwxbnxlek.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gttbkgpciw.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtptalumdj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sysykeji.top/gtwghxdgcz.html

Ruby: def to_s; @name; end
来源：http://hz.sxryk.cn/gtkfekolxo.html

C#:   public override string ToString() => Name;
来源：http://hz.kuanghao11.cn/gtxoylygif.html

[G13] 判断对象类型
来源：http://hz.cucudq.cn/gtlcxuvmac.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtrlgmsrpt.html

PHP:  $u instanceof User
来源：http://hz.jiagoushi.top/gtxcwzlvbl.html

JS:   u instanceof User
来源：http://hz.xylfe.cn/gtyxtpuvmj.html

TS:   u instanceof User
来源：http://hz.zhixingplan.top/gtosytmxmt.html

Java: u instanceof User
来源：http://hz.daria6918.cn/gtotnxmmut.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtbasxgdtw.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtnnsusput.html

C#:   u is User
来源：http://hz.hammf.cn/gtpnysmccs.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtzjbjemig.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xziqi.cn/gtvmhuvhpl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtsqohwbqs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gtcbwddnba.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinyuanbaomall.cn/gtsaqyxmvs.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtfknneryo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtgwpxaugr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhongyouzk.top/gtaffvpvsz.html

C#:   record User(string Name, int Age);
来源：http://hz.ehwqpu.com/gttswrqmxn.html

[G15] 枚举
来源：http://hz.hammf.cn/gtktyrwruo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtbnzqqnyk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gtxetbocye.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.52xcode.cn/gtbcvamwtu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtfcjrasmb.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangshuangyany.cn/gtmjyjehwq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gtkmwlykaa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gttwguqpbn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtotbsbukm.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gtmownbgsp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jianghu66.top/gtuqiwuzra.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtggvnexvu.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtjalmtnqe.html

TS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtysbeyhyq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtkcnjojqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.iojbl.cn/gtwuvsfcpw.html

Ruby: obj.instance_variables
来源：http://hz.fzhhl.top/gtrtmdafxd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hammf.cn/gtsjllhapa.html

================================================================================
来源：http://hz.yueranfly.top/gtoyiainxg.html

H. 异常与错误处理
来源：http://hz.gzhubu.top/gtwwhlckak.html

================================================================================
来源：http://hz.cqqwz.cn/gtluzrmtnf.html

[H01] try / catch 基础
来源：http://hz.chenzaomai.com/gtatwnqemm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gttnlhomwf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.kuanghao11.cn/gtwkqvduea.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtcjlakluz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtcwpylegy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.meibo888.top/gtdcwunwbv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gthmgjlnru.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.meibo888.top/gttarbwvmz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gogol.net.cn/gttkfamzjd.html

[H02] finally / ensure 收尾
来源：http://hz.316326.xyz/gtbyfsjdue.html


<!-- 参考信息 -->