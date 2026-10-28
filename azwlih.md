代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhongyouzk.top/gtteryjelg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cdnleiting.top/gtvsajxirk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtkwxkrnht.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtydmxrtsb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hongshengwenyu.top/gtkomveglz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yueranfly.top/gtutxeymsa.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtfxjxvfio.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtvloshybt.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtzyqkwjyw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.bjfxy.top/gtasvhbqst.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hfpthk.cn/gtdttgrcrw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtbekyeoan.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cashguo.top/gttjsdizuu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhijiandao.cn/gteshgbddh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hammf.cn/gtosvbxole.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sysykeji.top/gtrkkffsed.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sufxvd.cn/gtwptvytar.html

[E19] 多行文本按行拆分
来源：http://hz.zdqjudy.top/gtxiqpwcxd.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtjklnqrnj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydzc1.top/gthodmzahd.html

JS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtvqmdcfcq.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtztswnmxj.html

Java: s.lines().toList()
来源：http://hz.gogol.net.cn/gtediiiaue.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtzslhfwfv.html

Ruby: s.lines
来源：http://hz.jianghu66.top/gtmdsucipg.html

C#:   s.Split('\n')
来源：http://hz.ydjk.org.cn/gtceoqztgz.html

[E20] 判断字符串是否为空
来源：http://hz.ppjwa.cn/gtbwnmrdza.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtrkzswdql.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gaohongyu789.top/gtdbbqujml.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.pycfn.com/gtbpsoammm.html

TS:   if (s === "") {}
来源：http://hz.jyoumei.cn/gtvhaalrmx.html

Java: if (s.isEmpty()) {}
来源：http://hz.hammf.cn/gtbqhsajji.html

Go:   if s == "" {}
来源：http://hz.ydjk.org.cn/gtodegjriz.html

Ruby: if s.empty?
来源：http://hz.cashguo.top/gttgfuodfz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yongpay.top/gtrfonlefn.html

[E21] 超长截断加省略号
来源：http://hz.gaohongyu789.top/gtrfdtujyi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shzxlz.cn/gtxfrgatri.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.svipenyu.cn/gtwvaymgcz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtyiwlcwyk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtpnazsgle.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtvbaqszkn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhoulong.xyz/gtorrnemea.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zdqjudy.top/gtfswqzonr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yanxiufei.cn/gtqlduvkbx.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangkeji.top/gtixjkinoj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.52xcode.cn/gtkspvdfna.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydjk.org.cn/gthdgadyzj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtotypjlci.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtkonqirge.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ivvv.top/gtwygrkcza.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nwbrower.top/gtjzhpwhkw.html

Ruby: s.bytesize;  s.length
来源：http://hz.xuetiantiany.cn/gtiudwbqyy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pycfn.com/gtuyjzgrxy.html

================================================================================
来源：http://hz.52xcode.cn/gtjxxzqade.html

F. 文件与目录
来源：http://hz.cheryme.top/gtzegivkfr.html

================================================================================
来源：http://hz.ivvv.top/gtvjconqyd.html

[F01] 读取整个文件
来源：http://hz.meibo888.top/gtfyebbdbz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258888.top/gtovaiyubh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.9152youxi.cn/gtalivhlut.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gttqciqizd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tanke756.top/gtkustnghf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtubtwpuch.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtazcmmlba.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtccglhqun.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yangfankeji.com/gtvuytegef.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gtiwuqqwng.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hfpthk.cn/gtppsulwch.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhijiandao.cn/gtkthqvqwp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.kuanghao11.cn/gtchfrvyrb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.smart0.xyz/gtjadlpidq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gttvwphxqj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.quarkkingdee.top/gthxolwhwo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.aibaodan.cn/gtobspynrt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aibaodan.cn/gtsnlxyije.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258888.top/gtqsdwcuzq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yueranfly.top/gtobhhmplg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtmpisnpqq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtdzopftvk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gtatljfumu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtgfbozuvs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zdqjudy.top/gtwormtcnl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cdnleiting.top/gtsufzzvgi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtlippalge.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtleepfdpk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtipardfdv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yongpay.top/gtsovnozvk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtzebfkdym.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtfelpdmrg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuetiantiany.cn/gtwlftpgez.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtlrjqlgls.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtlfkbmjgf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ivvv.top/gtcoacqmbg.html

[F05] 判断文件或目录是否存在
来源：http://hz.tanke756.top/gtzhprfydf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nwbrower.top/gtkabwxstc.html

PHP:  file_exists("a.txt");
来源：http://hz.zhixingplan.top/gtnluhnhsp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fengsongda.top/gtxivckxyx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtpuzougor.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtsenjhmyw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shangyingyoupin.top/gtmaamywcc.html

Ruby: File.exist?("a.txt")
来源：http://hz.guowangkeji.top/gtrqkaqbja.html

C#:   File.Exists("a.txt")
来源：http://hz.dianchejie.cn/gtuvopquho.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gtfpxwyqng.html

Py:   os.remove("a.txt")
来源：http://hz.dashuyun.cn/gtwagmhbpb.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtjlxzlbwb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtgnsuqtfu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtrxhqymge.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtntwgpqlh.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtuevscsrp.html

Ruby: File.delete("a.txt")
来源：http://hz.jianghu66.top/gtoeexkdsm.html

C#:   File.Delete("a.txt");
来源：http://hz.meibo888.top/gtzvuepwle.html

[F07] 创建目录（含多级）
来源：http://hz.zdqjudy.top/gtffptbukx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtcgixvtxh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.quarkkingdee.top/gtdprahugo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtzwqzjvrh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtcymjcrvh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj202588.top/gturncppha.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ywan-chungtsiang.top/gtmgidpejb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yongpay.top/gtoctnmnij.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtxczktsjt.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtgunjwmrp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtjsybnfpw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtfhpemmbc.html

JS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtfsfwogjt.html

TS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtacnqxtqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtkpowruah.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtkleytqgc.html

Ruby: Dir.children("dir")
来源：http://hz.jianghu66.top/gtovcpyijz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pengpengdd.cyou/gtldfvhdhg.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtjidhkony.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtwewvvstb.html

PHP:  filesize("a.txt");
来源：http://hz.aibaodan.cn/gtgvyzracw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xylfe.cn/gtqzqpbqxx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtfzcjipvt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtqbofudkn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtdfxcufob.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gtgdnwafcb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shzxlz.cn/gtoqakeyio.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cucudq.cn/gtfovhxbxl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtbdqjnpjq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtuhzfjmdl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtqygrjlfh.html

TS:   path.extname("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtxwviybor.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gtkposdqhx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gtqfbaaclb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtufnhphop.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gtbnnrebeg.html

[F11] 复制与移动文件
来源：http://hz.cdnleiting.top/gtidrdklwo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtmzmoijsq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.havefunace.top/gtsmxqlhcn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtkqwnnesm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtzhdggvam.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtwzehrkms.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gotoacloud.top/gtcdnylecw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtnsuevpzd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtqaunyvjb.html

[F12] CSV 读写
来源：http://hz.bjfxy.top/gtreqxpccg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gtuwqsmweo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gttakxisel.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shuidangran.top/gtvuxumazp.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtbsslslwn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.9152youxi.cn/gtcdcaizxz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhongyouzk.top/gtblwlkuue.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtqmukpjju.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gtlcikfoal.html

================================================================================
来源：http://hz.ivvv.top/gtfvrtzrgn.html

G. 面向对象
来源：http://hz.havefunace.top/gtdipambwe.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsgpqhtmq.html

[G01] 定义类
来源：http://hz.yongpay.top/gtbtaldyyi.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtyprfurec.html

PHP:  class User {}
来源：http://hz.jinghuilouyu.cn/gtglykvmpk.html

JS:   class User {}
来源：http://hz.0kj1m.cn/gtudrstceo.html

TS:   class User { name: string = ""; }
来源：http://hz.cashguo.top/gtapjdjbah.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtpgxjixni.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtibvptfke.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gthbsyhywo.html

C#:   class User {}
来源：http://hz.yj20258888.top/gtnhgxklcr.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gttucrails.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.0kj1m.cn/gtpgarcssd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.kuanghao11.cn/gtqmnhdiok.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtlzbjbxnb.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gttthwgjzp.html

Java: User(String name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtqhuqeyjs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yvedp.cn/gtqtnsbeec.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtwcmhfdsx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daxiang520.top/gtvfztuudm.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtckqjdbjx.html

Py:   self.name = "x"
来源：http://hz.hysaishi.cn/gtylawbglu.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtrmnmjvpx.html

JS:   this.name = "x";
来源：http://hz.xylfe.cn/gtjgneghxu.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtidzjnfyu.html

Java: private String name;
来源：http://hz.sweek.top/gtifhktzoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtlfqjiwza.html

Ruby: @name = "x"
来源：http://hz.nanxinkj.top/gtjikwvtte.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtgrwaetjs.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtshjoogzj.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtrgwsoyll.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtfhzsxjlx.html

JS:   greet() { return this.name; }
来源：http://hz.guowangkeji.top/gtwrocmbol.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtfoievhtb.html

Java: String greet() { return name; }
来源：http://hz.sysykeji.top/gtgsfbfuna.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtgzsaayuq.html

Ruby: def greet; @name; end
来源：http://hz.ybcxt.top/gtfpiehcjq.html

C#:   public string Greet() => Name;
来源：http://hz.snrcjt.cn/gtlimqzcam.html

[G05] 继承
来源：http://hz.yonumen.top/gttlvwosig.html

Py:   class Admin(User): pass
来源：http://hz.andypj.xyz/gthueecxmu.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtywdgmnqy.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtphkedbtl.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtdbfigkrz.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtrigrnnqi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.bjfxy.top/gtuqlqyudr.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtcoexcwhu.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtjyeviahz.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gtvefcvdcc.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtqwvumhrv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtqfvrfpze.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtopkidgze.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtwyzvgejy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtfuryztkj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtdqrkcedb.html

Ruby: def greet; "admin"; end
来源：http://hz.tianlin.xyz/gtcywijmvp.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtwvnubsew.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtpsbdfsrm.html

Py:   super().greet()
来源：http://hz.jinqigufen.top/gtzcqzzscq.html

PHP:  parent::greet();
来源：http://hz.jinyuanbaomall.cn/gtswxtecsi.html

JS:   super.greet();
来源：http://hz.gogol.net.cn/gtcvqvemnq.html

TS:   super.greet();
来源：http://hz.fzhhl.top/gtfzilbfik.html

Java: super.greet();
来源：http://hz.andypj.xyz/gtnadxolip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shuidangran.top/gtpfswknbk.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtaxkoethc.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtiqfqzube.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtbeokpocs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.0kj1m.cn/gtzwppnchi.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtxzireqjn.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtvbdhwypn.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtqickgwch.html

Java: static void f() {}
来源：http://hz.ydjk.org.cn/gtusfqjawa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtgswznqnf.html

Ruby: def self.f; end
来源：http://hz.sufxvd.cn/gtefgoddez.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtcflhbbln.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtmcsvpuwe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenlongwang.top/gtqhkackiz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtosjgzypp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtujvrpwog.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtisuepiao.html

Java: interface Shape { double area(); }
来源：http://hz.jqgufenzy.top/gtsllatgio.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtnrbssnxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gaohongyu789.top/gtpuegllmk.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtbyzxjtme.html

[G10] 访问控制
来源：http://hz.hysaishi.cn/gtqdpjiwen.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cqqwz.cn/gtcavjdpwc.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtvkqzvjyl.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtvoadsufj.html

TS:   public / protected / private
来源：http://hz.hywenlv.cn/gtmiarossy.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtzsqsyhtz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtvcyhrazc.html

Ruby: public / protected / private
来源：http://hz.xziqi.cn/gtlhivgykr.html

C#:   public / protected / private / internal
来源：http://hz.wangshuangyany.cn/gtuiglomxr.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gtfhlsszzh.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtmshlxdfe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtnzvrkwmj.html

JS:   get name() { return this._name; }
来源：http://hz.meibo888.top/gtcepghwpn.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtbflsoulm.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtxasxvnwy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtxptbrmbg.html

Ruby: attr_accessor :name
来源：http://hz.hywenlv.cn/gthbksqbid.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtqlzhgfrm.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtoioexmft.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtssprccat.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtjnqoefhl.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gtdkozuhiy.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtsmdjeuqi.html

Java: @Override public String toString() { return name; }
来源：http://hz.snrcjt.cn/gtgsskvqqs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtptlyywdi.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtugybtitu.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gttermxptf.html

[G13] 判断对象类型
来源：http://hz.yanxiufei.cn/gtoavkltry.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtcialtpww.html

PHP:  $u instanceof User
来源：http://hz.9152youxi.cn/gtbjedcmla.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtwnyxsggp.html

TS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtaicsjrde.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gtyvrtgewy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtseilxbdf.html

Ruby: u.is_a?(User)
来源：http://hz.yonumen.top/gtokirbfvg.html

C#:   u is User
来源：http://hz.chenjidiqi.icu/gtlrbngpml.html

[G14] 数据类 / record
来源：http://hz.xinyue.icu/gtcrnvvrep.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yonumen.top/gtvjvvnywx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtpslfqoqf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtnntbmczk.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydzc1.top/gtojnvhpgu.html

Java: record User(String name, int age) {}
来源：http://hz.feifeiyinyue.top/gtzsqgwqnw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtrzvngoxh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtjahjwjoi.html

C#:   record User(string Name, int Age);
来源：http://hz.hfpthk.cn/gtifdaztmy.html

[G15] 枚举
来源：http://hz.hfpthk.cn/gtxshkwsjk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtrzsvfjpb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.316326.xyz/gtpftnjetg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hysaishi.cn/gtpybbxiun.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtsmhieafy.html

Java: enum Color { RED, GREEN }
来源：http://hz.birdmap.top/gtzmqxgilv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.svipenyu.cn/gtmuturigq.html


<!-- 参考信息 -->