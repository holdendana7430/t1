代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.jiagoushi.top/gtgqwkudvj.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenzaomai.com/gtfczfpskr.html

Java: s.lines().toList()
来源：http://hz.jinyuanbaomall.cn/gtjookhbqd.html

Go:   strings.Split(s, "\n")
来源：http://hz.fzhhl.top/gtzhxtnnwk.html

Ruby: s.lines
来源：http://hz.sweek.top/gttukdarbe.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gtdqlntjkv.html

[E20] 判断字符串是否为空
来源：http://hz.sufxvd.cn/gtoiqnadga.html

Py:   if not s:
来源：http://hz.cheryme.top/gtxrljxgsc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258888.top/gtrjvqszgw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.feifeiyinyue.top/gtgdqnaazz.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtyattfzky.html

Java: if (s.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtxclmtivi.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtnsnylaba.html

Ruby: if s.empty?
来源：http://hz.zhijiandao.cn/gtoxglmrbo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.andypj.xyz/gtxnthpuhm.html

[E21] 超长截断加省略号
来源：http://hz.xinyue.icu/gtkqtcihyi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.c1oappe.top/gtkejqtmmp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangshuangyany.cn/gtkvsmdhyc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtshzytlcj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtdagznkrz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtqazjaexd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shuidangran.top/gtolwhnynj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aizwys.cn/gtmqcnvcrq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gtyfzkfwhb.html

[E22] 字节长度与字符长度
来源：http://hz.nwbrower.top/gtcdzquqwo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhixingplan.top/gttnltvrfb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtjhpzqvrk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tanke756.top/gtnqsecasv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gthmyebsei.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.pengpengdd.cyou/gthqrslmld.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xingfuxueyuan.xyz/gtsnpoxzog.html

Ruby: s.bytesize;  s.length
来源：http://hz.sufxvd.cn/gtkxdzoaxq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gtqqzjsmxk.html

================================================================================
来源：http://hz.zycfv.cn/gtadmiezwu.html

F. 文件与目录
来源：http://hz.316326.xyz/gtoztkrgbv.html

================================================================================
来源：http://hz.316326.xyz/gtpzofqovn.html

[F01] 读取整个文件
来源：http://hz.shzxlz.cn/gtmsawbgeg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtgxhrvoet.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258888.top/gtzwycxxzy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtfknvxupm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.0kj1m.cn/gtpjjoupnn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtotjuvmlm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jiagoushi.top/gtzbnhfzex.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtvyxyfkdt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cheryme.top/gtgcrrdthg.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gtmiifysrn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.316326.xyz/gtgrohnzrh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtcmetfuyk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinyuanbaomall.cn/gtqtjvqcht.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtwmjunirb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtdlnczqvs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pycfn.com/gtprogjsbk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnqzz.top/gtaqjnekfo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gtysdrtscr.html

[F03] 写入文件（覆盖）
来源：http://hz.yanxiufei.cn/gtiuajbysv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xingfuxueyuan.xyz/gtjhrswmai.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtehasyldy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gttxhzhlzs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtwhqqsvjv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cashguo.top/gtqmkblbyb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.feifeiyinyue.top/gtgpeuhtgf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pycfn.com/gtcyobvuro.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtfozqdcai.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gtnscqfqyq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtwecnjxgd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hfpthk.cn/gtlgdfttfr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhengqikj.top/gtzretesnr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtojbmuwzo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtszawoblf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zycfv.cn/gtthptvfto.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.havefunace.top/gtdegrdzjl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.smart0.xyz/gtbgujohti.html

[F05] 判断文件或目录是否存在
来源：http://hz.jiagoushi.top/gtzoeeechp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtpfhvrsoe.html

PHP:  file_exists("a.txt");
来源：http://hz.52xcode.cn/gtdiwqvfmd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtfbuqyqyv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtlzhqpguw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gticvfyraw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.havefunace.top/gtmtrckwib.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhongyouzk.top/gtzkinguxk.html

C#:   File.Exists("a.txt")
来源：http://hz.jlsjyb.cn/gtoaywplry.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtxqesrqvc.html

Py:   os.remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtmibtoaur.html

PHP:  unlink("a.txt");
来源：http://hz.hysaishi.cn/gtsptbsyuq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtqixgshot.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtfxxpzzcr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtiliuahnl.html

Go:   os.Remove("a.txt")
来源：http://hz.zhoulong.xyz/gtgsqvxzdm.html

Ruby: File.delete("a.txt")
来源：http://hz.yangfankeji.com/gteyagmpgd.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtjmxhpbth.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gtkkjfewvp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtejevqdxk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhoulong.xyz/gtczeugink.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtvzhrthkc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtrnprsivn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.mhx1999.top/gtydnwcbjr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtwfkqcgro.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigfzy.top/gtxvmfpclk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cucudq.cn/gtaksheuns.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtfbzlpndj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtiyzcbiwz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtgppwqkek.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gteffryxjk.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgufenzy.top/gtzrfgnrym.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtkrwshlyg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtedkiytsd.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtdavysvic.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hammf.cn/gtycexxvjd.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtopbnpoqx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.pycfn.com/gtrmeruiro.html

PHP:  filesize("a.txt");
来源：http://hz.zdqjudy.top/gtjaecipqr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtjgkragyr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtntgykrep.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtaoasdqco.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtecvjgkga.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gtsenlvkzc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tian-w.cn/gtuvubwrip.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gthzhfjrxt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtdqqxmkax.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtrbsmimsn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtekeunapt.html

TS:   path.extname("a.txt")
来源：http://hz.cdnleiting.top/gtikjvxvrv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtefsuzpky.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gtsryreonb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtxepdzicq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pycfn.com/gtirxnvoca.html

[F11] 复制与移动文件
来源：http://hz.cheryme.top/gtauezazdn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtyifdcuqz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtmiinhgpg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtprjjlotp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtenffvfhj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtrldpzssb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zycfv.cn/gtgvseccgb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtrxrqbucz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinyuanbaomall.cn/gtvwfvpjrs.html

[F12] CSV 读写
来源：http://hz.tian-w.cn/gthrvufhnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sufxvd.cn/gthonvdmzo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtvljbozkd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.havefunace.top/gtikigrxlc.html

TS:   // 同上
来源：http://hz.shuidangran.top/gtafhrjiwp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtmcknrdkp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.mhx1999.top/gtkalikyzu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shangyingyoupin.top/gtkezflian.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gtmqctiswb.html

================================================================================
来源：http://hz.cqqwz.cn/gtspkcqnvk.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtvpghzvnv.html

================================================================================
来源：http://hz.hnqzz.top/gtuycrqmze.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtplafmotg.html

Py:   class User: pass
来源：http://hz.tanke756.top/gtamfchikx.html

PHP:  class User {}
来源：http://hz.xinyue.icu/gtaejmabor.html

JS:   class User {}
来源：http://hz.sysykeji.top/gtflxohaug.html

TS:   class User { name: string = ""; }
来源：http://hz.hywenlv.cn/gtqsitgqjh.html

Java: class User {}
来源：http://hz.smart0.xyz/gtafiltyat.html

Go:   type User struct { Name string }
来源：http://hz.9152youxi.cn/gtxrjeptph.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gthaiyrnzu.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gttvbtlcvf.html

[G02] 构造函数
来源：http://hz.sweek.top/gtswfaoikz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydzc1.top/gtigutexah.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cdnleiting.top/gtprhgmusq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtrnyjchyt.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtxtfrthyq.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258888.top/gtuljoddyk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtglufuveo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtbfhftftb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtxuooexao.html

[G03] 实例属性
来源：http://hz.jinqigfzy.top/gtesvytrca.html

Py:   self.name = "x"
来源：http://hz.yj202588.top/gtglwufydp.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtygzqnvch.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gttzwpnzad.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtuwxahtuw.html

Java: private String name;
来源：http://hz.sweek.top/gtxaemrfwt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtxhddewyy.html

Ruby: @name = "x"
来源：http://hz.jinyuanbaomall.cn/gtvmopznhh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.316326.xyz/gtxspyoxky.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gtzgsetqma.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtngxpeadd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ivvv.top/gtgyruogry.html

JS:   greet() { return this.name; }
来源：http://hz.xziqi.cn/gtdmohkeio.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gttkbattrz.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtrooqtypj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aizwys.cn/gtxdftndel.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtckawcxvi.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtmmsygafl.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtofgtizeg.html

Py:   class Admin(User): pass
来源：http://hz.yj20258888.top/gtoougxwpd.html

PHP:  class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gteakpmnqo.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtxypdhhnn.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtzwnawdvj.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtvdteudih.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtxrknpwvj.html

Ruby: class Admin < User; end
来源：http://hz.shzxlz.cn/gtfgbkduao.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtqlrroupt.html

[G06] 重写方法
来源：http://hz.vqdsnc.cn/gtdnxanfwv.html

Py:   def greet(self): return "admin"
来源：http://hz.zhoulong.xyz/gtwbgfhvlk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtfoaegcdw.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtitpfotdn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtylitbdlk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtmwhchlzx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtgtpagcdk.html

Ruby: def greet; "admin"; end
来源：http://hz.52xcode.cn/gthvksaxvt.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtmqmwfifb.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtcxqtcooc.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gtnmuqwtbb.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gtdlhhisub.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtupgqblud.html

TS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtwudyehre.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtzopfeswl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtwwjeifdo.html

Ruby: super
来源：http://hz.yongpay.top/gtvazwvdgq.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gttqaltshb.html

[G08] 静态方法与属性
来源：http://hz.c1oappe.top/gtfkdjiwpp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.vqdsnc.cn/gtdqnizeml.html

PHP:  public static function f() {}
来源：http://hz.316326.xyz/gtfwuaknvd.html

JS:   static f() {}
来源：http://hz.aibaodan.cn/gtgsyadlsg.html

TS:   static f(): void {}
来源：http://hz.chenjidiqi.icu/gtirvebrqj.html

Java: static void f() {}
来源：http://hz.ywan-chungtsiang.top/gtsdlkpcjv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aibaodan.cn/gtsqmqfbbn.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtugxiutaz.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtrpifcgts.html

[G09] 接口 / 抽象类
来源：http://hz.tianlin.xyz/gtqritwiml.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtxbatqhfq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtibztflba.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gtkzfnjpjg.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtvtcegqeb.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtrkqasnxs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtogfvemfo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ivvv.top/gtheimzwfh.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtqczwqyys.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtnfffrpug.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtjfvlcxmb.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtreugaisv.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtjpjbyvsb.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtldtvqayy.html

Java: public / protected / private / 默认包级
来源：http://hz.tianlin.xyz/gtaufbqmyf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gtnjajnaqs.html

Ruby: public / protected / private
来源：http://hz.shzxlz.cn/gtplarmveq.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtkhnjqxsb.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gttexhzjmy.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258888.top/gtxespvqdr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtpknldcuj.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigufen.top/gtqwzlxuuy.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gtbtyzxjwi.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gtidbigndh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtciahsrnm.html

Ruby: attr_accessor :name
来源：http://hz.hnqzz.top/gtjuurhzyy.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtfdovosuh.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtnxggqugd.html

Py:   def __str__(self): return self.name
来源：http://hz.shuidangran.top/gthkzmizdv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gthhxfglto.html

JS:   toString() { return this.name; }
来源：http://hz.svipenyu.cn/gteglmxobx.html

TS:   toString(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtlvnasvmg.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtriwfdcgi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ivvv.top/gtzyfdmktk.html

Ruby: def to_s; @name; end
来源：http://hz.xziqi.cn/gtegfzlrrp.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtskngqivf.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtvnuqbdtg.html

Py:   isinstance(u, User)
来源：http://hz.iojbl.cn/gtoqipxitq.html

PHP:  $u instanceof User
来源：http://hz.jqgfzy.top/gtrbeigric.html

JS:   u instanceof User
来源：http://hz.xinyue.icu/gtmakzsmvi.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtnvobpvbt.html

Java: u instanceof User
来源：http://hz.birdmap.top/gtdrodwjhw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.smart0.xyz/gtxcgtxsif.html

Ruby: u.is_a?(User)
来源：http://hz.ydzc1.top/gtrujtedgd.html

C#:   u is User
来源：http://hz.pycfn.com/gtocvipddh.html

[G14] 数据类 / record
来源：http://hz.tian-w.cn/gtvlvixxny.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ppjwa.cn/gtalghktnd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.snrcjt.cn/gtxsgrqmxk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aibaodan.cn/gtxcnjqmsw.html

TS:   type User = { name: string; age: number };
来源：http://hz.zdqjudy.top/gtqiwrrplb.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtaaqtlney.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gttvbgbooc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhaomingkeji.xyz/gtvnookzga.html

C#:   record User(string Name, int Age);
来源：http://hz.yuanzhike.top/gtfdryiehm.html

[G15] 枚举
来源：http://hz.tanke756.top/gtykzkbkyt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.9152youxi.cn/gtoqktsawj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gtbihfcpye.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxuanxn.top/gtcrrgmwml.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtechsynnk.html

Java: enum Color { RED, GREEN }
来源：http://hz.yangfankeji.com/gtvchmjiom.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtzcddaoau.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cdnleiting.top/gtfwnzjutp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtjnttzozi.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtvqinflna.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhoulong.xyz/gtmekmlltm.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtqvkxjvrf.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtpctmgbtw.html

TS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gtsjhlitol.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtvmfdxeyl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtrmwnktfn.html

Ruby: obj.instance_variables
来源：http://hz.fzhhl.top/gtqnlzpqot.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtrnglfqxn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdzxwymwu.html

H. 异常与错误处理
来源：http://hz.zhiwuduotai.top/gtosubamhr.html

================================================================================
来源：http://hz.cucudq.cn/gtiqikbcqc.html

[H01] try / catch 基础
来源：http://hz.hysaishi.cn/gtogwmyoso.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtvdogucwz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gtcnolqfjy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtxxwrrage.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yueranfly.top/gtonhomwgm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtykyijtug.html


<!-- 参考信息 -->