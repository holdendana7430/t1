代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhoulong.xyz/gtmdvajkrh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sxryk.cn/gtgehyyguu.html

Ruby: s.capitalize
来源：http://hz.jinqigufen.top/gtejzyzvgf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtkvcavsww.html

[E18] 模板占位符替换
来源：http://hz.zhaomingkeji.xyz/gtrdhakvyn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yangfankeji.com/gtmufyyuhz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daxiang520.top/gtomjsatsm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtamkrathu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtopzwdkxh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuanzx.com/gtdavsgdpq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.feifeiyinyue.top/gtjgsfugxw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxinkj.top/gtjhfkbket.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tanke756.top/gtooapuvsw.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtmogucjfd.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtvuhmskwb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtcbfaozpz.html

JS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtnxzbjzaa.html

TS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtqbervjta.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtlsybqknq.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gtiaequyet.html

Ruby: s.lines
来源：http://hz.shanyushiyangkeji.top/gtkfsfjnlf.html

C#:   s.Split('\n')
来源：http://hz.andypj.xyz/gtzuiqrzmb.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtzysqwoev.html

Py:   if not s:
来源：http://hz.yanxiufei.cn/gtxhvgdfhl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aibaodan.cn/gtxudzcjqc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gotoacloud.top/gtpwbmapqw.html

TS:   if (s === "") {}
来源：http://hz.chenzaomai.com/gtrqhytzea.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtqlzplwlo.html

Go:   if s == "" {}
来源：http://hz.daxiang520.top/gtbznxbnaa.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtysqdkunj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtfbugeujq.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtgoqqmlgr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtnarlmpbg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.feifeiyinyue.top/gtqiwtrkqb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gttslajmpr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtzwkyldmb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtvszgwome.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtareguath.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.meibo888.top/gtsxyuvsyr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.bjfxy.top/gtbfzftjmm.html

[E22] 字节长度与字符长度
来源：http://hz.chenzaomai.com/gtmoshlwlx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhongyouzk.top/gtdhocckzj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtxoyxbapo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtprscweoa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtptcaopfd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.redwolf501.top/gtetyjirya.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gogol.net.cn/gtyrkdnfig.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gtzgfmqfsn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ydjk.org.cn/gtwtslypqk.html

================================================================================
来源：http://hz.aizwys.cn/gtlqtjgofn.html

F. 文件与目录
来源：http://hz.ybcxt.top/gtyyhcppii.html

================================================================================
来源：http://hz.birdmap.top/gtwbjfgdbn.html

[F01] 读取整个文件
来源：http://hz.316326.xyz/gtsaetqfli.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtxtjhythd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtftpomzph.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ehwqpu.com/gtnqtjsroa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258888.top/gtndhjveyp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtfnogiupc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtrxlpphpo.html

Ruby: File.read("a.txt")
来源：http://hz.zhengqikj.top/gtxcjwslab.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.9152youxi.cn/gtwbaldbbi.html

[F02] 逐行读取文件
来源：http://hz.haohaochexian.top/gtayjrjson.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.birdmap.top/gteitztjwg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zycfv.cn/gtlesiqzbv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtvspvuzki.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtsbikipbn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtcyxjfdad.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinghuilouyu.cn/gtpaorrxof.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigufen.top/gtsxxwmhxi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shangyingyoupin.top/gtxkjnnyea.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtfuzpnzrv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenzaomai.com/gtpormktrw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gttjbtzvrq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yueranfly.top/gtemueirfn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gteqsahfvw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gtwfnwnqra.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jlsjyb.cn/gtzivruyqq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtfzpnznos.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.andypj.xyz/gtuqlhsdkh.html

[F04] 追加写入文件
来源：http://hz.xingfuxueyuan.xyz/gtfnazvlcw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yvedp.cn/gtjisiyeur.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhengqikj.top/gtmynkldrz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fengsongda.top/gtmzsfpqjc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gthfmnrsiy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtsbkvwhkm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangtech.top/gtyqeshfoq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtjozcxgov.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gtsniwpoox.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtkeefykhr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xingfuxueyuan.xyz/gtkuumjioa.html

PHP:  file_exists("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtvqwakctu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtbkutonfp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtpbfqdifo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gthgaecews.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tanke756.top/gtyiihhrsw.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuxming.cn/gtxxvhmkib.html

C#:   File.Exists("a.txt")
来源：http://hz.jianghu66.top/gtzyplhwir.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtbypfzvyz.html

Py:   os.remove("a.txt")
来源：http://hz.tianlin.xyz/gtneojtrod.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gtfhzlcvjl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtwuzcwuic.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtjquqsgpw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtpvglxuxf.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxtlbgups.html

Ruby: File.delete("a.txt")
来源：http://hz.cheryme.top/gtnpwapxtw.html

C#:   File.Delete("a.txt");
来源：http://hz.gzhubu.top/gtiasfleha.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtqwstqcrn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daxiang520.top/gtdgmnngxf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtsheekuvm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtcqzzyxqa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtnhyulbno.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fzhhl.top/gtgwywadbo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtcxkpghwk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtvvtrjudx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenlongwang.top/gtshlfzhiw.html

[F08] 遍历目录
来源：http://hz.bjfxy.top/gtbdtpxykj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hfpthk.cn/gtuahorblw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shanyushiyangkeji.top/gtxtznfbjg.html

JS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtzdwlpzkz.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtpbelbsag.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtcfnnuvec.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gtxcwgalpf.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtaimsylbp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtzeikffyv.html

[F09] 获取文件大小
来源：http://hz.aizwys.cn/gtmzezeazw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtqdfgngsc.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtfaasyvll.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtgtxxdmuw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtnbehzapc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtwqyleens.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgfzy.top/gtvhdhhqkk.html

Ruby: File.size("a.txt")
来源：http://hz.ppjwa.cn/gtuursxaqj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.dashuyun.cn/gtcjxzdqib.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.smart0.xyz/gtzhmrtgxb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtvlwrkhjz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangkeji.top/gtlnfxrazh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtdribmvvi.html

TS:   path.extname("a.txt")
来源：http://hz.shangyingyoupin.top/gtyitybkgd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gtrrvgntpx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.birdmap.top/gtoqrtkjxj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtzavkygvh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tianlin.xyz/gtbqeyfjqu.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtjnstqbup.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtzcpnkxdp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.meibo888.top/gtztsdsotr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtfbsymzsq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtdamfaspy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.haohaochexian.top/gtwtljqczv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gtgogajevp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gttaxpjbpi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.snrcjt.cn/gtqueakshx.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtcuqfikpe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sweek.top/gtyutjioqx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgfzy.top/gtppclnvyw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtwmdorfnr.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtdaxqteij.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinyuanbaomall.cn/gtoaqzpmeg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xingfuxueyuan.xyz/gtcrsgxpox.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gogol.net.cn/gtqxnmoweg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hysaishi.cn/gtkccwnnes.html

================================================================================
来源：http://hz.jqgfzy.top/gtywmrorta.html

G. 面向对象
来源：http://hz.iojbl.cn/gtdzrhluhy.html

================================================================================
来源：http://hz.316326.xyz/gtveaafoco.html

[G01] 定义类
来源：http://hz.zycfv.cn/gthmurjgkj.html

Py:   class User: pass
来源：http://hz.aizwys.cn/gtmoaibfnp.html

PHP:  class User {}
来源：http://hz.gaohongyu789.top/gttrynumrv.html

JS:   class User {}
来源：http://hz.nanxuanxn.top/gtixdpazxx.html

TS:   class User { name: string = ""; }
来源：http://hz.daria6918.cn/gtlpgipalj.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtgnfzkxfy.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gtuylubhee.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtogcjxytx.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gtougtorqn.html

[G02] 构造函数
来源：http://hz.ivvv.top/gtewoathic.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zycfv.cn/gtmjgpoluj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtwlomvnkk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtvyfbnctn.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtewfgmvre.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtubfojvco.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yvedp.cn/gtvfpucsdd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gtbwdpkkyi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangdashe.top/gtbglcsibg.html

[G03] 实例属性
来源：http://hz.meibo888.top/gtrrrovguj.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtwpzfediw.html

PHP:  public string $name = "x";
来源：http://hz.nwbrower.top/gtixoqqnav.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtcduhdgbp.html

TS:   name: string = "x";
来源：http://hz.guowangkeji.top/gtjvvxzvoa.html

Java: private String name;
来源：http://hz.jinghuilouyu.cn/gtmlldrugm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtyzupyttl.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtcecgkhzy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtfeoukyol.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtmuubsiim.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtfvfqneej.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtgjmhiuij.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtxmpranuc.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtrtwjddza.html

Java: String greet() { return name; }
来源：http://hz.zhongyouzk.top/gtfswchsfe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtxdjmjhjj.html

Ruby: def greet; @name; end
来源：http://hz.xuetiantiany.cn/gtbqlcbmia.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gthprwcyxd.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtugogaqqm.html

Py:   class Admin(User): pass
来源：http://hz.xylfe.cn/gtardpnrhl.html

PHP:  class Admin extends User {}
来源：http://hz.xziqi.cn/gtxriajazj.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtsizeggfi.html

TS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gthiuwczhm.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtrnmhfxvu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxuanxn.top/gtdfdznmjv.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtrnacrneb.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gtkrmdycak.html

[G06] 重写方法
来源：http://hz.shanyushiyangtech.top/gtwcpvdowf.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gtsijjfora.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtvhmsyftk.html

JS:   greet() { return "admin"; }
来源：http://hz.svipenyu.cn/gtzfgbvypm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtcslcwyyr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtmpyoctln.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtnengehxs.html

Ruby: def greet; "admin"; end
来源：http://hz.chenzaomai.com/gtvwhiesjz.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtbvpxwbxw.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtgsvkpaxy.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtuqkvndij.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtnuxbovzu.html

JS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtjnkryzbl.html

TS:   super.greet();
来源：http://hz.snrcjt.cn/gtqwmnrzvn.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtopdbolmk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zdqjudy.top/gthzqylodb.html

Ruby: super
来源：http://hz.daxiang520.top/gtevjwzgxn.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtxfcctwru.html

[G08] 静态方法与属性
来源：http://hz.jinqigufen.top/gtjiogekvr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtsmqagnxh.html

PHP:  public static function f() {}
来源：http://hz.gzhubu.top/gttdupnqcz.html

JS:   static f() {}
来源：http://hz.fzhhl.top/gtxvwxmqpe.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtagfcuniq.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtruswxydg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtqjjrvhhd.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtrrgpkcls.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtqhwsybju.html

[G09] 接口 / 抽象类
来源：http://hz.guannengcc.top/gtqqakhuho.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtmwidqvyc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtntoelgon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sxryk.cn/gtxmkakonr.html

TS:   interface Shape { area(): number; }
来源：http://hz.guowangkeji.top/gtbyulawec.html

Java: interface Shape { double area(); }
来源：http://hz.cqqwz.cn/gtnaxjdhfe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydzc1.top/gtihyihvkm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenjidiqi.icu/gttvilimvf.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gtndwpdqdz.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtnqeluabs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pengpengdd.cyou/gtppvndrof.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtpjhhzyui.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtpiendkrc.html

TS:   public / protected / private
来源：http://hz.jyoumei.cn/gtvodwuozc.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtzgbfpgtz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuanzx.com/gtdppnacwk.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gthcukzake.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtbriuujja.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gtxhbsxvsl.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtiylkkhga.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtmqlquvuv.html

JS:   get name() { return this._name; }
来源：http://hz.hywenlv.cn/gtqctpgrid.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gthawnopuh.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gtwylqmbws.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.mhx1999.top/gtxujhbepq.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gtsszklydh.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtmmzydelb.html

[G12] 对象转字符串
来源：http://hz.guowangkeji.top/gtvkakbmkx.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258.top/gtkavpptgv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtzavcuxuv.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtkiqdxoal.html

TS:   toString(): string { return this.name; }
来源：http://hz.c1oappe.top/gtlnhdjfyq.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtukyayros.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenlongwang.top/gtxxkuudzl.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gtsvakefoh.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtxitgqjil.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtammlsohu.html

Py:   isinstance(u, User)
来源：http://hz.dashuyun.cn/gtmjazulth.html

PHP:  $u instanceof User
来源：http://hz.hnqzz.top/gtuqjxmpov.html

JS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gttnxeqwfp.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtkzysvqzw.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtuxpkweqe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yvedp.cn/gtgohyqkie.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtvmlagqly.html

C#:   u is User
来源：http://hz.ivvv.top/gtvyeufmzt.html

[G14] 数据类 / record
来源：http://hz.zhixingplan.top/gtgjsainim.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tian-w.cn/gtknjbmqte.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtmpsmxahs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gogol.net.cn/gtahrxxqwd.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigfzy.top/gthdogbxtu.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gtvgzulrhp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gtwttaegns.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jlsjyb.cn/gtkhwiwigv.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gttftpiaco.html

[G15] 枚举
来源：http://hz.pycfn.com/gtipicntjq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gtjmucxryg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258888.top/gtantfcugt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sysykeji.top/gteqlvcamr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gthromjmby.html

Java: enum Color { RED, GREEN }
来源：http://hz.hysaishi.cn/gtycpfqowz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hongshengwenyu.top/gtcogltjgb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.svipenyu.cn/gtucpokudk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtlkzbuzdh.html

[G16] 对象转数组 / 字典
来源：http://hz.9152youxi.cn/gtiaysvngw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtvzncchan.html


<!-- 参考信息 -->