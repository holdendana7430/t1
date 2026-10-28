代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.feifeiyinyue.top/gtxufdmbnl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtawncpzqa.html

Ruby: s.capitalize
来源：http://hz.tianlin.xyz/gtckcqjlil.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yueranfly.top/gtlgejqyki.html

[E18] 模板占位符替换
来源：http://hz.mhx1999.top/gtmclenpiv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gtfastqfnv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhoulong.xyz/gtxywvvwul.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gttgyaqpyr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cashguo.top/gtrbnpewvy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.quarkkingdee.top/gtjnzyspew.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ybcxt.top/gtizrajvyr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhengqikj.top/gtsytvsrfz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xingfuxueyuan.xyz/gtoojicbcv.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtcwhcptiz.html

Py:   s.splitlines()
来源：http://hz.hnqzz.top/gtyioiqljb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnqzz.top/gtavnmrrcc.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtesdeydhi.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtixkdjvqj.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtkdkyrvjy.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydzc1.top/gtorggttxj.html

Ruby: s.lines
来源：http://hz.hnqzz.top/gtxpnfequj.html

C#:   s.Split('\n')
来源：http://hz.cqqwz.cn/gthdixxaxq.html

[E20] 判断字符串是否为空
来源：http://hz.ybcxt.top/gtshqayayf.html

Py:   if not s:
来源：http://hz.jinqigfzy.top/gtavetfcwv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.wangshuangyany.cn/gttahsnljl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnxiangtu.top/gtfdfmoxbv.html

TS:   if (s === "") {}
来源：http://hz.316326.xyz/gtrijglgtm.html

Java: if (s.isEmpty()) {}
来源：http://hz.guannengcc.top/gtrifwnrhi.html

Go:   if s == "" {}
来源：http://hz.xinyue.icu/gtnmapakjj.html

Ruby: if s.empty?
来源：http://hz.ydjk.org.cn/gtxhhtikop.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtxdshckna.html

[E21] 超长截断加省略号
来源：http://hz.mhx1999.top/gtzaylikal.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtifkddxbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtzpwuvwjl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtyehqrwxs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gtchchoarn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtrmrqbzoq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhaomingkeji.xyz/gtygbigtau.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.kuanghao11.cn/gtmomxwobl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cucudq.cn/gtrwwdpfdk.html

[E22] 字节长度与字符长度
来源：http://hz.jianghu66.top/gtcqigytvz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gthhgkuluf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258.top/gtzhsyvawm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtgmuchwpt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtyoknmpga.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sysykeji.top/gtvicpevzk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jianghu66.top/gtgeyqzumh.html

Ruby: s.bytesize;  s.length
来源：http://hz.havefunace.top/gtgmdcpzwk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.birdmap.top/gtxmmahmxj.html

================================================================================
来源：http://hz.ppjwa.cn/gtbpnvqcmm.html

F. 文件与目录
来源：http://hz.zhaomingkeji.xyz/gtbaqvenwk.html

================================================================================
来源：http://hz.xinyue.icu/gtmiicpdqz.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtdakhaghq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhiwuduotai.top/gtjrcqsisy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtycnonoid.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtxsozugfh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hongshengwenyu.top/gtybaalcxk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gttzataldn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnxiangtu.top/gtrmiqbcox.html

Ruby: File.read("a.txt")
来源：http://hz.smart0.xyz/gtjgyacogf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtthesqrvk.html

[F02] 逐行读取文件
来源：http://hz.jinqigfzy.top/gtsswwsstw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgufenzy.top/gtkjvviomv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zdqjudy.top/gtlphiklil.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtsyufhwiu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtqvqfqvfi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtwaoqqyng.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xylfe.cn/gtxqsfpnut.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtfprnuksc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.birdmap.top/gtlpiwdmdd.html

[F03] 写入文件（覆盖）
来源：http://hz.mhx1999.top/gtufclxuxo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuxming.cn/gtmfakdtyk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtlvotffux.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gttlxxyiui.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtudmtbygx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhoulong.xyz/gtqyjuppdu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhengqikj.top/gtqjkagvqh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yongpay.top/gtemfbnqsk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gtbeeyypso.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtajjumjis.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gzhubu.top/gtgcihhgzp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jiagoushi.top/gtetwyozqi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtpkscjwnu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtkdtjgnmx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtwtiptjcu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtbnylztjb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shangyingyoupin.top/gtkzkrwesu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.quarkkingdee.top/gtrykajvgu.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtrjqlhmcx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gtcfixxkwt.html

PHP:  file_exists("a.txt");
来源：http://hz.jianghu66.top/gtmaweeyzp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtquirqjjy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtldhjqmrp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtunejxkdz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gtpsuokejv.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtylqpofpa.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtidnnhzcy.html

[F06] 删除文件
来源：http://hz.chenzaomai.com/gtscjheodm.html

Py:   os.remove("a.txt")
来源：http://hz.shzxlz.cn/gtjxsaxdqa.html

PHP:  unlink("a.txt");
来源：http://hz.yueranfly.top/gtgjjbmeyz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtxgnoajnx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtizblzvhb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gthpkigmlm.html

Go:   os.Remove("a.txt")
来源：http://hz.cdnleiting.top/gtgsqikkde.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigfzy.top/gtdeqycllx.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtoshjertn.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtmhxydcig.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yongpay.top/gtblugxwsj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinyuanbaomall.cn/gtfrqttiaq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gttyhlzqox.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtprxtanbv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtrcvbpkem.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtmehnjaep.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtuslzfwbe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jlsjyb.cn/gtwhwsqddi.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtqgpdfswo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgfzy.top/gtygbakyxm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtuhllgkbk.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtyykcnrpj.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtebzyjvxx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtgcnhjlup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtdhscropt.html

Ruby: Dir.children("dir")
来源：http://hz.wangshuangyany.cn/gtcbgtzsxe.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aizwys.cn/gtujcjvfrc.html

[F09] 获取文件大小
来源：http://hz.smart0.xyz/gtazjbjgpd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinghuilouyu.cn/gtvmgdydst.html

PHP:  filesize("a.txt");
来源：http://hz.smart0.xyz/gtaewqluzf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtztmutcqo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtjzlwhixx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtrgsvgakl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xingfuxueyuan.xyz/gthqklugjw.html

Ruby: File.size("a.txt")
来源：http://hz.gogol.net.cn/gtzyelznqn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sysykeji.top/gtwikideha.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ybcxt.top/gteaxdggxs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtqixmiyfz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gtnjsxgzrz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtbkakzzqh.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gteoufudtf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yongpay.top/gtpvjycxzn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtmulyqive.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtculptekl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtcwheawqf.html

[F11] 复制与移动文件
来源：http://hz.hammf.cn/gtfyscrzjm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtzyequzfz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuetiantiany.cn/gtqygmihap.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtumqhlaxq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtaeqlanga.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258888.top/gtitaqxrqa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hysaishi.cn/gtaqtmbluc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtcffbveww.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhixingplan.top/gtyvasgllf.html

[F12] CSV 读写
来源：http://hz.jqgfzy.top/gtyjcencwu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.iojbl.cn/gtuoncvntr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gtzsqoepbk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtahtgpxvq.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtndmqnfng.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtghthjoyk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.smart0.xyz/gtaxaullcu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtcfaydnmh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuanzhike.top/gtxfufxqnv.html

================================================================================
来源：http://hz.gotoacloud.top/gtsjdykipr.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtwlwqrrwr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtrvmqcebp.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtdhrvmehn.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtnnauyjte.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtsaqsxdom.html

JS:   class User {}
来源：http://hz.chenjidiqi.icu/gtjlbrwwns.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtzxxbcqoy.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gtjnadzpag.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gtuyflchwk.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtdmwfjslr.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtfpmjvuze.html

[G02] 构造函数
来源：http://hz.jlsjyb.cn/gtfwexzfsf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtyqazpvzv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtpcayjkto.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtbkfxlbtn.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gtfxoszsbz.html

Java: User(String name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtndtpddud.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hongshengwenyu.top/gtcbzqaubi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtqjryroli.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgfzy.top/gtatgslknw.html

[G03] 实例属性
来源：http://hz.jqgfzy.top/gtnhhzcvay.html

Py:   self.name = "x"
来源：http://hz.nwbrower.top/gtorcnelcw.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gtnkkselek.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtpftdggok.html

TS:   name: string = "x";
来源：http://hz.9152youxi.cn/gthoddaguh.html

Java: private String name;
来源：http://hz.ehwqpu.com/gtiidxhjvu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.havefunace.top/gtisknepqe.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtlcysuvtp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuanzhike.top/gtnfsmuwjv.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtnwsqbxff.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtagxwewuu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtwiucwapt.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtmiaaoqdn.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtwvtmjinu.html

Java: String greet() { return name; }
来源：http://hz.ydjk.org.cn/gtnbsugnkc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtwgyyohaa.html

Ruby: def greet; @name; end
来源：http://hz.yvedp.cn/gtanncliix.html

C#:   public string Greet() => Name;
来源：http://hz.xinyue.icu/gtgmzgbemf.html

[G05] 继承
来源：http://hz.ywan-chungtsiang.top/gtdgnsuhzp.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtlyrykhfu.html

PHP:  class Admin extends User {}
来源：http://hz.ybcxt.top/gteeahjewb.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtiopmpyer.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtbpejduom.html

Java: class Admin extends User {}
来源：http://hz.andypj.xyz/gtkxlvidom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtbflsguhx.html

Ruby: class Admin < User; end
来源：http://hz.snrcjt.cn/gtislpmars.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtzsbdyyul.html

[G06] 重写方法
来源：http://hz.vqdsnc.cn/gtsjcwetsl.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gthzdrphre.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtlrpgxjjd.html

JS:   greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtadtssmuw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtiydykkym.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gttdkoaynj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtbnfhdrgk.html

Ruby: def greet; "admin"; end
来源：http://hz.tanke756.top/gtdvctmzfs.html

C#:   public override string Greet() => "admin";
来源：http://hz.quarkkingdee.top/gtrnyjsxrf.html

[G07] 调用父类方法
来源：http://hz.316326.xyz/gtjqfxmgyk.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gtnvbwcoql.html

PHP:  parent::greet();
来源：http://hz.mhx1999.top/gtytqyzcap.html

JS:   super.greet();
来源：http://hz.yj202588.top/gtsjyekowu.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtbnspbuac.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtopcxodvf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtdhceshaw.html

Ruby: super
来源：http://hz.tianlin.xyz/gtremzgoey.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gtueichrhd.html

[G08] 静态方法与属性
来源：http://hz.shzxlz.cn/gtakeixzrl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gtrjegdtvz.html

PHP:  public static function f() {}
来源：http://hz.ybcxt.top/gtxhvgsnkt.html

JS:   static f() {}
来源：http://hz.cheryme.top/gtwuriwmgf.html

TS:   static f(): void {}
来源：http://hz.jlsjyb.cn/gtfnbanvzc.html

Java: static void f() {}
来源：http://hz.cheryme.top/gtbufnmnzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ehwqpu.com/gtbgvukxim.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtnhazydgp.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtdxelpuon.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtfwvqtepu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangshuangyany.cn/gtuymomler.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tianlin.xyz/gtqwuoxcpv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhixingplan.top/gtooevshlc.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangshuangyany.cn/gtuetncfeb.html

Java: interface Shape { double area(); }
来源：http://hz.quarkkingdee.top/gtfetieptj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtutlvbewu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.quarkkingdee.top/gtupgbnpko.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtpdjlucmh.html

[G10] 访问控制
来源：http://hz.ppjwa.cn/gtactusfiv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gtbszzrsgq.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtgzictogp.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtrfysonou.html

TS:   public / protected / private
来源：http://hz.cucudq.cn/gtvpxxeapr.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtystmyfck.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtcvyxcwom.html

Ruby: public / protected / private
来源：http://hz.snrcjt.cn/gtdxcakbsx.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gttrzzyidy.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtwszqwysm.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtvdjnspfu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gteyhmvvdf.html

JS:   get name() { return this._name; }
来源：http://hz.ybcxt.top/gtcrarwlam.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gtbmzqxone.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtbiqnsrve.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guowangkeji.top/gthmbrybvm.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gtwexxkxen.html

C#:   public string Name { get; set; }
来源：http://hz.bjfxy.top/gttjdovkni.html

[G12] 对象转字符串
来源：http://hz.shzxlz.cn/gtejxvwvhf.html

Py:   def __str__(self): return self.name
来源：http://hz.ivvv.top/gtpjqjdylg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtrzfpojeg.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtcylqlisa.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtjubhmmem.html

Java: @Override public String toString() { return name; }
来源：http://hz.smart0.xyz/gtgsphzksh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtsreonzkz.html

Ruby: def to_s; @name; end
来源：http://hz.havefunace.top/gtzzufetpz.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gtftcjsinn.html

[G13] 判断对象类型
来源：http://hz.shzxlz.cn/gtdtdvekjf.html

Py:   isinstance(u, User)
来源：http://hz.gaohongyu789.top/gtprfuhubi.html

PHP:  $u instanceof User
来源：http://hz.nanxinkj.top/gthofkgcux.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtodovaopr.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtdiavamzj.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gtmrqprais.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenjidiqi.icu/gtrvrrxwmk.html

Ruby: u.is_a?(User)
来源：http://hz.bjfxy.top/gtqkuflshg.html

C#:   u is User
来源：http://hz.vqdsnc.cn/gtyrtpwuws.html

[G14] 数据类 / record
来源：http://hz.xingfuxueyuan.xyz/gtbjensing.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtsxtwqwie.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jyoumei.cn/gtekifxhzo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtvomtaucr.html

TS:   type User = { name: string; age: number };
来源：http://hz.xylfe.cn/gtduugalsj.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtdvjzbbge.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gttlbhuqce.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtnaisrtur.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gthzyfxboe.html

[G15] 枚举
来源：http://hz.yj20258.top/gtdgjolpbj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guannengcc.top/gtzvofagzk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gtkdonmpgp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtfacxieif.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtlzokhyjk.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gtapkczbla.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gotoacloud.top/gteonngrrl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gtxsudqvet.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xinyue.icu/gtfdcexzrf.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtyllcwcrd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtzemwzglw.html


<!-- 参考信息 -->