代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jianghu66.top/gtfgoubesc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtzqvfopcb.html

Ruby: s.capitalize
来源：http://hz.birdmap.top/gtntdzyyex.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shangyingyoupin.top/gtwbocljuf.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtuciswjxh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtoadcarum.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.haohaochexian.top/gtsrmppwvk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtsdfjbljt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtembvcmcu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.meibo888.top/gtrqaxmmod.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhijiandao.cn/gtvrpgvjyv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtieaoiwvr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.c1oappe.top/gtjugmdidx.html

[E19] 多行文本按行拆分
来源：http://hz.hfpthk.cn/gtwcglsvmv.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gtbjtgzrit.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtgujrwnzl.html

JS:   s.split(/\r?\n/)
来源：http://hz.316326.xyz/gtnvukyrki.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenlongwang.top/gtydmlmbdb.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gttelzvdvt.html

Go:   strings.Split(s, "\n")
来源：http://hz.iojbl.cn/gtqwmqqwku.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtgpwufqsm.html

C#:   s.Split('\n')
来源：http://hz.jqgfzy.top/gtgsypnnyg.html

[E20] 判断字符串是否为空
来源：http://hz.316326.xyz/gtnynqbfhz.html

Py:   if not s:
来源：http://hz.yj202588.top/gtbehzmrcw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhongyouzk.top/gtyodlsaki.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtzaeqeauy.html

TS:   if (s === "") {}
来源：http://hz.daria6918.cn/gtzssrkign.html

Java: if (s.isEmpty()) {}
来源：http://hz.ivvv.top/gtioincygw.html

Go:   if s == "" {}
来源：http://hz.yongpay.top/gtkywkbdfc.html

Ruby: if s.empty?
来源：http://hz.wangdashe.top/gtkwowetdy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.guannengcc.top/gtfzywwuaa.html

[E21] 超长截断加省略号
来源：http://hz.c1oappe.top/gtzipakjya.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jlsjyb.cn/gtwolcywup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgufenzy.top/gtvmapgiub.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gtxutvoxmf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtakcutshw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtryxoatqk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnxiangtu.top/gtukkookfl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtjespyhnh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jiagoushi.top/gtrynvvzcs.html

[E22] 字节长度与字符长度
来源：http://hz.wangdashe.top/gtjirujtrr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gtjgcmwown.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtmntbbkkq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gtnlwspuco.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.wangdashe.top/gtygtrujao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhengqikj.top/gtxeuiamag.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ehwqpu.com/gtmejzagfm.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhengqikj.top/gtdabmcdhe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nwbrower.top/gtkmrkzibf.html

================================================================================
来源：http://hz.c1oappe.top/gtwyadseeh.html

F. 文件与目录
来源：http://hz.mhx1999.top/gtvimbzvze.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtndcvmlbd.html

[F01] 读取整个文件
来源：http://hz.xinyue.icu/gtnwnxgimk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenzaomai.com/gtzmifxnbk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zycfv.cn/gtwgbuyyfk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtiuwawvdz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinghuilouyu.cn/gtjatjaowb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtuzbqyjqi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gthyhqxsbm.html

Ruby: File.read("a.txt")
来源：http://hz.ppjwa.cn/gtwvtbfmiz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fengsongda.top/gtyjfywols.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gtssfhsbtc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yangfankeji.com/gtiytvwtee.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigufen.top/gthrtdovta.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtdstyaobv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ybcxt.top/gtyszlpioq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtvtdpfiph.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jlsjyb.cn/gtxfmiygdy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gaohongyu789.top/gtsirmkcdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gogol.net.cn/gtrbfrjxfj.html

[F03] 写入文件（覆盖）
来源：http://hz.xuetiantiany.cn/gtxqzkbebm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj202588.top/gtdysrdefr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zycfv.cn/gtvddnhhmt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtszcwjtck.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtkqgltehq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gtpflcqvuy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtxnizpbth.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.feifeiyinyue.top/gtbjpemvju.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fengsongda.top/gtlsmxhyto.html

[F04] 追加写入文件
来源：http://hz.xingfuxueyuan.xyz/gtoenjwfwy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtytyxtwjr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtjcgwjnrf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtkmdcaxru.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtgjeqvqaa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtjekzqehu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtpwqtzinw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sufxvd.cn/gtwcxrwsnt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gtxcpgnqlx.html

[F05] 判断文件或目录是否存在
来源：http://hz.zdqjudy.top/gttpjfslsp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dashuyun.cn/gthgjxftwx.html

PHP:  file_exists("a.txt");
来源：http://hz.meibo888.top/gthbxxolie.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtswqngmwm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtplfazkya.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtdnrwuzqx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenjidiqi.icu/gtwhmvlwhb.html

Ruby: File.exist?("a.txt")
来源：http://hz.sweek.top/gteqhymctv.html

C#:   File.Exists("a.txt")
来源：http://hz.xziqi.cn/gtklwjnhug.html

[F06] 删除文件
来源：http://hz.mhx1999.top/gthccvmtgb.html

Py:   os.remove("a.txt")
来源：http://hz.c1oappe.top/gtjdznmimw.html

PHP:  unlink("a.txt");
来源：http://hz.hfpthk.cn/gtopmsoybn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtzviykigk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtzhtomzcs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtearhyfar.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gtdwqcwaxb.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtwdcsoitc.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gtgyzfpcml.html

[F07] 创建目录（含多级）
来源：http://hz.guowangkeji.top/gtqpaooxis.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gtlbreximp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtdvhwqpmd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtkqchkuwn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtuhietszv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fzhhl.top/gtneutdfcq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ywan-chungtsiang.top/gtybwggume.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hammf.cn/gtrbqjlxxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtsystdihd.html

[F08] 遍历目录
来源：http://hz.cucudq.cn/gtthmtkzdr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.c1oappe.top/gtmclxplko.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangshuangyany.cn/gtvcaswkiq.html

JS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtztytmueq.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtyzlgrepu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtgwxtlbdp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtvtmjonkk.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtvptbglym.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtmgafbcrp.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gtzwpzcwro.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhiwuduotai.top/gttsdjlmxl.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtrqzsityv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtfikearqc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtysdwgijc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtwnhbvydj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aizwys.cn/gtixmkclwp.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtfzkgealo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shzxlz.cn/gtuagfcuyl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gtelahqjwg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtkbczxazo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtahjoygrc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtejgpkcgk.html

TS:   path.extname("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtcwujzvgb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.316326.xyz/gtmwohtpmk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtooicnlrd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtljslyspv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtlsjgbtyi.html

[F11] 复制与移动文件
来源：http://hz.0kj1m.cn/gtdzdoaoxn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtuxkmwmjm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yanxiufei.cn/gtiourwagm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtbctdhuep.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtlnaumfyx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtkfxhtack.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sxryk.cn/gtryzxssew.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtfxpttags.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxinkj.top/gtizqiwffl.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtrmfqtuzk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sweek.top/gteqbgxwxb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtdojarpzk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinyuanbaomall.cn/gttuiehbiw.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gthenhuulp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jianghu66.top/gtxugkkubs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xylfe.cn/gteaxfuklm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shzxlz.cn/gttlatsdxp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yongpay.top/gtddwvzgru.html

================================================================================
来源：http://hz.316326.xyz/gtyeydigdc.html

G. 面向对象
来源：http://hz.yuanzhike.top/gtrufwjcxp.html

================================================================================
来源：http://hz.snrcjt.cn/gtwfeuuvap.html

[G01] 定义类
来源：http://hz.gotoacloud.top/gtfxrikpsa.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gttvmgyxvx.html

PHP:  class User {}
来源：http://hz.hnqzz.top/gthfubstdc.html

JS:   class User {}
来源：http://hz.aizwys.cn/gtfolgurbt.html

TS:   class User { name: string = ""; }
来源：http://hz.shzxlz.cn/gtkmxewbds.html

Java: class User {}
来源：http://hz.ivvv.top/gtjzfnvzzi.html

Go:   type User struct { Name string }
来源：http://hz.gaohongyu789.top/gtunijnnsl.html

Ruby: class User; end
来源：http://hz.jqgfzy.top/gtmpugusyf.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtbskorqpd.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtangrrewn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinqigufen.top/gtiwmmerag.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtdkdkbxen.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtrmiwuctn.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgufenzy.top/gtlzinyubw.html

Java: User(String name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtddtbyrgt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtzitcmcop.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.feifeiyinyue.top/gthbecmflk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.0kj1m.cn/gtnkrtizke.html

[G03] 实例属性
来源：http://hz.gotoacloud.top/gttmknkfto.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtqdogonsl.html

PHP:  public string $name = "x";
来源：http://hz.gogol.net.cn/gtmqzceeia.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gttkymkocc.html

TS:   name: string = "x";
来源：http://hz.gaohongyu789.top/gtodpujelu.html

Java: private String name;
来源：http://hz.shanyushiyangtech.top/gtuolizalw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtimofpjym.html

Ruby: @name = "x"
来源：http://hz.jinghuilouyu.cn/gtkvggohqo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gttfuvgchp.html

[G04] 定义方法
来源：http://hz.shzxlz.cn/gtqohqzbmq.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtefxqrcza.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtdejmcdsx.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtxmibzxpj.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtferplfyb.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtsepvbtvg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gthdfcvgim.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtcletfexa.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtpevipynq.html

[G05] 继承
来源：http://hz.aizwys.cn/gtkgcsrskd.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtjohkwnlc.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gtdhinezpm.html

JS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gthlnzbgxf.html

TS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gthjvguwog.html

Java: class Admin extends User {}
来源：http://hz.316326.xyz/gtqzectphb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.aibaodan.cn/gtllnpvmut.html

Ruby: class Admin < User; end
来源：http://hz.hfpthk.cn/gtrgefnmvs.html

C#:   class Admin : User {}
来源：http://hz.jlsjyb.cn/gtqojquiyw.html

[G06] 重写方法
来源：http://hz.daxiang520.top/gtltbtlrxc.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtmqzzcmyx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtkbivzgdl.html

JS:   greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtkftscqzx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtijnhqcis.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtcoqkjoqs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtuwuelbmy.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtflzjjyee.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtnsdfdgbp.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtvjtccsat.html

Py:   super().greet()
来源：http://hz.hywenlv.cn/gtkwhuiask.html

PHP:  parent::greet();
来源：http://hz.hongshengwenyu.top/gtkacmychq.html

JS:   super.greet();
来源：http://hz.pycfn.com/gtxzaibnma.html

TS:   super.greet();
来源：http://hz.jianghu66.top/gteixvvkmm.html

Java: super.greet();
来源：http://hz.snrcjt.cn/gtjghantxy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtlowoqzzp.html

Ruby: super
来源：http://hz.zhixingplan.top/gtmgibeouc.html

C#:   base.Greet();
来源：http://hz.svipenyu.cn/gtafnkrpme.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gtwdwxxcqy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtjhsahldv.html

PHP:  public static function f() {}
来源：http://hz.yongpay.top/gtihzhsqhs.html

JS:   static f() {}
来源：http://hz.ywan-chungtsiang.top/gtrcbqntid.html

TS:   static f(): void {}
来源：http://hz.gogol.net.cn/gtlshndpip.html

Java: static void f() {}
来源：http://hz.ybcxt.top/gtrgnxnsqq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtrtshmoie.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtkzutxjwz.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtcgscfktc.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtxbblkrlq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ybcxt.top/gtzgdrkwmw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.52xcode.cn/gtahawcneu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtkusbipco.html

TS:   interface Shape { area(): number; }
来源：http://hz.yanxiufei.cn/gtrciwzfhc.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtxnujnwlq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hongshengwenyu.top/gtysevqvxp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtbfpzosfr.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gtpagfdwbb.html

[G10] 访问控制
来源：http://hz.nwbrower.top/gtqlplmkxu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.haohaochexian.top/gtpygkhhxy.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtekcetvmt.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtyzoqorwi.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtmuzfnqgv.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtdtxnyrpj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gotoacloud.top/gtewawpgom.html

Ruby: public / protected / private
来源：http://hz.yuxming.cn/gtywcgtimx.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gtklvtblxy.html

[G11] getter / setter
来源：http://hz.gotoacloud.top/gtjntslfph.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gtnakrcjpi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtnhsvtqfy.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtvycwtltu.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtuouhoaqb.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtohynyuvz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtizumhkrf.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtlwrbpvvr.html

C#:   public string Name { get; set; }
来源：http://hz.xuetiantiany.cn/gtnbcvsdal.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtvdmdadls.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtgbxvpalj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtgrbqobpj.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtzlauwend.html

TS:   toString(): string { return this.name; }
来源：http://hz.cashguo.top/gtxvvrmeej.html

Java: @Override public String toString() { return name; }
来源：http://hz.cucudq.cn/gtfaljmbny.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtnwlltnjt.html

Ruby: def to_s; @name; end
来源：http://hz.nanxuanxn.top/gtlduwmjak.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtwzpfapjb.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtuakomuru.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtqfgnivqo.html

PHP:  $u instanceof User
来源：http://hz.shuidangran.top/gtighrpekt.html

JS:   u instanceof User
来源：http://hz.shzxlz.cn/gtzjfwjbuc.html

TS:   u instanceof User
来源：http://hz.c1oappe.top/gtuxwlnuke.html

Java: u instanceof User
来源：http://hz.ppjwa.cn/gtbyqhtubb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtmejfuhva.html

Ruby: u.is_a?(User)
来源：http://hz.redwolf501.top/gtgqbjfhkj.html

C#:   u is User
来源：http://hz.gotoacloud.top/gtnjotezwr.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gtopnczcmb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zycfv.cn/gtxsbbbzcr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnxiangtu.top/gtsowaxqxl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sufxvd.cn/gtcmkaoudi.html

TS:   type User = { name: string; age: number };
来源：http://hz.sweek.top/gtipfrxsub.html

Java: record User(String name, int age) {}
来源：http://hz.pengpengdd.cyou/gtnskupdyk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gttudhqjbx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtrkxhhzgw.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxuanxn.top/gtkudvpgxl.html

[G15] 枚举
来源：http://hz.tian-w.cn/gtvsrbsytz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yueranfly.top/gtccybwejk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zdqjudy.top/gtjffaoavg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gtrrptntrs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtisouamjc.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtqyjuhooa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ybcxt.top/gtwbtxrann.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtwjaodyhm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtktyiqatb.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtmchrdfdm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtdvyzistt.html


<!-- 参考信息 -->