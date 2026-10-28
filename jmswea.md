代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gtridyliqh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtfyjhxsdt.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtnuwxarzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtlarxgriu.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtfmawsnka.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tanke756.top/gtopswdmsf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenjidiqi.icu/gtsbvzmcjx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gthgzpmdlk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtnkhlwbuo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydzc1.top/gtyzgzeizd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.feifeiyinyue.top/gtvelaahst.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ywan-chungtsiang.top/gtsmeycors.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258.top/gteumutzbb.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtpblfjbqw.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtgspascob.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hfpthk.cn/gtmdfzpuhy.html

JS:   s.split(/\r?\n/)
来源：http://hz.xingfuxueyuan.xyz/gtggjgsusu.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtljzxnuba.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtvxtwbjui.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhengqikj.top/gtxkgwjkcf.html

Ruby: s.lines
来源：http://hz.nanxuanxn.top/gtzavmwsnn.html

C#:   s.Split('\n')
来源：http://hz.dashuyun.cn/gtxlirqwnb.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtebafybwu.html

Py:   if not s:
来源：http://hz.vqdsnc.cn/gtsfnftkhv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtcekoirhc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtzjtrrbyu.html

TS:   if (s === "") {}
来源：http://hz.jlsjyb.cn/gtleprpmot.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtcyqmkoyg.html

Go:   if s == "" {}
来源：http://hz.hysaishi.cn/gtndmqwejl.html

Ruby: if s.empty?
来源：http://hz.gzhubu.top/gtojpdrwvo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.mhx1999.top/gtymsotdjh.html

[E21] 超长截断加省略号
来源：http://hz.jiagoushi.top/gtqkwtacjp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtaaofmign.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gaohongyu789.top/gthrcbnrud.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtkmffubdj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtmgjmzbeh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtozytgpbp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fzhhl.top/gtttzxansp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtevocxkbi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxuanxn.top/gtogpeciqm.html

[E22] 字节长度与字符长度
来源：http://hz.hysaishi.cn/gtzrnbrqvn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhaomingkeji.xyz/gtplxdsulm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtpohjphzm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtxfmdhmvu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtbtlnctds.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yvedp.cn/gtnldmuitx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ybcxt.top/gtudrbjkfp.html

Ruby: s.bytesize;  s.length
来源：http://hz.sxryk.cn/gtfgwiawae.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuxming.cn/gtsurqajnw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtlomgeoaw.html

F. 文件与目录
来源：http://hz.smart0.xyz/gtawszvsub.html

================================================================================
来源：http://hz.yvedp.cn/gtxubsltau.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtkuqxeviv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yuxming.cn/gtjyvrzlns.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yongpay.top/gtzyyfbfla.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sysykeji.top/gtvpxvcuqw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgufenzy.top/gtsjkmjsfp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtweoueajc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.smart0.xyz/gtwiumrpoc.html

Ruby: File.read("a.txt")
来源：http://hz.ivvv.top/gtiifzelob.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.svipenyu.cn/gtzlsocbfd.html

[F02] 逐行读取文件
来源：http://hz.aizwys.cn/gtiddvvnbd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jianghu66.top/gtnflctesv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aizwys.cn/gtjzhqjaeg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtfptxqwpv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtxyzvfmws.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.quarkkingdee.top/gtkonkgvyk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtkzgxencu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtcteivseh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.daxiang520.top/gtowtmucqa.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gtdmjnvrve.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jianghu66.top/gtqxmcclcd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtnbcuiasv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shzxlz.cn/gtyyyadfwg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.0kj1m.cn/gtmuhgoiek.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtzeltoezt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gtuhzuczka.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ywan-chungtsiang.top/gtdgtqldkr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gtxmuaghzi.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gttecuuhgx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cqqwz.cn/gtfwnhyriv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yvedp.cn/gtvyidrqbc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtwgzalgjd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtcyexnkgp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hongshengwenyu.top/gtvdxenblk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cheryme.top/gttjesbkag.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.0kj1m.cn/gtjfwsgmrk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jlsjyb.cn/gtflpvgqdb.html

[F05] 判断文件或目录是否存在
来源：http://hz.jinqigufen.top/gtcfnawssj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtvhvtusnt.html

PHP:  file_exists("a.txt");
来源：http://hz.sweek.top/gtfhxcpqai.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtqgnioayd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtmbuilkuz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtivbvypfd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gtkvrpsstw.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuanzx.com/gtncfkmgon.html

C#:   File.Exists("a.txt")
来源：http://hz.gzhubu.top/gtzrynomfk.html

[F06] 删除文件
来源：http://hz.chenzaomai.com/gtxyavtbev.html

Py:   os.remove("a.txt")
来源：http://hz.yuanzhike.top/gtbxshcllo.html

PHP:  unlink("a.txt");
来源：http://hz.cucudq.cn/gtzietbjeu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtgerdwjak.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtceoluvru.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtpkixmilm.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gtdwnlthlb.html

Ruby: File.delete("a.txt")
来源：http://hz.yuanzhike.top/gtbprzkihb.html

C#:   File.Delete("a.txt");
来源：http://hz.gogol.net.cn/gtlhkzuagg.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gttweuhnak.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtjounybml.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cqqwz.cn/gtpbeqapen.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtgcbplvku.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtosvypiap.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xylfe.cn/gtcrwwqzbd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhiwuduotai.top/gtwgismwcf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tianlin.xyz/gtilhgcrwv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhaomingkeji.xyz/gtssbqcsim.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gttpghjwss.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cdnleiting.top/gtwmrdtqkg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gttzitgwlr.html

JS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtuxjqkyqb.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtcoifbvoq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtyjlxyugg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ivvv.top/gtcwejuevn.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtldmacuuy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.9152youxi.cn/gtmbftnttm.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtmgybrulx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ybcxt.top/gtormroxqy.html

PHP:  filesize("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtybotwtdx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gthogmaccs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yonumen.top/gtoiiyxsjf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtomszxpph.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shuidangran.top/gtkijyvkqo.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtgqmafqxs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nwbrower.top/gtrouocpoa.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gttxadqjbo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtmifipznh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxuanxn.top/gtxitchhgz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtnhzaqsoj.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtuhwzmovb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.andypj.xyz/gtuaiylimt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gtzfqrztoz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtkljknjrz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yonumen.top/gtqijnxiyt.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtdwuqumww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtzqkkigds.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtnijahwkf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtdpabifcr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtcsfgxubv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenlongwang.top/gtwmrezfbu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gtilenkjyn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtmptjxngh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gthfxmohnr.html

[F12] CSV 读写
来源：http://hz.tanke756.top/gtdouocpmk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ywan-chungtsiang.top/gtbdlciyhf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gtzopkirep.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtkntdzseq.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtjfyjvwte.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258888.top/gtjjptsmni.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtpbhwdezq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cashguo.top/gtjkskrplv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zycfv.cn/gtgkmrjktk.html

================================================================================
来源：http://hz.cashguo.top/gtjawfifik.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gthfuydhwd.html

================================================================================
来源：http://hz.hammf.cn/gtroxmyvbw.html

[G01] 定义类
来源：http://hz.hysaishi.cn/gtqnwiqryg.html

Py:   class User: pass
来源：http://hz.hammf.cn/gtzltsstro.html

PHP:  class User {}
来源：http://hz.cashguo.top/gtrpjobmpv.html

JS:   class User {}
来源：http://hz.chenjidiqi.icu/gtlotwcjwm.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtbsqnlame.html

Java: class User {}
来源：http://hz.jinqigufen.top/gtbqmgoyjj.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gtchqwdhys.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gtaptzstyk.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtcsehdjhs.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtjnqiknam.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtejktbljn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pengpengdd.cyou/gtitroigak.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtugjeiifc.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigufen.top/gtxciwsiui.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtthtorrfg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtiitvhqix.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yanxiufei.cn/gtlyfxypbz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtawbzdhzy.html

[G03] 实例属性
来源：http://hz.zhixingplan.top/gtosahqwwi.html

Py:   self.name = "x"
来源：http://hz.chenjidiqi.icu/gtstylhxck.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtlhkmnbmu.html

JS:   this.name = "x";
来源：http://hz.hammf.cn/gtfacqkeph.html

TS:   name: string = "x";
来源：http://hz.cqqwz.cn/gtlqtfiayx.html

Java: private String name;
来源：http://hz.shuidangran.top/gtmnxfppvp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dashuyun.cn/gtmhwaqiwj.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtfiepowtb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtekmhgcns.html

[G04] 定义方法
来源：http://hz.shanyushiyangkeji.top/gtbemunumh.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtitjqxiyi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtzcscxqun.html

JS:   greet() { return this.name; }
来源：http://hz.chenzaomai.com/gtskihczab.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtqtfndrcw.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtjhumlgcg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xinyue.icu/gtgvklrika.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtjtvbuwva.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtfuicezgq.html

[G05] 继承
来源：http://hz.shuidangran.top/gtsyylbhkh.html

Py:   class Admin(User): pass
来源：http://hz.cheryme.top/gtedygqwve.html

PHP:  class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtvfvyvrfu.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtspilhexf.html

TS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtsxiozszg.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtzptfxzkh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtnwbhhdua.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtswbyoano.html

C#:   class Admin : User {}
来源：http://hz.cucudq.cn/gtauwpqqij.html

[G06] 重写方法
来源：http://hz.quarkkingdee.top/gtfzkhbndv.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gteuakkbjy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtsrmextwp.html

JS:   greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtvurujaxn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtnirwxckc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtljdzjdqi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtpvttkqtb.html

Ruby: def greet; "admin"; end
来源：http://hz.jiagoushi.top/gtnezsotbu.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtbxevvpnx.html

[G07] 调用父类方法
来源：http://hz.havefunace.top/gtgzingejs.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtqzrwwdih.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtsdufamsq.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtyeupuajl.html

TS:   super.greet();
来源：http://hz.jyoumei.cn/gtkourwfxb.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtcneuldox.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtegkhunrn.html

Ruby: super
来源：http://hz.jinqigfzy.top/gtxdwujazq.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtdfcfobbp.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtwhhtwfgc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydzc1.top/gtsmjxboaj.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtuqjhjdym.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtuwdujikv.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gtfxhavgzc.html

Java: static void f() {}
来源：http://hz.ppjwa.cn/gtfsvlbjnv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtltidrcpi.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtbhvduexp.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtqtzvntvr.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtkrtwrium.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtskglwxzc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gttkjwhksx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtwkxxgyhy.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtlaikwuvx.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gtjxgtpthv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sysykeji.top/gtmegdtgba.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.andypj.xyz/gtgloipxwj.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangtech.top/gtqjtaifvs.html

[G10] 访问控制
来源：http://hz.gogol.net.cn/gtwgvpkxiu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtzhbwnjhl.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtreikcqah.html

JS:   #private 字段；其余公开
来源：http://hz.ydjk.org.cn/gttttfucwt.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtvowjimcz.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtsaryvuaf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtairiyqvo.html

Ruby: public / protected / private
来源：http://hz.gaohongyu789.top/gtajtkhhux.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gtzjeupwtn.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtkisraywl.html

Py:   @property 与 @x.setter
来源：http://hz.jinghuilouyu.cn/gtumylzjgq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtmgurjqpz.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtlbimjgyt.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtyyqrgkfh.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtkgrzktga.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtwfadpjzu.html

Ruby: attr_accessor :name
来源：http://hz.jlsjyb.cn/gtkrxaazsf.html

C#:   public string Name { get; set; }
来源：http://hz.wangshuangyany.cn/gtmxxwuzya.html

[G12] 对象转字符串
来源：http://hz.chenlongwang.top/gtnuliwsex.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258.top/gtlnuhonms.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtonzwxnpn.html

JS:   toString() { return this.name; }
来源：http://hz.svipenyu.cn/gtdicrtmel.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gttxltnfin.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnqzz.top/gthvctwjrw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.snrcjt.cn/gtygfujlct.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtiojayepe.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtbwvdjrvp.html

[G13] 判断对象类型
来源：http://hz.bjfxy.top/gtlznfwwos.html

Py:   isinstance(u, User)
来源：http://hz.c1oappe.top/gtsfzkwcgu.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtbhormumd.html

JS:   u instanceof User
来源：http://hz.wangdashe.top/gtszkhmrrj.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtbsfleglb.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtrqscypco.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtbpfksnxe.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtbjiwpjdc.html

C#:   u is User
来源：http://hz.fzhhl.top/gthqpvqonq.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtdmcvwmpy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtfcaeqfoh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shuidangran.top/gtmcisyhss.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.quarkkingdee.top/gtzlbtwxsg.html

TS:   type User = { name: string; age: number };
来源：http://hz.sxryk.cn/gtxvcxckin.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtiblbrxex.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhengqikj.top/gttwflsvoo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xziqi.cn/gtfvbohhob.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gtnpaufosz.html

[G15] 枚举
来源：http://hz.gzhubu.top/gtwgxyvbmw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtwwkldtwp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtvhfwwexp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gthumascsx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gthgjttint.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtzgfisvod.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fengsongda.top/gttxpqbjsy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ybcxt.top/gtpgnallfm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtzlmmshqv.html

[G16] 对象转数组 / 字典
来源：http://hz.tanke756.top/gtxgeyiifq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.birdmap.top/gtbusozmmx.html


<!-- 参考信息 -->