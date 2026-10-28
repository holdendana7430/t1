代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtjwmiaqev.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhoulong.xyz/gtapewapaw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenlongwang.top/gtfensronf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.snrcjt.cn/gtdvxlmggf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhijiandao.cn/gtetzbpytt.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtztgumbic.html

Py:   s.splitlines()
来源：http://hz.zhongyouzk.top/gtuerujbul.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtsfgjgdfe.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtwytccleu.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangdashe.top/gtuxpmlzzf.html

Java: s.lines().toList()
来源：http://hz.pycfn.com/gtbatvifry.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gtcvfppoiw.html

Ruby: s.lines
来源：http://hz.ivvv.top/gtcokgcgub.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtgqrwdofv.html

[E20] 判断字符串是否为空
来源：http://hz.hfpthk.cn/gtrxvuxxst.html

Py:   if not s:
来源：http://hz.aibaodan.cn/gtxmsetalm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtnkxdphtk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cashguo.top/gtbcfauqcg.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtxxmcqjhu.html

Java: if (s.isEmpty()) {}
来源：http://hz.ybcxt.top/gtikjwndbz.html

Go:   if s == "" {}
来源：http://hz.quarkkingdee.top/gtxzrkqniv.html

Ruby: if s.empty?
来源：http://hz.kuanghao11.cn/gtqigrpfiv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gtycsahliu.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtzpatvghp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtlldrkinx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtakhwkrdt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtdaxcmokv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtezocwarv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtthsrnqfm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.quarkkingdee.top/gttvsramnp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guowangkeji.top/gtqvgcjmbr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sxryk.cn/gtccgoswkf.html

[E22] 字节长度与字符长度
来源：http://hz.jinqigfzy.top/gtesxrxyis.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhengqikj.top/gtiuvsemmw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtoccejadn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtiiyeedyy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gttychmntc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.9152youxi.cn/gtifyzsqfk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gtbqylynli.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtamymnufg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.daxiang520.top/gtgsnetpja.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjsuyipmh.html

F. 文件与目录
来源：http://hz.fzhhl.top/gttazbzczc.html

================================================================================
来源：http://hz.sxryk.cn/gtndbtueou.html

[F01] 读取整个文件
来源：http://hz.wangdashe.top/gtjsjkyerk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangshuangyany.cn/gtdilacvza.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gthoiwqjur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtrceepskh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtrmofdvzv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtypwbzbsk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.iojbl.cn/gttrgbcsmn.html

Ruby: File.read("a.txt")
来源：http://hz.haohaochexian.top/gtquuzwwgm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.snrcjt.cn/gtwnnytdtr.html

[F02] 逐行读取文件
来源：http://hz.fengsongda.top/gtzgmxdoct.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenzaomai.com/gtyuyrirvy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtkrliezng.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtakislmmd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtqnwgofda.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtnvriocob.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yuxming.cn/gtuhfmlejf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hysaishi.cn/gtmafsnpre.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sufxvd.cn/gtvwbnqqpe.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigufen.top/gtcwdwezpe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258.top/gtuprfgast.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gtfadhaheh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtjoszfjyn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtzvwobxkc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hysaishi.cn/gttytxwcve.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenlongwang.top/gtftgtwflq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pengpengdd.cyou/gthqueroyw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtaendqexz.html

[F04] 追加写入文件
来源：http://hz.xuetiantiany.cn/gtxzoewgwk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hywenlv.cn/gtxvmcjifk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhengqikj.top/gttqnflnwe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtquzzwodj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtggssfukh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.haohaochexian.top/gtslymjhxv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtzmombgoy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtnxutsiae.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtzvvmnmui.html

[F05] 判断文件或目录是否存在
来源：http://hz.316326.xyz/gthwwwlfyx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.c1oappe.top/gthksmtufs.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtnaczcrhp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtficmqvwo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtuqzpzhzo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtmxcjqmig.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtpszrxqtn.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnxiangtu.top/gtwtzclodt.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtpuercnfj.html

[F06] 删除文件
来源：http://hz.andypj.xyz/gtgiuhsflm.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gthfkxtbmv.html

PHP:  unlink("a.txt");
来源：http://hz.hysaishi.cn/gtkrlmzwav.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtnyxkohbn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtmzotpgjb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtiroeebic.html

Go:   os.Remove("a.txt")
来源：http://hz.jianghu66.top/gtytgdtkvl.html

Ruby: File.delete("a.txt")
来源：http://hz.xuetiantiany.cn/gtpztgjogy.html

C#:   File.Delete("a.txt");
来源：http://hz.wangdashe.top/gtrnolhhzm.html

[F07] 创建目录（含多级）
来源：http://hz.zhijiandao.cn/gtorudkvvc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtqgayauli.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenzaomai.com/gtaorcueay.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtbglacoxl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtbndkzyys.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtjawyotyc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cdnleiting.top/gttvbttjxg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gtxjlooorf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.52xcode.cn/gtvkyfakgv.html

[F08] 遍历目录
来源：http://hz.aizwys.cn/gtvrjiaogl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangdashe.top/gtoixibpev.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtbaprlwhl.html

JS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtyqdbxaok.html

TS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtmpwwhebp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtfrqgwkjw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jqgufenzy.top/gtiskaeufk.html

Ruby: Dir.children("dir")
来源：http://hz.redwolf501.top/gtuljuxhbp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shuidangran.top/gtykerjinv.html

[F09] 获取文件大小
来源：http://hz.cdnleiting.top/gtvntfhglc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxinkj.top/gtznqvizar.html

PHP:  filesize("a.txt");
来源：http://hz.chenjidiqi.icu/gtclusyufc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenlongwang.top/gtngfljeue.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtqjxqcrgx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtpfqimgmk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtlgebhuru.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtkusyqjyo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtpulzwmyy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtmuancaob.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtasuwinxu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dashuyun.cn/gtqesyeugm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtyhtsvqhn.html

TS:   path.extname("a.txt")
来源：http://hz.xylfe.cn/gtoqtolcms.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aizwys.cn/gtyyigecqp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtcpptnvxu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtnbynicdl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gtwjbcxvfq.html

[F11] 复制与移动文件
来源：http://hz.jianghu66.top/gtgwcomiuj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtwicnprcz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhengqikj.top/gtrrrbeqwf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtmwknxtdk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtphqfrftn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangdashe.top/gtmfbrirrf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jlsjyb.cn/gtgwmvjftr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtmpqcsfcc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shanyushiyangkeji.top/gtljrcskhu.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gtkcbxyyti.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtllotvoih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gtezdkcebm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtnueoqvxt.html

TS:   // 同上
来源：http://hz.aibaodan.cn/gtzlfxydmz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gtfzvnhcsc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangshuangyany.cn/gtvwjwxjku.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.meibo888.top/gtgermtsxd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gtnopiradv.html

================================================================================
来源：http://hz.snrcjt.cn/gtigcfoyre.html

G. 面向对象
来源：http://hz.xuanzx.com/gtqimecnbs.html

================================================================================
来源：http://hz.jinqigufen.top/gtzfoarlef.html

[G01] 定义类
来源：http://hz.yueranfly.top/gtqtrjvccs.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtldahcnyu.html

PHP:  class User {}
来源：http://hz.aibaodan.cn/gtqhpjzpfd.html

JS:   class User {}
来源：http://hz.shuidangran.top/gttqpcwfnk.html

TS:   class User { name: string = ""; }
来源：http://hz.meibo888.top/gtgepwncti.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtwuqzpfrp.html

Go:   type User struct { Name string }
来源：http://hz.cucudq.cn/gtrodyykep.html

Ruby: class User; end
来源：http://hz.fzhhl.top/gtdtdxroyi.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtdnrskzny.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtzrynfsci.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.bjfxy.top/gtthbipiga.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fzhhl.top/gtlmzalvfb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtktnhyvpb.html

TS:   constructor(public name: string) {}
来源：http://hz.hongshengwenyu.top/gtdcbiwnvl.html

Java: User(String name) { this.name = name; }
来源：http://hz.c1oappe.top/gtqpblcdfn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gtnnhwgwfp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtzvajjutj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtdkxvtjlr.html

[G03] 实例属性
来源：http://hz.hysaishi.cn/gtiuukjuwk.html

Py:   self.name = "x"
来源：http://hz.yuxming.cn/gtenoyirgv.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gtgqesrdgv.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtdhnclyhz.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gthcwmbdfx.html

Java: private String name;
来源：http://hz.c1oappe.top/gtwolitsgc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zycfv.cn/gtdkkvhwuv.html

Ruby: @name = "x"
来源：http://hz.gzhubu.top/gthcacodez.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtpigeyhen.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtedueddxm.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtpdowkajb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtvjvoqxsy.html

JS:   greet() { return this.name; }
来源：http://hz.hongshengwenyu.top/gttsumdfqf.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtluvjxgdi.html

Java: String greet() { return name; }
来源：http://hz.guannengcc.top/gtkevlqona.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtosfflrwa.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gttjofiqxf.html

C#:   public string Greet() => Name;
来源：http://hz.fzhhl.top/gtyuhgxtbr.html

[G05] 继承
来源：http://hz.daxiang520.top/gtrvxrkklp.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtlrgwuipw.html

PHP:  class Admin extends User {}
来源：http://hz.hnqzz.top/gtzxyvsgtu.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtjnlzkvbe.html

TS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtqheksqym.html

Java: class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtzlpddjeb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtrwgkluaq.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtiaqqrklu.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gtugolpejs.html

[G06] 重写方法
来源：http://hz.cheryme.top/gteofrasfv.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtysogprkf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtfythqbic.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtltnkzpfm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtsixbpyvr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gtwfxfjcne.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgufenzy.top/gtkyjwlhlg.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtpcydzham.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtzvkwvxpv.html

[G07] 调用父类方法
来源：http://hz.ivvv.top/gtfaynpekk.html

Py:   super().greet()
来源：http://hz.svipenyu.cn/gteyzhanhd.html

PHP:  parent::greet();
来源：http://hz.jiagoushi.top/gtbzhwjtwz.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtxrxtnssr.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtgdzxzgdx.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtjablyytp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tian-w.cn/gtynnsixal.html

Ruby: super
来源：http://hz.xinyue.icu/gtqfcqzqwr.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gthljmuzaz.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtxnyfzgnv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ybcxt.top/gtrsnyjfhj.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtfbaonbze.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gthqbgkpht.html

TS:   static f(): void {}
来源：http://hz.zhixingplan.top/gtewcqqwdu.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtxzyhrahv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258888.top/gtzarjgqka.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gtrrzvrxxx.html

C#:   public static void F() {}
来源：http://hz.chenzaomai.com/gtfeogmxxf.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtmsigymrd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhongyouzk.top/gtrsdmoukk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtzkgpstfi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangkeji.top/gtoaffudwi.html

TS:   interface Shape { area(): number; }
来源：http://hz.smart0.xyz/gtojzfxmtk.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtjkvlaqth.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydzc1.top/gtmesznqtf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtacfoimfr.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnxiangtu.top/gtxnaftqyv.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtzfaaaqoq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtmoirbbmy.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gtaeayarrg.html

JS:   #private 字段；其余公开
来源：http://hz.zhiwuduotai.top/gtzpmsomtr.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtkclvwyku.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtwnrcurnn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtczznjpxj.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtiscfpfpw.html

C#:   public / protected / private / internal
来源：http://hz.chenzaomai.com/gtfbtfdaee.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtjrzftvxs.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gtyxsaboxs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gttrgepyri.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gtikalhyyg.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtdoayckoi.html

Java: public String getName() { return name; }
来源：http://hz.yvedp.cn/gtqzumjpuz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtiuvtbvld.html

Ruby: attr_accessor :name
来源：http://hz.cashguo.top/gtkktplmrv.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtwdozvpwo.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gttrfrzcqs.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtpmbxznda.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtloobsssr.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gtbczmbifd.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtiigzueda.html

Java: @Override public String toString() { return name; }
来源：http://hz.dianchejie.cn/gtpptnxeun.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dashuyun.cn/gtashphdpo.html

Ruby: def to_s; @name; end
来源：http://hz.hnxiangtu.top/gtmntpzzfx.html

C#:   public override string ToString() => Name;
来源：http://hz.vqdsnc.cn/gtwionxokt.html

[G13] 判断对象类型
来源：http://hz.jianghu66.top/gtteawkqcc.html

Py:   isinstance(u, User)
来源：http://hz.kuanghao11.cn/gtdwwgfcow.html

PHP:  $u instanceof User
来源：http://hz.jinqigufen.top/gtqjeqedva.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtzovrbcfa.html

TS:   u instanceof User
来源：http://hz.xylfe.cn/gtkefbfxaf.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gttjmksgrl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.bjfxy.top/gtgiegbtyl.html

Ruby: u.is_a?(User)
来源：http://hz.shanyushiyangkeji.top/gteuxsoufq.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtboaldihi.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtvoajimrb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtmquguevp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenlongwang.top/gtnrvsykhd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gtszzhbyze.html

TS:   type User = { name: string; age: number };
来源：http://hz.yongpay.top/gtpelatpsd.html

Java: record User(String name, int age) {}
来源：http://hz.yj202588.top/gttzevobxe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nwbrower.top/gttgurojvv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtpvcdjduf.html

C#:   record User(string Name, int Age);
来源：http://hz.52xcode.cn/gtubwdmkug.html

[G15] 枚举
来源：http://hz.birdmap.top/gtcjsjetjb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sysykeji.top/gttnhwrrje.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuanzx.com/gttdsnqzxk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daria6918.cn/gtrhgbhxgs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtwghtvsoc.html

Java: enum Color { RED, GREEN }
来源：http://hz.gogol.net.cn/gthdcilqmd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.daxiang520.top/gtpqxvhopy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hongshengwenyu.top/gtazrwovym.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtctdetcrn.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtqyblxbaz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtratzjjtv.html

PHP:  get_object_vars($obj);
来源：http://hz.smart0.xyz/gtirxibinw.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtgedkbqsj.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtqrtntldu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtfiovfhgr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtbscrwniu.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtevpbqgcf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtvqhwykkc.html

================================================================================
来源：http://hz.jinqigfzy.top/gttmvbttef.html


<!-- 参考信息 -->