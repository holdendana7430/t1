代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtsniilixq.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtuudabuyc.html

Py:   s.splitlines()
来源：http://hz.sxryk.cn/gtgaasfkrr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sufxvd.cn/gthebrogny.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtfsqnkqai.html

TS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtmoxyhpys.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtwrgtdqgo.html

Go:   strings.Split(s, "\n")
来源：http://hz.yongpay.top/gttpkxdqlh.html

Ruby: s.lines
来源：http://hz.sweek.top/gtvzhtmgdo.html

C#:   s.Split('\n')
来源：http://hz.hywenlv.cn/gtegxnkerq.html

[E20] 判断字符串是否为空
来源：http://hz.fengsongda.top/gtrhiallvi.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtpjhcfeip.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenjidiqi.icu/gtiwhzurxs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhaomingkeji.xyz/gtbvcqpwzj.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtmcrhpnlv.html

Java: if (s.isEmpty()) {}
来源：http://hz.yanxiufei.cn/gtgrublaze.html

Go:   if s == "" {}
来源：http://hz.xuanzx.com/gtuwycuudg.html

Ruby: if s.empty?
来源：http://hz.hysaishi.cn/gttmyipihs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenjidiqi.icu/gtneblhpia.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gttazrluxo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ydjk.org.cn/gtrofsoedf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangdashe.top/gtiznhxpzo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtnpdxqias.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gtfedchvhw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtkxewctzk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gtzvayjxpj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zdqjudy.top/gtcvtikwxd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.vqdsnc.cn/gtsliedpei.html

[E22] 字节长度与字符长度
来源：http://hz.zhoulong.xyz/gtwwrrzmfp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xuanzx.com/gtvzuzuvvh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ppjwa.cn/gtcnpeuryu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gthesvolhu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtqpycygdu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cucudq.cn/gteniprccu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.mhx1999.top/gtgqqsaawp.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxuanxn.top/gtecislsvl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtnjzerbnm.html

================================================================================
来源：http://hz.haohaochexian.top/gtzjoctfjl.html

F. 文件与目录
来源：http://hz.cucudq.cn/gtbncrsndd.html

================================================================================
来源：http://hz.gogol.net.cn/gtkofvauzr.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gtikhbyanx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtbgewrqrk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhengqikj.top/gtcjlqxxux.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ehwqpu.com/gtbrtshphj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gtcbqifwah.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gthnntkrrd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jiagoushi.top/gtdwucjlru.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtxfhbempr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.smart0.xyz/gtcyznuisx.html

[F02] 逐行读取文件
来源：http://hz.jqgufenzy.top/gtrxzvdwwu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenzaomai.com/gtcqyndwxq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangdashe.top/gtplzokiqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtwziccayd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtbvllvprv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtnuppscvv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtvtvnqgfh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtwobqjysz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtpxhohpon.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtbhtsukhh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenzaomai.com/gthlxmwcvj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258.top/gtoeqvgfvb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xingfuxueyuan.xyz/gtnmutqqpm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtysckitmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jianghu66.top/gtgdwsacaa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigufen.top/gtnxjiiuvn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.0kj1m.cn/gtkagurxya.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gthydocvmr.html

[F04] 追加写入文件
来源：http://hz.aibaodan.cn/gtbqjpyrby.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.birdmap.top/gtrdabdzab.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gtyqnsxagr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtwzgemxpa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtmarbftez.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtjpejntdf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinqigfzy.top/gtjpwuxfng.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtbeoynufv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zdqjudy.top/gtsdwkgidd.html

[F05] 判断文件或目录是否存在
来源：http://hz.vqdsnc.cn/gtbnksykyp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tianlin.xyz/gtkxkvdrcd.html

PHP:  file_exists("a.txt");
来源：http://hz.ydzc1.top/gttpucjkpv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtjpftecgl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpvjihtnz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gtabtrnhuz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cdnleiting.top/gtjbxfppgr.html

Ruby: File.exist?("a.txt")
来源：http://hz.fzhhl.top/gteuybqvsm.html

C#:   File.Exists("a.txt")
来源：http://hz.wangdashe.top/gtckgglgsf.html

[F06] 删除文件
来源：http://hz.zycfv.cn/gterojpzlh.html

Py:   os.remove("a.txt")
来源：http://hz.shzxlz.cn/gtavqutfot.html

PHP:  unlink("a.txt");
来源：http://hz.52xcode.cn/gtzwlqnlgo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtscgjmajp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtnahydfno.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtgsylgdfh.html

Go:   os.Remove("a.txt")
来源：http://hz.cheryme.top/gtoloutsij.html

Ruby: File.delete("a.txt")
来源：http://hz.xuanzx.com/gtjnyjtmsf.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtoxfnjpuy.html

[F07] 创建目录（含多级）
来源：http://hz.shzxlz.cn/gtcngwjavo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nwbrower.top/gtxhwienep.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jianghu66.top/gtzoepwjtj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtudneojrc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gtyamxslia.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yangfankeji.com/gtehfualfc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aibaodan.cn/gtmatmiyik.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gtpitrjcry.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtwqvnyroh.html

[F08] 遍历目录
来源：http://hz.sweek.top/gtnwsulmwx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtrewkuaxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuetiantiany.cn/gtknaumsxl.html

JS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtingurtkt.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtzdwsblwe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtzdzihchq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aizwys.cn/gtdpwktpkp.html

Ruby: Dir.children("dir")
来源：http://hz.ivvv.top/gtkajfheof.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fzhhl.top/gttdsnargb.html

[F09] 获取文件大小
来源：http://hz.yj202588.top/gtsdldtbqx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinghuilouyu.cn/gtdcwjlkgj.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtnowsybys.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daxiang520.top/gtccgmppca.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtmmerzsrv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtqliqiozb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtvjepurjg.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtkbgrhovp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtoliecaxz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtnypkiovp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtbyesjhhl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.haohaochexian.top/gtpzrhdxiy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtyyqlcywl.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtyhcmyyby.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gtvcttodir.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gtbjopufiq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtocygfnab.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gtaaktwvdn.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtkafvkbaz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtowddtbre.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.birdmap.top/gtcrvfsolg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtbusylpzr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtoevoobnu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shuidangran.top/gtonkluypj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhiwuduotai.top/gtlffqjvjw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtlqhzarmy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jyoumei.cn/gtzgfnbatm.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gthbwjqzaz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtaahuzcnu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtfsqvrebu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigfzy.top/gtrtuppdjk.html

TS:   // 同上
来源：http://hz.hfpthk.cn/gtxifbtszd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtrgfjaupc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cucudq.cn/gtwboekawd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gthehfipth.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gtagtmluho.html

================================================================================
来源：http://hz.yongpay.top/gtdmxwctam.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtrpfnevit.html

================================================================================
来源：http://hz.quarkkingdee.top/gtutaovqmj.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtnhiwzimn.html

Py:   class User: pass
来源：http://hz.yueranfly.top/gtiifzmbjg.html

PHP:  class User {}
来源：http://hz.316326.xyz/gthdphwcbr.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtnntmfwza.html

TS:   class User { name: string = ""; }
来源：http://hz.hfpthk.cn/gtrmmrmxfq.html

Java: class User {}
来源：http://hz.tian-w.cn/gtolfcqnnj.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtigsdnaly.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtcpilfdit.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtzuvbsewm.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtzxdxueqy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shuidangran.top/gtohemyoug.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.316326.xyz/gtnamwaose.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gttjfzuiaf.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258888.top/gthfmouube.html

Java: User(String name) { this.name = name; }
来源：http://hz.nwbrower.top/gtbodfmzhs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.dianchejie.cn/gtmqzszknx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtvnpqsrna.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fzhhl.top/gtkuadlzry.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gtvunmkbls.html

Py:   self.name = "x"
来源：http://hz.gogol.net.cn/gtyxkkaoqd.html

PHP:  public string $name = "x";
来源：http://hz.chenlongwang.top/gtuajchduw.html

JS:   this.name = "x";
来源：http://hz.tianlin.xyz/gtjewxrlok.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gtylfdkpuc.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtmzzzeefy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtpgofennf.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtddmybpbe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gtszhvknwg.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtxdaxuftn.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtpwqbovlk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtwoifuvgw.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtlinwzczt.html

TS:   greet(): string { return this.name; }
来源：http://hz.316326.xyz/gtkzwvvvhs.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gthbpaoagm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtmjilcrxn.html

Ruby: def greet; @name; end
来源：http://hz.svipenyu.cn/gtmpcjkhul.html

C#:   public string Greet() => Name;
来源：http://hz.zhongyouzk.top/gtexhpmjff.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtdmgibhgr.html

Py:   class Admin(User): pass
来源：http://hz.chenzaomai.com/gtutaympui.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtxmnhmymc.html

JS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtyatzopjp.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtztguwzkc.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtomhnrteb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fengsongda.top/gtfjgmtgxs.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtjmllqomy.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtprriebhr.html

[G06] 重写方法
来源：http://hz.hywenlv.cn/gtfjogammq.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtzujbexlu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gthmzprgbw.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtprbqfnsx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtxscvrluw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtgczjppdd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.quarkkingdee.top/gtrfxwdtya.html

Ruby: def greet; "admin"; end
来源：http://hz.ppjwa.cn/gtmovctbox.html

C#:   public override string Greet() => "admin";
来源：http://hz.cqqwz.cn/gtakvsimit.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtxrtscpeg.html

Py:   super().greet()
来源：http://hz.chenjidiqi.icu/gtblrcacva.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gturpvngnx.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gtbejaabuf.html

TS:   super.greet();
来源：http://hz.hfpthk.cn/gtcztjpeiv.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtwsftorgp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yanxiufei.cn/gtvvhjburc.html

Ruby: super
来源：http://hz.chenzaomai.com/gtoxwaaubb.html

C#:   base.Greet();
来源：http://hz.pycfn.com/gtzpvtcihh.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtiicztxuh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtjjhlgpch.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtrsdyyouh.html

JS:   static f() {}
来源：http://hz.xuanzx.com/gtlrfhdbgi.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtmlygqycc.html

Java: static void f() {}
来源：http://hz.andypj.xyz/gtpxmhxnpr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zycfv.cn/gtecepoecr.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gthdhkgivg.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gtkqyypows.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gtamlwbpao.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtmlyfqzgt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shanyushiyangtech.top/gtkdveavyw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aizwys.cn/gtldchhlkb.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtzfqlhshf.html

Java: interface Shape { double area(); }
来源：http://hz.chenlongwang.top/gtyohzcvzv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtedvcozvu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yvedp.cn/gtbzelbrwv.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuxming.cn/gtbkvktsvz.html

[G10] 访问控制
来源：http://hz.xingfuxueyuan.xyz/gteabheqgt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gttujdkvjz.html

PHP:  public / protected / private
来源：http://hz.smart0.xyz/gtjincowiz.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtbnlylutf.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtskjdzexx.html

Java: public / protected / private / 默认包级
来源：http://hz.9152youxi.cn/gthpaesxxo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtyuvpefjt.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtbbmrxsys.html

C#:   public / protected / private / internal
来源：http://hz.xingfuxueyuan.xyz/gtdzdurxaa.html

[G11] getter / setter
来源：http://hz.sweek.top/gtmblxfuha.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gtutnzmohn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtowdwzagv.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtjyywjfhf.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtepprigbk.html

Java: public String getName() { return name; }
来源：http://hz.andypj.xyz/gtyagtnluh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pycfn.com/gttydugyif.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtcfbrbpfr.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gtnrzozczr.html

[G12] 对象转字符串
来源：http://hz.guannengcc.top/gtcuzcvmwg.html

Py:   def __str__(self): return self.name
来源：http://hz.hammf.cn/gtajatvqpp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtttsxiqcw.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258.top/gtivgyittu.html

TS:   toString(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gttqxwutoo.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gtlusubbxd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtoufijobj.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtoiqefbyq.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtnerhyokt.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtnddzheyr.html

Py:   isinstance(u, User)
来源：http://hz.52xcode.cn/gtlwxareip.html

PHP:  $u instanceof User
来源：http://hz.iojbl.cn/gtacknjxwh.html

JS:   u instanceof User
来源：http://hz.ybcxt.top/gtljsukehm.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtfoxdtlud.html

Java: u instanceof User
来源：http://hz.ivvv.top/gtwuawwlsr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtrqvgconz.html

Ruby: u.is_a?(User)
来源：http://hz.shanyushiyangtech.top/gtyfajacqu.html

C#:   u is User
来源：http://hz.jiagoushi.top/gtrdmppwmv.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtjoqxghgk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guannengcc.top/gtcfrcbhmu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gtqbaacrhu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtfqnlhozc.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhoulong.xyz/gtuqnasumz.html

Java: record User(String name, int age) {}
来源：http://hz.ehwqpu.com/gtkopsjyhn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gtnylnzrkt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shuidangran.top/gtmlcopetq.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtiatcsqkm.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtmkdbihul.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtmcegluxp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtagiyiewb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gtsygpkkbs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtrudnwmbt.html

Java: enum Color { RED, GREEN }
来源：http://hz.vqdsnc.cn/gtwkuzvizl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtkkxbdhkv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dianchejie.cn/gtthysbika.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtmnztbbfh.html

[G16] 对象转数组 / 字典
来源：http://hz.0kj1m.cn/gtpagyskyv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.svipenyu.cn/gtuyondutk.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtfhdqtjah.html

JS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtgkymbvuz.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtwucvbxor.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtvjoztwwm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtemoidgeh.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtfdxqvbgc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj202588.top/gtvcvyfajq.html

================================================================================
来源：http://hz.gaohongyu789.top/gtvlsruqrt.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtwoznmmdk.html

================================================================================
来源：http://hz.jyoumei.cn/gtmrenussy.html

[H01] try / catch 基础
来源：http://hz.aibaodan.cn/gtktwnletx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cucudq.cn/gtgthoicqa.html


<!-- 参考信息 -->