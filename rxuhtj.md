代发 wailian999

[E18] 模板占位符替换
来源：http://hz.xuanzx.com/gthdcxvril.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtecrocpgl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtqaxaatsl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtngivrzpb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtqofrcolm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtrxbkqbta.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnxiangtu.top/gtdglyiqrm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cucudq.cn/gtzhusmenn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shangyingyoupin.top/gtkqeoykio.html

[E19] 多行文本按行拆分
来源：http://hz.sufxvd.cn/gtctlvkkao.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangtech.top/gtegtjpnzz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gogol.net.cn/gtsysmpzsh.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtinyqbdlj.html

TS:   s.split(/\r?\n/)
来源：http://hz.hysaishi.cn/gtxcguecnd.html

Java: s.lines().toList()
来源：http://hz.jinqigfzy.top/gtwcceljyj.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtriuzsaje.html

Ruby: s.lines
来源：http://hz.0kj1m.cn/gtcgzjvalq.html

C#:   s.Split('\n')
来源：http://hz.yuxming.cn/gtpaqmgwai.html

[E20] 判断字符串是否为空
来源：http://hz.nanxinkj.top/gtivkjunle.html

Py:   if not s:
来源：http://hz.daria6918.cn/gtkqtuuplx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydzc1.top/gtirbifjxv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.vqdsnc.cn/gtjhetigpc.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gtdugmaftq.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtpmsuoton.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtpmkprgfp.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtbuonhswu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenlongwang.top/gtcktdaopl.html

[E21] 超长截断加省略号
来源：http://hz.jiagoushi.top/gtkhhbnero.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.fzhhl.top/gtvzyxrozp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtcusmrqef.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtbdowbgfu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtliwmhski.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtgcawkeuq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yonumen.top/gtedrnhwbn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guannengcc.top/gtoahbiehu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtdajnheja.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangtech.top/gtgpmmkwzx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ehwqpu.com/gtktvzwrex.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.svipenyu.cn/gtvrxfnjky.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtpapyipjk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtgwfzbvlq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tianlin.xyz/gtlutvsfma.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ybcxt.top/gtyjqqnzgd.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhengqikj.top/gtnseerytw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shuidangran.top/gtqtlbnfiw.html

================================================================================
来源：http://hz.vqdsnc.cn/gtkbejwjjb.html

F. 文件与目录
来源：http://hz.hywenlv.cn/gtywgxhhzd.html

================================================================================
来源：http://hz.yj202588.top/gtssgiekpk.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtlkaxgims.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtbvkbnbve.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxuanxn.top/gttrzmzfce.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gthcyzioxa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtialmxsbf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtcbjqyilv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xziqi.cn/gtgnjukgfk.html

Ruby: File.read("a.txt")
来源：http://hz.dashuyun.cn/gtualrlhot.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.daxiang520.top/gtnjjtxvlx.html

[F02] 逐行读取文件
来源：http://hz.xinyue.icu/gtkexdvgib.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.wangshuangyany.cn/gttskfcozk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtrekqttoc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtoqxkdski.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtoosxpscy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.pengpengdd.cyou/gtfscgvzlh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.svipenyu.cn/gtgffapcwx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtgdmlwugm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.andypj.xyz/gtinltavxo.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtnbkmdxrj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ivvv.top/gtmewjfqbo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gzhubu.top/gtyvuzzqvd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtpseucmms.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtjwvmgcgt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pengpengdd.cyou/gtejwtdxny.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.haohaochexian.top/gtnspsumft.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.kuanghao11.cn/gthuuscphy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtqzudftgd.html

[F04] 追加写入文件
来源：http://hz.hywenlv.cn/gtmkximxwp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ywan-chungtsiang.top/gtzedproud.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtidrmtcfx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtymbtiiww.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.iojbl.cn/gtlnmxvboy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hongshengwenyu.top/gtikastesx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aizwys.cn/gtmuuxaprc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtvibwoxxy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.quarkkingdee.top/gtbizvkoap.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtqbnrzmkg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtfowyayae.html

PHP:  file_exists("a.txt");
来源：http://hz.wangshuangyany.cn/gtjsukovle.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xylfe.cn/gtecatetit.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtarxmlxxf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtigilzbzl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gtaswudpvv.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinqigufen.top/gtrfdjdwqn.html

C#:   File.Exists("a.txt")
来源：http://hz.svipenyu.cn/gthaarqxec.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gtqmrlmcvf.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtigmwatnl.html

PHP:  unlink("a.txt");
来源：http://hz.gotoacloud.top/gtotchhzhm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtlddorebv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gttgwbttws.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtgiiafate.html

Go:   os.Remove("a.txt")
来源：http://hz.fengsongda.top/gtuvjnttif.html

Ruby: File.delete("a.txt")
来源：http://hz.yuanzhike.top/gtcuqnxoyj.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtcmffgwow.html

[F07] 创建目录（含多级）
来源：http://hz.zhiwuduotai.top/gtxpmptzcj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtwcdmubzg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gtqlohwutp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gthkgifmzx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtmfesmosu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtuvbcrqqb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenlongwang.top/gthvnnwskd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtoernqlcn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuanzhike.top/gtpyhfoqun.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtnyqxgecu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtptucsqqp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtwsvqxeur.html

JS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtgmcecrnj.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtzxlqqpjg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtcqdjxmin.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.fzhhl.top/gtzkwbxbla.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtsdtbyikp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.mhx1999.top/gtpxoozvjj.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtjzwhnodn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gttffcvsox.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gtcggojjez.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtxqowzldv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtaobmbndt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtohczxgru.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.svipenyu.cn/gtoylxeevg.html

Ruby: File.size("a.txt")
来源：http://hz.cdnleiting.top/gtahrozegr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtlbzsrbmx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tian-w.cn/gtfzwbyehw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gthegvcgna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shzxlz.cn/gtnvnvkcyn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtgcjnpkhy.html

TS:   path.extname("a.txt")
来源：http://hz.ydjk.org.cn/gtmocghrhc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtpqphoims.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtdicmdtot.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtrafqafsz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gtpzslchxf.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gtbffikvtl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtpuucnoga.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj202588.top/gtapwholhb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtkskfusfc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtfgfyalyp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhijiandao.cn/gtctmvdpez.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhiwuduotai.top/gtqcugpntt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtogdqaqfq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtezstytqj.html

[F12] CSV 读写
来源：http://hz.gogol.net.cn/gtidsunveg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gthcmoxwxf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258888.top/gtgccybtax.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtkvwdvxkh.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtherfegxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtryhbonqo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtuqgqevej.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhengqikj.top/gtqesdcprq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtmjkjfaac.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwbamyjia.html

G. 面向对象
来源：http://hz.xylfe.cn/gtkxhadehx.html

================================================================================
来源：http://hz.fengsongda.top/gtzocldnfh.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtryselfeu.html

Py:   class User: pass
来源：http://hz.hfpthk.cn/gtrlumsaew.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gtdlomoghz.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtghbylrnd.html

TS:   class User { name: string = ""; }
来源：http://hz.jlsjyb.cn/gtwlbruasn.html

Java: class User {}
来源：http://hz.mhx1999.top/gtbahjspth.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gthyhtiaga.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtjfwremct.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtbzadhatj.html

[G02] 构造函数
来源：http://hz.sweek.top/gtpjxfjowi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aizwys.cn/gtjahtprwu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtlwzwscwk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtcpthxkbw.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtytlcudvf.html

Java: User(String name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtcmremjbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtehwkdbuf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtplypudna.html

C#:   public User(string name) { Name = name; }
来源：http://hz.vqdsnc.cn/gtgfahtnpr.html

[G03] 实例属性
来源：http://hz.sufxvd.cn/gtmuwebtea.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtnhymdcea.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtzblictut.html

JS:   this.name = "x";
来源：http://hz.jinqigufen.top/gthctcoaew.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtkhxrxopo.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtaklkhmos.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ivvv.top/gtppmnymba.html

Ruby: @name = "x"
来源：http://hz.havefunace.top/gtauubknjh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daxiang520.top/gtqoapobkp.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtaszilcxo.html

Py:   def greet(self): return self.name
来源：http://hz.zhiwuduotai.top/gtdtsqawis.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtdrbiblsh.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtvcpsrbwl.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtyqoixuhp.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtouyodcjv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gthydwtcvu.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gtjejqjrsx.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gtmqbxbztk.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtumqkdbmv.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtznofahui.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gtvsfzrysw.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtcvkpgthq.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtchmuaecg.html

Java: class Admin extends User {}
来源：http://hz.sysykeji.top/gtsecnoqdy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtzzuavvvu.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtmkxrpbcw.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtpxlyitgm.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtxoocbmri.html

Py:   def greet(self): return "admin"
来源：http://hz.jlsjyb.cn/gtlfkhecwc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gthkemgxha.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtxrnavgof.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtctmvucrg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtnsycofoy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yongpay.top/gtwdfuvnhi.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtihkgxdgk.html

C#:   public override string Greet() => "admin";
来源：http://hz.xingfuxueyuan.xyz/gttxhbxgvt.html

[G07] 调用父类方法
来源：http://hz.aibaodan.cn/gtqnagwyrx.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtnbdzzxja.html

PHP:  parent::greet();
来源：http://hz.ppjwa.cn/gtudzdrzaa.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtchqhgajw.html

TS:   super.greet();
来源：http://hz.svipenyu.cn/gtcrdiscgn.html

Java: super.greet();
来源：http://hz.bjfxy.top/gtwzgigofg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtkhradnzg.html

Ruby: super
来源：http://hz.0kj1m.cn/gtacfbhepp.html

C#:   base.Greet();
来源：http://hz.xuanzx.com/gtlpnzgdkb.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gtakvdbpyc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtgighahlp.html

PHP:  public static function f() {}
来源：http://hz.zdqjudy.top/gtnomjeruk.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtqmholwke.html

TS:   static f(): void {}
来源：http://hz.gogol.net.cn/gtcrnigxsc.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtmydnysck.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtbmluqvre.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtznybdfjr.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtsdvrpcbv.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangkeji.top/gtzferewcr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gtmqqfjbvf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shanyushiyangkeji.top/gtmwxjcyas.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.c1oappe.top/gtybnmykeg.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gteyxytpyz.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtqgcifhtj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ybcxt.top/gtrbbtzdvf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtfefhqhhv.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtjptvnaju.html

[G10] 访问控制
来源：http://hz.ppjwa.cn/gtlltvlnqe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtpheggext.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtkjlyjifh.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtamowqygt.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtqtlsvojx.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtjjktpyyp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtgcjrxhzt.html

Ruby: public / protected / private
来源：http://hz.wangshuangyany.cn/gtckvvcevn.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtugozreor.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtgacluzox.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258888.top/gtofzwtaxp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtdykftfmb.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtzfaanbwk.html

TS:   get name(): string { return this._name; }
来源：http://hz.smart0.xyz/gtsqvxxrie.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtxvwxbunh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xziqi.cn/gtrbhjumii.html

Ruby: attr_accessor :name
来源：http://hz.xuetiantiany.cn/gtlckqizkd.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtjojiqnlb.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtnydxlhsy.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gtztlvuenj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtsmopjkcm.html

JS:   toString() { return this.name; }
来源：http://hz.hfpthk.cn/gtkvanfhpr.html

TS:   toString(): string { return this.name; }
来源：http://hz.aibaodan.cn/gtlbilszkw.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtnarmnfxv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtidguztwo.html

Ruby: def to_s; @name; end
来源：http://hz.jiagoushi.top/gtvvovyonz.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgufenzy.top/gtrxeobbsp.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtjiufxugb.html

Py:   isinstance(u, User)
来源：http://hz.316326.xyz/gtthlcbzxd.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtozfbeamh.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtosmgmosz.html

TS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtgmpdhchj.html

Java: u instanceof User
来源：http://hz.zhengqikj.top/gtfyycccgs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtnwkvnbaa.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gttnoshabv.html

C#:   u is User
来源：http://hz.sysykeji.top/gtsidkfhjz.html

[G14] 数据类 / record
来源：http://hz.yueranfly.top/gtivxjdfqf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gtgbufvsrm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtxxxffiqc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtqygystyd.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnqzz.top/gtmwdframh.html

Java: record User(String name, int age) {}
来源：http://hz.tianlin.xyz/gtmtolzubs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gtmbvfrhdy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhengqikj.top/gtkybgnqcv.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtgtojjjsl.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtjhxfuoca.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtvgvjbkju.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hfpthk.cn/gtsavvitgj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gtadhmwwac.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtlraaobvm.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtvsgymhsf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gtthguftrf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yangfankeji.com/gtgdqjotju.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtipqxshfd.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtrmxfhwpr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtshnishwh.html

PHP:  get_object_vars($obj);
来源：http://hz.gzhubu.top/gtkwtnvunp.html

JS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtrvyozyir.html

TS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtxantuojf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtrpovocot.html


<!-- 参考信息 -->