代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtxrjzavyb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtmxxvvrox.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gttxbxyrzy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtxfbgevoo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dianchejie.cn/gtpzmhicux.html

[E19] 多行文本按行拆分
来源：http://hz.shuidangran.top/gttwnswimh.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtmgtjchvi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.haohaochexian.top/gtykezcjgt.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtkbzaevzc.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gthplikxvr.html

Java: s.lines().toList()
来源：http://hz.hysaishi.cn/gtomgnyven.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxuanxn.top/gtgdsmuwjz.html

Ruby: s.lines
来源：http://hz.tian-w.cn/gtktberfdi.html

C#:   s.Split('\n')
来源：http://hz.snrcjt.cn/gtglkeoyfk.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtmjjwaxgm.html

Py:   if not s:
来源：http://hz.vqdsnc.cn/gtxaupmnhw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sysykeji.top/gtwihvbapc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtovtfflkw.html

TS:   if (s === "") {}
来源：http://hz.yanxiufei.cn/gtjunloewj.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtiqakepza.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtpbgnsloe.html

Ruby: if s.empty?
来源：http://hz.yanxiufei.cn/gtuknawdqc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtcnliqnwn.html

[E21] 超长截断加省略号
来源：http://hz.jqgufenzy.top/gtmathzhor.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.0kj1m.cn/gtdftstbwt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangshuangyany.cn/gtihvbqafj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtrpgdzblj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtxsuyhagg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtouinrwwh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aibaodan.cn/gtkwomydiw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hysaishi.cn/gtjutxumxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtmhqvbdyp.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtucloxvad.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jiagoushi.top/gtrwfoqbsz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.andypj.xyz/gtbunhetut.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtnkfbtuyt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtyiyvzjxu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtnzdwwhro.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sweek.top/gtairkmnmg.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gtavjacrjf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.dianchejie.cn/gtcanqnbrf.html

================================================================================
来源：http://hz.havefunace.top/gtnnmpqxfy.html

F. 文件与目录
来源：http://hz.bjfxy.top/gtkjttiaqt.html

================================================================================
来源：http://hz.yanxiufei.cn/gtbplqchkq.html

[F01] 读取整个文件
来源：http://hz.yuxming.cn/gtzpypfqdo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtuycgbzzv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenjidiqi.icu/gthyfkczwf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhixingplan.top/gteahrmnxp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shangyingyoupin.top/gtpuccmtid.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtwwxfrvxr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtfzsytpcl.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtvfowwaeg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj202588.top/gtzviurdhz.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtageuexag.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gtrhagizyo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.9152youxi.cn/gtfpnirfuc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtgftmrnjl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dianchejie.cn/gtpbsjkqzg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtooojqdzi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtryyloqeh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtxdzlullb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.vqdsnc.cn/gtjzehokej.html

[F03] 写入文件（覆盖）
来源：http://hz.zhiwuduotai.top/gtupwwplas.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hysaishi.cn/gtrwuuweue.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtdghjlrkl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtktlpcehh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gttlvmkzpb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gtgxhtezxl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtjbxqiwqw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jianghu66.top/gtlbjsyhyl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtwjenzzat.html

[F04] 追加写入文件
来源：http://hz.ivvv.top/gtjhbglfhl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cucudq.cn/gtdhtvklee.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shzxlz.cn/gtqopzwjds.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtpjgemdlm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtjgbgvjhy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yvedp.cn/gtcsyicgup.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtufyqydoc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtrkkyvpyb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtvprcxtwt.html

[F05] 判断文件或目录是否存在
来源：http://hz.yanxiufei.cn/gtvrbajvjh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xziqi.cn/gtmypbvuem.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtzaytluac.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtmkywqedm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gticigfnkn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtwdjxmgbo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtdnegtfsl.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtoqjhrzvv.html

C#:   File.Exists("a.txt")
来源：http://hz.hfpthk.cn/gtattdiuhx.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtvlbmtrti.html

Py:   os.remove("a.txt")
来源：http://hz.zhoulong.xyz/gtriudeuzi.html

PHP:  unlink("a.txt");
来源：http://hz.iojbl.cn/gtyfscfhqa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtjprujkco.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtvuqlbmty.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtusgswpfz.html

Go:   os.Remove("a.txt")
来源：http://hz.pengpengdd.cyou/gtkbdredtk.html

Ruby: File.delete("a.txt")
来源：http://hz.sweek.top/gtbbtoymyi.html

C#:   File.Delete("a.txt");
来源：http://hz.yueranfly.top/gtmusaimaa.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtavcwrbpx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daxiang520.top/gtqriwqgng.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtyuztzkgo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtovkkvrhs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtuudeudut.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zdqjudy.top/gtiqzmqrvv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xuetiantiany.cn/gtuobyvwxm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tian-w.cn/gtrkkcqeeh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinyuanbaomall.cn/gtuuvrjbbn.html

[F08] 遍历目录
来源：http://hz.jqgfzy.top/gtnbaqdfok.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhijiandao.cn/gtxgtldzng.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gtoqrafygk.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtpxrtkynb.html

TS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gthqajmjau.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtjkaaavbw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hysaishi.cn/gthkqtrmee.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gthbaaqbng.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhongyouzk.top/gtvnpkieeu.html

[F09] 获取文件大小
来源：http://hz.jinqigufen.top/gtromewldu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtkyiebtsl.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtbvawytnp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtqhwqzbyq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtxeffcgzd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtcnkwcxvm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zdqjudy.top/gtymgjdqtl.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtynjoktap.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtuqwliosy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigufen.top/gtymhllmfd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtxyhafeld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinyuanbaomall.cn/gtqpedauit.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtiklrserh.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtmtpdaukl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gteoeoxfiy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zycfv.cn/gtgeswpgmg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtfdungidh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtqjijujjr.html

[F11] 复制与移动文件
来源：http://hz.smart0.xyz/gtrtjkjsel.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtpkiqfnnm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhiwuduotai.top/gtpevmdapi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtalasvvvk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtgscxugmr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtdiobfbiw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daxiang520.top/gtpinpbqpj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtcpeunpcx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhijiandao.cn/gtzwmiajpj.html

[F12] CSV 读写
来源：http://hz.cqqwz.cn/gtlodvfqig.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtgdmzzebq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtbsdaoxle.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gttqddwadk.html

TS:   // 同上
来源：http://hz.wangdashe.top/gtydpuvpdc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.wangdashe.top/gtorrzjrpc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gotoacloud.top/gtdczbmans.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gzhubu.top/gtnxmrzcbr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtqcshllmr.html

================================================================================
来源：http://hz.yuanzhike.top/gttjakemda.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtuwvuweum.html

================================================================================
来源：http://hz.0kj1m.cn/gtziabwapv.html

[G01] 定义类
来源：http://hz.zhaomingkeji.xyz/gtjshppoym.html

Py:   class User: pass
来源：http://hz.tanke756.top/gteuuourka.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtkvwqpitt.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtlfprzkea.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtetqgrzcj.html

Java: class User {}
来源：http://hz.shuidangran.top/gtnwpserah.html

Go:   type User struct { Name string }
来源：http://hz.zdqjudy.top/gtnjtvgsds.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtftejjlpp.html

C#:   class User {}
来源：http://hz.9152youxi.cn/gtcbmruvrf.html

[G02] 构造函数
来源：http://hz.shanyushiyangkeji.top/gtmpcejgtu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hammf.cn/gtkaznodag.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.vqdsnc.cn/gtnesyryte.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zycfv.cn/gtoysnhdxl.html

TS:   constructor(public name: string) {}
来源：http://hz.sysykeji.top/gtghclhknk.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gttugafrut.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtalrfgkfk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtfrgiords.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhaomingkeji.xyz/gtziovypzz.html

[G03] 实例属性
来源：http://hz.jianghu66.top/gtbfcpmhpv.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtwqtlrygj.html

PHP:  public string $name = "x";
来源：http://hz.hysaishi.cn/gtasrxrgyw.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtjuhokoqw.html

TS:   name: string = "x";
来源：http://hz.yueranfly.top/gtmywhrkzv.html

Java: private String name;
来源：http://hz.xuanzx.com/gthtawrnwa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtmagdptpe.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtsdzaloer.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hongshengwenyu.top/gtdgokzcnr.html

[G04] 定义方法
来源：http://hz.xuetiantiany.cn/gttrtcckwv.html

Py:   def greet(self): return self.name
来源：http://hz.gzhubu.top/gtrdvnsmcz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtsxeqxhjf.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtzozqtypw.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtfpckyztw.html

Java: String greet() { return name; }
来源：http://hz.c1oappe.top/gtkotyspkj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtwmeuxprz.html

Ruby: def greet; @name; end
来源：http://hz.yanxiufei.cn/gtotkidavo.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtmsrmlpmd.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gttesxnbxz.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtmebpwefb.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gtoozkqmdi.html

JS:   class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtmlbmjmcm.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtzfuroikd.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtbccosqoi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gthlgcosxa.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtoubahfit.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtrzkeoxwy.html

[G06] 重写方法
来源：http://hz.jlsjyb.cn/gttitrtbuu.html

Py:   def greet(self): return "admin"
来源：http://hz.hnqzz.top/gtaxqncqmv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtukclrkjd.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtgyotclkb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtsjiuovyd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yongpay.top/gtvpscqlld.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ppjwa.cn/gtnnefjfmh.html

Ruby: def greet; "admin"; end
来源：http://hz.nwbrower.top/gthtnjneag.html

C#:   public override string Greet() => "admin";
来源：http://hz.9152youxi.cn/gtqxtwzrte.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtwcoporqf.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtxeaoxmrh.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtovbhbwke.html

JS:   super.greet();
来源：http://hz.yueranfly.top/gtfzbpscyo.html

TS:   super.greet();
来源：http://hz.birdmap.top/gtlxwthsie.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtaptrhoya.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtgntdhyvg.html

Ruby: super
来源：http://hz.zhijiandao.cn/gtpffkmddl.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtctsmpfqn.html

[G08] 静态方法与属性
来源：http://hz.cqqwz.cn/gtxzfbuexn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtqqfxbmrh.html

PHP:  public static function f() {}
来源：http://hz.xziqi.cn/gtvlsiimlg.html

JS:   static f() {}
来源：http://hz.guannengcc.top/gtjnzynfvc.html

TS:   static f(): void {}
来源：http://hz.jinqigfzy.top/gtjmboiexw.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtyeiywogm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtxayjdhzx.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtmvovbovn.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtcwfbgvgh.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtymglhxww.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtemxifpkk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.andypj.xyz/gtyywxpyah.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuxming.cn/gtikygfurx.html

TS:   interface Shape { area(): number; }
来源：http://hz.c1oappe.top/gtmbqnlxtb.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtpqkszusp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gtlqhvqlsa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gtwbaezqij.html

C#:   interface IShape { double Area(); }
来源：http://hz.gotoacloud.top/gtdtpvlgyd.html

[G10] 访问控制
来源：http://hz.ppjwa.cn/gtpoqtuafv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtqrnzauhi.html

PHP:  public / protected / private
来源：http://hz.yangfankeji.com/gtwnndaple.html

JS:   #private 字段；其余公开
来源：http://hz.9152youxi.cn/gtqvaemora.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gthvbsnwvg.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtbjlengjw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.vqdsnc.cn/gtwxtylqgd.html

Ruby: public / protected / private
来源：http://hz.yuanzhike.top/gtwtuyjlnd.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtcxwsrkne.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtkealfvdt.html

Py:   @property 与 @x.setter
来源：http://hz.aibaodan.cn/gtpmmitvof.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sweek.top/gtesavmbfg.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtxwpxtsaq.html

TS:   get name(): string { return this._name; }
来源：http://hz.0kj1m.cn/gtopneimzn.html

Java: public String getName() { return name; }
来源：http://hz.zycfv.cn/gtxiimdufo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yvedp.cn/gtrxunpemh.html

Ruby: attr_accessor :name
来源：http://hz.316326.xyz/gtfnxqdxxt.html

C#:   public string Name { get; set; }
来源：http://hz.hammf.cn/gtijxicbzg.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtwwofkyci.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangtech.top/gttvgelxwf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtbpisjnzf.html

JS:   toString() { return this.name; }
来源：http://hz.yueranfly.top/gtybksywhy.html

TS:   toString(): string { return this.name; }
来源：http://hz.meibo888.top/gtudptemgj.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigfzy.top/gtkbwbcbsw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtfevzvcoc.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtciboxgqv.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gteactykgw.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtodsyikrc.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtehdwdqzv.html

PHP:  $u instanceof User
来源：http://hz.quarkkingdee.top/gtxoicwryt.html

JS:   u instanceof User
来源：http://hz.gotoacloud.top/gtlzvbdkto.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gthlqfxjiw.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtbfedekck.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuetiantiany.cn/gtxxizigsb.html

Ruby: u.is_a?(User)
来源：http://hz.chenzaomai.com/gtijomsdld.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtgjcqqucr.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtulmkjupw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhijiandao.cn/gtxtneurmk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258888.top/gtzafwtymy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jlsjyb.cn/gtypakylli.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinyuanbaomall.cn/gtztajhdzh.html

Java: record User(String name, int age) {}
来源：http://hz.zycfv.cn/gtgrueyoim.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtffdohhvm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtxihcmkrf.html

C#:   record User(string Name, int Age);
来源：http://hz.yangfankeji.com/gtrkkdlwbs.html

[G15] 枚举
来源：http://hz.jqgufenzy.top/gtogxwlzez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtdmmuntat.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtubctdlwc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxuanxn.top/gtxinfgvor.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtngqjvqxc.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gtzmmzwkgg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gtpqnjaiin.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtkhqofkrw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtwaaxjlax.html

[G16] 对象转数组 / 字典
来源：http://hz.xingfuxueyuan.xyz/gtcrquescr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtwroewiti.html

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gtaisipjta.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gthefdrjcv.html

TS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtxtynmpdm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgfzy.top/gtlkmufhbk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gtojaneinw.html

Ruby: obj.instance_variables
来源：http://hz.fzhhl.top/gttjhyivgx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtlovozrss.html

================================================================================
来源：http://hz.fzhhl.top/gtnflpftfs.html


<!-- 参考信息 -->