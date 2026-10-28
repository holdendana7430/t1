代发 wailian999

[E18] 模板占位符替换
来源：http://hz.zhixingplan.top/gtpsbmedih.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtncsxanae.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtqqesudlf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtstctzyfg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtxcfbpcso.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtejkmarok.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gtlwwxhoow.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtyvftaexx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gaohongyu789.top/gtrvvfacpm.html

[E19] 多行文本按行拆分
来源：http://hz.nwbrower.top/gthlicsaod.html

Py:   s.splitlines()
来源：http://hz.cheryme.top/gtlkuasyep.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gtaayztkas.html

JS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtarifatyc.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtdbjjpwbk.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gttekgnaic.html

Go:   strings.Split(s, "\n")
来源：http://hz.shzxlz.cn/gtyoldvrqz.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gttfziwiul.html

C#:   s.Split('\n')
来源：http://hz.quarkkingdee.top/gtmauxslyo.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtrshhrtlp.html

Py:   if not s:
来源：http://hz.jinqigufen.top/gthdqlzpkq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgfzy.top/gtijfyiqzp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtpevkjyyt.html

TS:   if (s === "") {}
来源：http://hz.zhijiandao.cn/gthwbshwfq.html

Java: if (s.isEmpty()) {}
来源：http://hz.hammf.cn/gttxgulvmy.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtnfeilzql.html

Ruby: if s.empty?
来源：http://hz.ydjk.org.cn/gtunujwyom.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gtrbidvxpn.html

[E21] 超长截断加省略号
来源：http://hz.cheryme.top/gtlubtwvhd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.havefunace.top/gtkavnyzyh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ppjwa.cn/gtzpwxyorv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gtnvkczoir.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtugrmefog.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtnyopwees.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gtvkqmscwc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hnxiangtu.top/gtwqyetjul.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtpbgxgpay.html

[E22] 字节长度与字符长度
来源：http://hz.guowangkeji.top/gtlviikjwf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtldomxnrl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtuodlzpha.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtpnyjfwkz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtjelteupm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhaomingkeji.xyz/gtemwcpmtm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.c1oappe.top/gthmilnzfv.html

Ruby: s.bytesize;  s.length
来源：http://hz.ivvv.top/gtcyyjwozp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxuanxn.top/gtmukzshmr.html

================================================================================
来源：http://hz.nwbrower.top/gtxvuquhmb.html

F. 文件与目录
来源：http://hz.ydjk.org.cn/gthwedsvlc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvfggamsq.html

[F01] 读取整个文件
来源：http://hz.xingfuxueyuan.xyz/gtugqbaxsg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gttzzjfuvl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sweek.top/gtmfeemyrx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gtggzvwwze.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ppjwa.cn/gtxqccfhfw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtsdhdgrlz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtcjfxmajd.html

Ruby: File.read("a.txt")
来源：http://hz.dashuyun.cn/gtcqrbonep.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.andypj.xyz/gtzwxbhaaq.html

[F02] 逐行读取文件
来源：http://hz.chenzaomai.com/gtjobdyfqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gzhubu.top/gtjufgouwx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtlxhhzbwu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtifqgsbae.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtztjkcjtt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtynrjqicl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.havefunace.top/gthakmdhsz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cucudq.cn/gtujzbpznv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhixingplan.top/gtdsxgowbl.html

[F03] 写入文件（覆盖）
来源：http://hz.zhiwuduotai.top/gtsaviohep.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cdnleiting.top/gtdlbgpymq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtszukapwr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtxptgmnvo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtorzbkrdc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinyuanbaomall.cn/gtskojrjrf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cucudq.cn/gtbymzbbpr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.andypj.xyz/gtwmfounnw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guannengcc.top/gtsmxsdobg.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtepdtgjzb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenjidiqi.icu/gtevbkwoyc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ywan-chungtsiang.top/gtujsaswyo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hywenlv.cn/gtoncvjivl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtnvfhzvym.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jianghu66.top/gtlxdnvigh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hammf.cn/gthtkzuyrs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgufenzy.top/gtkkosjdkj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuxming.cn/gtnsghhuog.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtgpexdfkz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxinkj.top/gtpitilzxi.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtcjusajgr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gttlqkkize.html

TS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtzyhawhnh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtqknowjip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtxldspwvr.html

Ruby: File.exist?("a.txt")
来源：http://hz.shzxlz.cn/gtmqlephsz.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtzjbyqkxk.html

[F06] 删除文件
来源：http://hz.shzxlz.cn/gtchirhpqt.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtlmmjdmea.html

PHP:  unlink("a.txt");
来源：http://hz.yueranfly.top/gtzkucdava.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtjwfjbsuj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtesctugdx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtxdhqrcbv.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtqqyttgya.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtiowvfanl.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtnsdrkbho.html

[F07] 创建目录（含多级）
来源：http://hz.tianlin.xyz/gtiutvkphy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xziqi.cn/gtawidtoog.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hfpthk.cn/gtqsqzpeup.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtcehdzrjs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtvulsufnt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtcvwjvjhu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gthiuvxsxs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hnqzz.top/gtscenjugq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ywan-chungtsiang.top/gtopbbypoi.html

[F08] 遍历目录
来源：http://hz.xziqi.cn/gtrcbjavnm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.fengsongda.top/gtrzkzrswz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xinyue.icu/gtdflfnxlj.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gthdgcjpxk.html

TS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtyydtknkr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtyigmagim.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gthyqnikeg.html

Ruby: Dir.children("dir")
来源：http://hz.zycfv.cn/gtvwctsbio.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shuidangran.top/gtloaakywj.html

[F09] 获取文件大小
来源：http://hz.sysykeji.top/gtltrjxpvf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258.top/gtquhmcnms.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtnzcegqaj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtzinxvens.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtzoaazoti.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtvtujyzvv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhongyouzk.top/gtqxeekcqo.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtspjmygbe.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgfzy.top/gtbjagjpjt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gttcfhaowv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtjvhioows.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtrtvwhlqt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtfmbchsgm.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtccnmscra.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pycfn.com/gtgfkwyobt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gtxcvdlijf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtgchkoaiq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xylfe.cn/gtqzidvylx.html

[F11] 复制与移动文件
来源：http://hz.yuanzhike.top/gtwwqejlrz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtcabzyusg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtzodwzecs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtrccdnejs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtggwsrbmg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangshuangyany.cn/gtiulapuab.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtjodgphrf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtamnnbaal.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gtzkkrqcwt.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtylscftbu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.smart0.xyz/gtkibbyzdu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hysaishi.cn/gtmasiadqf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nanxinkj.top/gtzrampayh.html

TS:   // 同上
来源：http://hz.xuetiantiany.cn/gtmcgorkup.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtcjdytaso.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gthuicvhqm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtbchhzeqc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gtknmtbogn.html

================================================================================
来源：http://hz.ydzc1.top/gtzjlvipci.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtckvpivaw.html

================================================================================
来源：http://hz.9152youxi.cn/gtrxgliuro.html

[G01] 定义类
来源：http://hz.ydzc1.top/gtwndfopao.html

Py:   class User: pass
来源：http://hz.ehwqpu.com/gtyxxeauce.html

PHP:  class User {}
来源：http://hz.xinyue.icu/gthfgljtvn.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtrxhlbqkm.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtyazsudip.html

Java: class User {}
来源：http://hz.cashguo.top/gtnpxxuqzn.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtknteytho.html

Ruby: class User; end
来源：http://hz.zhixingplan.top/gtorcsulzb.html

C#:   class User {}
来源：http://hz.tianlin.xyz/gthnnqdafr.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gtcxhdthth.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.svipenyu.cn/gtaoscizuf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jyoumei.cn/gtgexoomff.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtkdhtvinw.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgufenzy.top/gtfsizwhik.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtwwkuycdp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtxmqvcbjd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhoulong.xyz/gtfavvkkki.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtzbnwuopz.html

[G03] 实例属性
来源：http://hz.nanxinkj.top/gtbywnecqb.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gthasfcqxr.html

PHP:  public string $name = "x";
来源：http://hz.zhixingplan.top/gtpugezqqp.html

JS:   this.name = "x";
来源：http://hz.tianlin.xyz/gttgnjnjwr.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtebkesfqn.html

Java: private String name;
来源：http://hz.jinqigfzy.top/gttwezenln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hammf.cn/gtjpcavxko.html

Ruby: @name = "x"
来源：http://hz.yvedp.cn/gttzehidfu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xziqi.cn/gtblvoupgs.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gthdisgmcq.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtxemodsoj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gttgzguhsv.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtemngzbil.html

TS:   greet(): string { return this.name; }
来源：http://hz.jiagoushi.top/gthoixkyxm.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtzvzdbdre.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtvnpmipld.html

Ruby: def greet; @name; end
来源：http://hz.gaohongyu789.top/gtcdrbsmse.html

C#:   public string Greet() => Name;
来源：http://hz.ybcxt.top/gtgtdozkaa.html

[G05] 继承
来源：http://hz.nwbrower.top/gtqkiahivk.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtwphulxbp.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtevwnupkp.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtvcgnztmn.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtdonkrprr.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtlfnfusxt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhaomingkeji.xyz/gtcrngyzql.html

Ruby: class Admin < User; end
来源：http://hz.cqqwz.cn/gtbybmfpvj.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gtxwursrjs.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gtbwsgjpai.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtdiztakaq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtprtedtvc.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtsvwxcorj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtolwexyvo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yonumen.top/gtbhwhrrvt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhaomingkeji.xyz/gtxtlgexpu.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtabbwqdbi.html

C#:   public override string Greet() => "admin";
来源：http://hz.cashguo.top/gtwclaadeu.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gthqxhjcxh.html

Py:   super().greet()
来源：http://hz.redwolf501.top/gtunqvxbcf.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtvahxvnqu.html

JS:   super.greet();
来源：http://hz.daria6918.cn/gtlpnjikmr.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtsklotrrz.html

Java: super.greet();
来源：http://hz.316326.xyz/gtxqxjhony.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtkqrbhpli.html

Ruby: super
来源：http://hz.chenlongwang.top/gtwxpfided.html

C#:   base.Greet();
来源：http://hz.yj20258.top/gtyfsljggq.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtcszxgtza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gteyohsmys.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtjrpmqexv.html

JS:   static f() {}
来源：http://hz.ybcxt.top/gtcxrtvoiw.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtsfkbaxxs.html

Java: static void f() {}
来源：http://hz.aibaodan.cn/gtpnegnvef.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtzesckwok.html

Ruby: def self.f; end
来源：http://hz.yuxming.cn/gtzotrpllv.html

C#:   public static void F() {}
来源：http://hz.feifeiyinyue.top/gtobubmtsp.html

[G09] 接口 / 抽象类
来源：http://hz.guowangkeji.top/gtlsagawuj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenjidiqi.icu/gtnfcgrjju.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aibaodan.cn/gtkxdnwypj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jianghu66.top/gtqrfdpxyl.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtdhihemjr.html

Java: interface Shape { double area(); }
来源：http://hz.xuanzx.com/gtcmlukjxy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtdsmskfxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhongyouzk.top/gtzpyejhel.html

C#:   interface IShape { double Area(); }
来源：http://hz.jianghu66.top/gtseyghzto.html

[G10] 访问控制
来源：http://hz.wangdashe.top/gtkjiikthr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gtfxlheuyy.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtwmgsaevu.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gttwrkhexj.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtyoqehgys.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtzandzesn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuanzhike.top/gtaoxdgbhf.html

Ruby: public / protected / private
来源：http://hz.gzhubu.top/gtsgfoghke.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtbvipuqzf.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtuxmjfchj.html

Py:   @property 与 @x.setter
来源：http://hz.sufxvd.cn/gtnqbdtfzc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtaoaaofth.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gtgjnbdhjy.html

TS:   get name(): string { return this._name; }
来源：http://hz.yvedp.cn/gtynkgfpjh.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtzfndvxip.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtvaboijnx.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gtvetmolxb.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtkgbxbuci.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtimalujoq.html

Py:   def __str__(self): return self.name
来源：http://hz.gotoacloud.top/gtgaghyfhj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtdyfpjhkz.html

JS:   toString() { return this.name; }
来源：http://hz.9152youxi.cn/gtkzizehmw.html

TS:   toString(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtkupmumbc.html

Java: @Override public String toString() { return name; }
来源：http://hz.daria6918.cn/gthpbkkofl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gteqfccykl.html

Ruby: def to_s; @name; end
来源：http://hz.shzxlz.cn/gtzdmivuhu.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtpotjlxbi.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gtmpludiua.html

Py:   isinstance(u, User)
来源：http://hz.dashuyun.cn/gttdhgedic.html

PHP:  $u instanceof User
来源：http://hz.ydzc1.top/gtkzryqmch.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtcclapryv.html

TS:   u instanceof User
来源：http://hz.chenzaomai.com/gthwjierwf.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtkacpwyly.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hammf.cn/gtuqhaxqqn.html

Ruby: u.is_a?(User)
来源：http://hz.ivvv.top/gtgrtcjtjh.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtxrdyrfqv.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtwaawqwxj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtpvoulfhy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yueranfly.top/gthvipxnbt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sweek.top/gtgddktpbl.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtunlrhewz.html

Java: record User(String name, int age) {}
来源：http://hz.zhoulong.xyz/gtabyzisst.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydjk.org.cn/gtjuszyqeg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuxming.cn/gtjjhusuyo.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gtjgrriagq.html

[G15] 枚举
来源：http://hz.andypj.xyz/gtfwhazyoj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yvedp.cn/gtstfzlhbn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtssojefyj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xziqi.cn/gtzllsksbz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtmoztjrbw.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhijiandao.cn/gtrazlrqcn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtlkxpahnb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtuprpmszm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtlumfnejv.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtcydwgpiv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtrnubbnmd.html

PHP:  get_object_vars($obj);
来源：http://hz.sxryk.cn/gtuzmgqwwf.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtaswazbam.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtuweevesy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtliwncymo.html


<!-- 参考信息 -->