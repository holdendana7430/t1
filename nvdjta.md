代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtrmbknxgy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dashuyun.cn/gtdzzjaoxq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gtbccvowac.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gthuddbnib.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.birdmap.top/gtvzzbcwpo.html

[E19] 多行文本按行拆分
来源：http://hz.redwolf501.top/gtavtlgqag.html

Py:   s.splitlines()
来源：http://hz.zhixingplan.top/gtvozqeuxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtymkcufml.html

JS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtdehptvmj.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtrknuuufy.html

Java: s.lines().toList()
来源：http://hz.ehwqpu.com/gthqeryply.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtqjtxtiqg.html

Ruby: s.lines
来源：http://hz.chenzaomai.com/gtyylkewcr.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gtrdzdmeac.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtwtcdjbta.html

Py:   if not s:
来源：http://hz.sysykeji.top/gttwejahsc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.guannengcc.top/gtkfppmuct.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangtech.top/gtnjvkobny.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gtbarqipxu.html

Java: if (s.isEmpty()) {}
来源：http://hz.ybcxt.top/gtvarkmzth.html

Go:   if s == "" {}
来源：http://hz.redwolf501.top/gtmagejgqt.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtuziavbko.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.snrcjt.cn/gtysxwjeph.html

[E21] 超长截断加省略号
来源：http://hz.tian-w.cn/gtmknmpkmg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangdashe.top/gtcrgubjnr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jyoumei.cn/gtnzhvttpx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtullnvzre.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtusllsvse.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtqregvbht.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtvmmoamuz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hysaishi.cn/gtlzgxlmxi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtepeyqvve.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gtqywegaad.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenzaomai.com/gtcdquqfsb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtzuuggxug.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtezttjrbl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtwlobnurn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtiydeifxh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.haohaochexian.top/gtqfkdokhd.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtwmeptymc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtwmmofbro.html

================================================================================
来源：http://hz.jyoumei.cn/gttxlhzbmt.html

F. 文件与目录
来源：http://hz.daxiang520.top/gttbixdjgh.html

================================================================================
来源：http://hz.chenzaomai.com/gtqarwcnwq.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtzmxebjyd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtjzxlgewt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnqzz.top/gtlxsiistg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tianlin.xyz/gtahrvbidl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hfpthk.cn/gtnhhympwz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtmieopfzo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sxryk.cn/gtxonmvhhh.html

Ruby: File.read("a.txt")
来源：http://hz.xuetiantiany.cn/gtxbwmtynq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hysaishi.cn/gtbuhfdxbk.html

[F02] 逐行读取文件
来源：http://hz.zhaomingkeji.xyz/gtifmqixjx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gtibrdwjcn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pycfn.com/gtwvgbhwzt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gttxxbarfe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtrujdkobw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtezpukhgp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cashguo.top/gtqcivolcj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cucudq.cn/gtoitpzqzu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pengpengdd.cyou/gtmtojxjmg.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtudrvrlvv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtvdjdccem.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daxiang520.top/gtkalpqfpw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gtayiyzeyd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtnlrrbguh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtltffupgq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tian-w.cn/gtooajzatf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gteioldjnc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtxifnfmjv.html

[F04] 追加写入文件
来源：http://hz.fengsongda.top/gtmdcoprgb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tian-w.cn/gtboyducoq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gttqpyndqx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtoxnqwxpk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gttkpmovqj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aizwys.cn/gtpaegrwic.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fengsongda.top/gtnnkiwgpu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gtxfyoqjnl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sysykeji.top/gtwpulypnj.html

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gtwekyvbic.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtchiwqvxs.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtiwxipurw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtqzacleie.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtsrxfurnr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtflfnmvsa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gogol.net.cn/gtozeyhbus.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtpsqkaluw.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtkmmdssej.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gtzfxejahy.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gtgknvscpe.html

PHP:  unlink("a.txt");
来源：http://hz.aizwys.cn/gtzndfiecj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtfebnanip.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtmjrfxcfe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtfzfqdgve.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtwrkjplvh.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtdcpzawbv.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtfisntvha.html

[F07] 创建目录（含多级）
来源：http://hz.zhoulong.xyz/gthnvopllt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtdfunuhvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtmjmcsxco.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtfwhrvqpq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtjcctlias.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtlbamywit.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtasqgpqfe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xinyue.icu/gtjddtrsnd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtibkqvkgj.html

[F08] 遍历目录
来源：http://hz.cheryme.top/gtkytximpa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtdnqacxsm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtsciggdjb.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtryqtqzjd.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtcuwaqeas.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtmhcsivtq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtxzjoudhp.html

Ruby: Dir.children("dir")
来源：http://hz.ivvv.top/gtajeqhtav.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yanxiufei.cn/gtykicsikr.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gttrgfoepg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.quarkkingdee.top/gtfjrepjtl.html

PHP:  filesize("a.txt");
来源：http://hz.vqdsnc.cn/gtrrfcwkfg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gthtwqpgtv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtornmqlnr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtpvpnixvl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.316326.xyz/gtlpwwwmvq.html

Ruby: File.size("a.txt")
来源：http://hz.jqgfzy.top/gtmnojciyh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtffpgyijm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhiwuduotai.top/gtxynitswu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtaawyrphq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinghuilouyu.cn/gtxuorkyjg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtmexpkdoh.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtsfczxmic.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gtygdkrxri.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xinyue.icu/gtwvaqevvm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtmzlasgkm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtmsgyhekt.html

[F11] 复制与移动文件
来源：http://hz.dianchejie.cn/gtpheoftyc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtuppdbyaj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gtaoqwwvjk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtwjvgpqvm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtkshvwyyh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jianghu66.top/gtpkkfeuhi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhengqikj.top/gtidotwfrb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gthqtrebeo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cheryme.top/gtmacgpcqi.html

[F12] CSV 读写
来源：http://hz.sweek.top/gthhgfxulj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtwxlsdzzr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj202588.top/gtsdxloweb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenzaomai.com/gtwixqnbff.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gtgosaiugo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cucudq.cn/gtrwwsbbem.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gtubtseulf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cqqwz.cn/gtsrkhkiml.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258.top/gtrqaawsek.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpoiiaevr.html

G. 面向对象
来源：http://hz.cqqwz.cn/gtvctvovmw.html

================================================================================
来源：http://hz.aibaodan.cn/gtgnbcgdfe.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtuzardygp.html

Py:   class User: pass
来源：http://hz.vqdsnc.cn/gtnxinfjzs.html

PHP:  class User {}
来源：http://hz.yj202588.top/gthhakqepo.html

JS:   class User {}
来源：http://hz.316326.xyz/gtcywhuydu.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtvyrwgwhp.html

Java: class User {}
来源：http://hz.yongpay.top/gtjpllhmxa.html

Go:   type User struct { Name string }
来源：http://hz.yangfankeji.com/gtomhrofse.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtqgggovdz.html

C#:   class User {}
来源：http://hz.feifeiyinyue.top/gtnadhpqrm.html

[G02] 构造函数
来源：http://hz.xingfuxueyuan.xyz/gtiqmgikfb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.redwolf501.top/gtyxydstbl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sysykeji.top/gteucooxpv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.andypj.xyz/gtfmydddae.html

TS:   constructor(public name: string) {}
来源：http://hz.meibo888.top/gthtxjiveq.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtcqmsxjor.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtkbcwjiey.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuanzx.com/gthfoyogql.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fzhhl.top/gtddlkufnw.html

[G03] 实例属性
来源：http://hz.316326.xyz/gtoqmgbwzn.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtugsaafqq.html

PHP:  public string $name = "x";
来源：http://hz.sweek.top/gtjgqbuxbg.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtrjmjscfg.html

TS:   name: string = "x";
来源：http://hz.cucudq.cn/gtupfxzbpz.html

Java: private String name;
来源：http://hz.gzhubu.top/gtbzqwkzve.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenlongwang.top/gtpncgdjqy.html

Ruby: @name = "x"
来源：http://hz.yongpay.top/gtcoaoxfpo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gtdzlfpzxx.html

[G04] 定义方法
来源：http://hz.smart0.xyz/gtmvbfpnee.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gtuxcglcdg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtfuhkkxps.html

JS:   greet() { return this.name; }
来源：http://hz.yueranfly.top/gtpbekmpzx.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtrnnapigw.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtjlmqssaw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtlhizpzjf.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtbipnfcfe.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtedysovoz.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gteakuonqn.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gtifektxkw.html

PHP:  class Admin extends User {}
来源：http://hz.ybcxt.top/gtruqjhhkj.html

JS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtasznuqrj.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtongcjyfa.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gttesksbot.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtvjqcuhrt.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtqqgbwkbz.html

C#:   class Admin : User {}
来源：http://hz.52xcode.cn/gtckyiloku.html

[G06] 重写方法
来源：http://hz.sysykeji.top/gtqxjeqcei.html

Py:   def greet(self): return "admin"
来源：http://hz.zhoulong.xyz/gtkfadeimn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtuosgdiyp.html

JS:   greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtilhbqwkb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtngjstjzh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtokpfxojp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtlyfwdpqe.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtonoqottg.html

C#:   public override string Greet() => "admin";
来源：http://hz.feifeiyinyue.top/gtumtmsikm.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gtdhmbquph.html

Py:   super().greet()
来源：http://hz.yongpay.top/gtacofmbgx.html

PHP:  parent::greet();
来源：http://hz.jianghu66.top/gtepciqvzq.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtmkllesen.html

TS:   super.greet();
来源：http://hz.guowangkeji.top/gtrvukahxh.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtxydjyadg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtzjmgiwnm.html

Ruby: super
来源：http://hz.cashguo.top/gtqcgobtzi.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtqrtdszve.html

[G08] 静态方法与属性
来源：http://hz.cqqwz.cn/gtfhragsab.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hongshengwenyu.top/gtalzuyubw.html

PHP:  public static function f() {}
来源：http://hz.nanxinkj.top/gtehppgibc.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtnqezefri.html

TS:   static f(): void {}
来源：http://hz.xziqi.cn/gtfyfmprth.html

Java: static void f() {}
来源：http://hz.gaohongyu789.top/gtfavnooau.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cucudq.cn/gtekifrsah.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gttyzvnztf.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtqiamkcmr.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gthchiggwc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gteurvgrnx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gtfdtbkfbi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhengqikj.top/gtoybrtfqm.html

TS:   interface Shape { area(): number; }
来源：http://hz.feifeiyinyue.top/gtaolotsee.html

Java: interface Shape { double area(); }
来源：http://hz.sxryk.cn/gtlsnbmifc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtveinbdiw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pengpengdd.cyou/gttlnjgklp.html

C#:   interface IShape { double Area(); }
来源：http://hz.gogol.net.cn/gtbbrmybmq.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gttmkbiobg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtegokldqa.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gttvyqoafd.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtefjvdsxi.html

TS:   public / protected / private
来源：http://hz.fzhhl.top/gthckwudcy.html

Java: public / protected / private / 默认包级
来源：http://hz.gogol.net.cn/gtnnsccknd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtsoghbgld.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtkttuwrln.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtxmbqcrka.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtzoobleti.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtiuusdycw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtinghdtac.html

JS:   get name() { return this._name; }
来源：http://hz.hysaishi.cn/gttmhijyuj.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtrsbwdzbr.html

Java: public String getName() { return name; }
来源：http://hz.snrcjt.cn/gtubxaemno.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gtcnkrpakc.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtluyquoav.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtnyjqrmpq.html

[G12] 对象转字符串
来源：http://hz.jianghu66.top/gtntvdwkfx.html

Py:   def __str__(self): return self.name
来源：http://hz.xinyue.icu/gtdvqthrah.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtbcyzwoxi.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtxtzktevl.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtdcpdzonn.html

Java: @Override public String toString() { return name; }
来源：http://hz.jianghu66.top/gtiesylrsc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ivvv.top/gtopcgsfyg.html

Ruby: def to_s; @name; end
来源：http://hz.daria6918.cn/gtozjbavpf.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258888.top/gtozglpgqi.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtdiymozvz.html

Py:   isinstance(u, User)
来源：http://hz.jiagoushi.top/gtotbjqbht.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtxamupvzz.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtjwhgjeok.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gtvjvqghdu.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtytxoggut.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hywenlv.cn/gtpfnbzdqg.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtjjwqlrbp.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtcrunuyuu.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtunklqyzq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gtodhbutrg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gttbltedse.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ehwqpu.com/gtigqizdou.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuanzhike.top/gtraydldry.html

Java: record User(String name, int age) {}
来源：http://hz.gotoacloud.top/gtcmrwkiwc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinyuanbaomall.cn/gtxopebrym.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtuetdkxhs.html

C#:   record User(string Name, int Age);
来源：http://hz.vqdsnc.cn/gtskwdwxlo.html

[G15] 枚举
来源：http://hz.yueranfly.top/gtwzbedgty.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ppjwa.cn/gtzuaodfur.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gthasrtrca.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gtwflhprzb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtdqiircew.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtykidcxzr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jlsjyb.cn/gtpgmiblqr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.birdmap.top/gtxcyzqptu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtbxmviysf.html

[G16] 对象转数组 / 字典
来源：http://hz.hfpthk.cn/gtvvxknmkb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.kuanghao11.cn/gtiacptypz.html

PHP:  get_object_vars($obj);
来源：http://hz.gaohongyu789.top/gtjmpubkjd.html

JS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtoaxklhmh.html

TS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtpipefjwj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtwcpsyuto.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtaqnlkpra.html

Ruby: obj.instance_variables
来源：http://hz.andypj.xyz/gtnhtdjicd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtcysccyfv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtjqqhylnx.html


<!-- 参考信息 -->