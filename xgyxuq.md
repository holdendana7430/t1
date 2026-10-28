代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.dianchejie.cn/gtwgzfxsyg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtuxbhqulm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtqemomurl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.andypj.xyz/gtorwhapvi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ivvv.top/gtxmkwhnbu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pengpengdd.cyou/gtyjrxxfil.html

C#:   1234567.ToString("N0")
来源：http://hz.ivvv.top/gtopxjdgkc.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gtbidbxdho.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhoulong.xyz/gtyjprdlkm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hfpthk.cn/gteatypalb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtkvvuizox.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gttixialxw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gotoacloud.top/gtzxjamgay.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gtzzrwxdvs.html

Ruby: s.capitalize
来源：http://hz.guowangkeji.top/gtycsxhill.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gzhubu.top/gtymvnihsj.html

[E18] 模板占位符替换
来源：http://hz.chenjidiqi.icu/gtwanncqhg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.sysykeji.top/gtojgakfvd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xziqi.cn/gtouclmnqv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtjvenagug.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtbysplgsf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtlrzuvzqc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gaohongyu789.top/gtlakltbht.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuanzhike.top/gtxgbsbvxf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xuetiantiany.cn/gtmopbxcra.html

[E19] 多行文本按行拆分
来源：http://hz.yongpay.top/gtkioaunse.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtrnpenpnv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hongshengwenyu.top/gtsefpzwzy.html

JS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtqkqnvjjo.html

TS:   s.split(/\r?\n/)
来源：http://hz.shanyushiyangkeji.top/gtfcwoyvfr.html

Java: s.lines().toList()
来源：http://hz.zycfv.cn/gtwnnrrboe.html

Go:   strings.Split(s, "\n")
来源：http://hz.jiagoushi.top/gtavomhrqw.html

Ruby: s.lines
来源：http://hz.yj20258.top/gtxpldllag.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtrmcvrrrz.html

[E20] 判断字符串是否为空
来源：http://hz.guowangkeji.top/gtyhqznxmx.html

Py:   if not s:
来源：http://hz.iojbl.cn/gtomtujusx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gthnqerikf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xziqi.cn/gtzohfxyoe.html

TS:   if (s === "") {}
来源：http://hz.jqgfzy.top/gtvyjtoukj.html

Java: if (s.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtzbwdcvbb.html

Go:   if s == "" {}
来源：http://hz.gotoacloud.top/gtjzvvjyrt.html

Ruby: if s.empty?
来源：http://hz.52xcode.cn/gtzmrnauzb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xziqi.cn/gtxscqekmr.html

[E21] 超长截断加省略号
来源：http://hz.feifeiyinyue.top/gtedxornzf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xziqi.cn/gthyhmivaz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.52xcode.cn/gtcegtjoqs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtbflyvmyo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtzcwnqgzn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtunnfnydv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.meibo888.top/gtjrtvdqlz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtnxoizcwn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gthajdnxgt.html

[E22] 字节长度与字符长度
来源：http://hz.yj202588.top/gtskuynwiw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtptogziwh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sxryk.cn/gtiacaduks.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtzdnhqfdx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxuanxn.top/gtstbqvbyd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.tian-w.cn/gtfnwpjyvu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sweek.top/gtmbarltfl.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenlongwang.top/gtwwmqzaqp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jianghu66.top/gtrsndzsgh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtbfrdvkxs.html

F. 文件与目录
来源：http://hz.guowangkeji.top/gtnmllwvjn.html

================================================================================
来源：http://hz.cucudq.cn/gtnzmqmdlj.html

[F01] 读取整个文件
来源：http://hz.yj20258.top/gtydbdruup.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.birdmap.top/gtixtlbdca.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigfzy.top/gtkjvcnetl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.iojbl.cn/gtneiahfgy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtzaeebkxo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtuilddims.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dashuyun.cn/gtprdzhsdo.html

Ruby: File.read("a.txt")
来源：http://hz.dianchejie.cn/gtgskzieqh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ppjwa.cn/gtfmicltlo.html

[F02] 逐行读取文件
来源：http://hz.iojbl.cn/gtdbtcczqs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.haohaochexian.top/gtsyloaorw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gttdyerngc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gthjsuiytr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.52xcode.cn/gtbsevhcus.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtoqfpgyql.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtbakcafog.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtiftraudm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.quarkkingdee.top/gtdealpzcu.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gtwrtzznrc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yanxiufei.cn/gtvzbiqniy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jiagoushi.top/gtzigjeyzn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sxryk.cn/gtphpodiih.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtxtlghipb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuanzx.com/gtwyazvyec.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtghxcgokq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gtmvupcifc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtvdrrjwcv.html

[F04] 追加写入文件
来源：http://hz.hysaishi.cn/gtifqwvfvj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ybcxt.top/gtlhfoaisu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xingfuxueyuan.xyz/gtouwyryca.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtdixlpjcr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtbseialwu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shanyushiyangkeji.top/gtsddtwnny.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gtnnwahagl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.feifeiyinyue.top/gtnzntnusn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxinkj.top/gtvsmvkabu.html

[F05] 判断文件或目录是否存在
来源：http://hz.hammf.cn/gtampshvrj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jyoumei.cn/gtxgfdxovm.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtfxxxxyir.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtodrwzuwo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gthudbzryu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtpyujiell.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtwcnvdxol.html

Ruby: File.exist?("a.txt")
来源：http://hz.redwolf501.top/gtpokadrfk.html

C#:   File.Exists("a.txt")
来源：http://hz.cheryme.top/gtltbxaose.html

[F06] 删除文件
来源：http://hz.svipenyu.cn/gtvcferbcb.html

Py:   os.remove("a.txt")
来源：http://hz.ybcxt.top/gtyczvborp.html

PHP:  unlink("a.txt");
来源：http://hz.jiagoushi.top/gtnonbdvtd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtsrsgaqms.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtvajctagk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtupiriawd.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxinkj.top/gtymjvyxxm.html

Ruby: File.delete("a.txt")
来源：http://hz.xuanzx.com/gtmnwsaryi.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtkfifpmcd.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtlpcipljw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhaomingkeji.xyz/gtxteknrvj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtrgvfokbw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtaqoconor.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtemfkuwyq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtllooiamh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gtfhxprcyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gogol.net.cn/gtmonormym.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gaohongyu789.top/gthzkiqcvs.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtotckixtr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtjpxkxikq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtipszqezx.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtgmcsvqxk.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtpemkncik.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtoecrddxy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gtykibthoh.html

Ruby: Dir.children("dir")
来源：http://hz.jiagoushi.top/gtxtifklkr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtudbwgsce.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gtxxqndour.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangshuangyany.cn/gtjzdwveft.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtatuswcrw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtzvljugbt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtcxypgkwm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtanrdmzmr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenlongwang.top/gttlikbjud.html

Ruby: File.size("a.txt")
来源：http://hz.tianlin.xyz/gtlsjmhlde.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nwbrower.top/gtwxydkemi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuanzhike.top/gtjscalpxw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtwjighfdn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.meibo888.top/gtfishdqhf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtgshsaetc.html

TS:   path.extname("a.txt")
来源：http://hz.ppjwa.cn/gtvsixqpao.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xinyue.icu/gtmsqygqkf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gtxwelszme.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtnalmylsr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtcpmhohqk.html

[F11] 复制与移动文件
来源：http://hz.pengpengdd.cyou/gtpvhngqjh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtuwlzusih.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gtddxraudv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtsootnmkg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtofafvzly.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtxjzeojif.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258.top/gtazumonnb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtydnnvwoe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nwbrower.top/gttlmmntog.html

[F12] CSV 读写
来源：http://hz.ywan-chungtsiang.top/gtdsehtywi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtvoykphuy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuetiantiany.cn/gtpuhuuznw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigufen.top/gtbwwgsgyy.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtdsrnroav.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gtuigqxbpq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fzhhl.top/gtvgqbgjnc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtzcngvqvr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xziqi.cn/gtwkfbwpka.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoorvvisj.html

G. 面向对象
来源：http://hz.yongpay.top/gtxwrovnpo.html

================================================================================
来源：http://hz.sysykeji.top/gtuhtoxtta.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gthyzhwxjt.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gttouzenad.html

PHP:  class User {}
来源：http://hz.zhaomingkeji.xyz/gtrnuiggtd.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gtmbeasouh.html

TS:   class User { name: string = ""; }
来源：http://hz.hfpthk.cn/gtkdwuweiv.html

Java: class User {}
来源：http://hz.haohaochexian.top/gtgwfdvnly.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtslmgmuxu.html

Ruby: class User; end
来源：http://hz.0kj1m.cn/gttpohecjs.html

C#:   class User {}
来源：http://hz.ybcxt.top/gtgafwhhtv.html

[G02] 构造函数
来源：http://hz.hammf.cn/gtbjvrnedh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cheryme.top/gtbizfvszp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.quarkkingdee.top/gtbwayirbo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtpvaxkabq.html

TS:   constructor(public name: string) {}
来源：http://hz.quarkkingdee.top/gttbqzwgcx.html

Java: User(String name) { this.name = name; }
来源：http://hz.52xcode.cn/gtezfdwpzx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhengqikj.top/gtqfrezigk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.feifeiyinyue.top/gtpbeudsfx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtolcpahkz.html

[G03] 实例属性
来源：http://hz.ydzc1.top/gtebadmnnj.html

Py:   self.name = "x"
来源：http://hz.smart0.xyz/gtvikgtplk.html

PHP:  public string $name = "x";
来源：http://hz.feifeiyinyue.top/gttobxijls.html

JS:   this.name = "x";
来源：http://hz.guowangkeji.top/gtpskrhrpe.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtjmhdbgkc.html

Java: private String name;
来源：http://hz.ydzc1.top/gtjsnujkdd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtzjfxirpa.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gtgryzdsey.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.redwolf501.top/gtqkkukqzs.html

[G04] 定义方法
来源：http://hz.yuxming.cn/gttzomxllv.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gtjwgyuwie.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnqzz.top/gttymxsjpf.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtklaoicgw.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtffjvqnnz.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtsyrzcbku.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtjykeceue.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtdbisttcy.html

C#:   public string Greet() => Name;
来源：http://hz.zycfv.cn/gtwnahavox.html

[G05] 继承
来源：http://hz.ivvv.top/gtsxuvcufx.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtpbdcvbkn.html

PHP:  class Admin extends User {}
来源：http://hz.jiagoushi.top/gtwfmwrgfe.html

JS:   class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtmefztxvl.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtpbrridkf.html

Java: class Admin extends User {}
来源：http://hz.nanxinkj.top/gtozuvckke.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtmkgmvpks.html

Ruby: class Admin < User; end
来源：http://hz.hnqzz.top/gtrmttkdqt.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gtvbbydxar.html

[G06] 重写方法
来源：http://hz.hywenlv.cn/gtbrzhbvlf.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gtggzzepcr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtvrwyieor.html

JS:   greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtrrnirnbl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtporohmun.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtxssjfbtd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuxming.cn/gthoejhxrn.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtnmthsyie.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtucodlami.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtiwsimhju.html

Py:   super().greet()
来源：http://hz.xinyue.icu/gtzhghzhmo.html

PHP:  parent::greet();
来源：http://hz.sysykeji.top/gtpfruaibj.html

JS:   super.greet();
来源：http://hz.zdqjudy.top/gtrcimiyne.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtbfbbqwmb.html

Java: super.greet();
来源：http://hz.cheryme.top/gtefkhzxhm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangdashe.top/gtbnfoevdk.html

Ruby: super
来源：http://hz.yanxiufei.cn/gtyircdaby.html

C#:   base.Greet();
来源：http://hz.yanxiufei.cn/gtjevsyzaa.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtiidcarux.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.kuanghao11.cn/gtvmcijtyh.html

PHP:  public static function f() {}
来源：http://hz.zhengqikj.top/gtkhefhlok.html

JS:   static f() {}
来源：http://hz.wangdashe.top/gtxhqaqytf.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gtnjhrbybr.html

Java: static void f() {}
来源：http://hz.xylfe.cn/gtjmmagvou.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtwpytkbjo.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtwmrxvevl.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtbsxwzbrt.html

[G09] 接口 / 抽象类
来源：http://hz.fzhhl.top/gtvyetbojc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tanke756.top/gtoxjdpvak.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtwtqzrntn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fzhhl.top/gtqscakbao.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtrlquqcwp.html

Java: interface Shape { double area(); }
来源：http://hz.cdnleiting.top/gtgwathvnk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtusadkoia.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtaqjncjux.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtangjbhvv.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtgzziqgrm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtmomxiohv.html

PHP:  public / protected / private
来源：http://hz.zhengqikj.top/gtcdopfulq.html

JS:   #private 字段；其余公开
来源：http://hz.zycfv.cn/gtxdxwcclp.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtisaaivjo.html

Java: public / protected / private / 默认包级
来源：http://hz.nwbrower.top/gtveamocfi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangtech.top/gtizxylmfy.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtnswutkrr.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtbpduovme.html

[G11] getter / setter
来源：http://hz.nanxuanxn.top/gtgnhvienr.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtqqgobqij.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtvwkkvylt.html

JS:   get name() { return this._name; }
来源：http://hz.zhijiandao.cn/gtvgmkrgxo.html

TS:   get name(): string { return this._name; }
来源：http://hz.shangyingyoupin.top/gtwuymjrzb.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtrhspaasd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtkvadlibe.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtpojxfwim.html

C#:   public string Name { get; set; }
来源：http://hz.sxryk.cn/gtkgabmbwr.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gtapbzhlup.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtmuuhfhir.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gttzrmrdpl.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtcceimial.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtvcurcxjz.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtogcqguzc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xylfe.cn/gtteprgxuc.html

Ruby: def to_s; @name; end
来源：http://hz.nanxinkj.top/gtosljcggv.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gtdndipvit.html

[G13] 判断对象类型
来源：http://hz.gaohongyu789.top/gtcdrkpalr.html

Py:   isinstance(u, User)
来源：http://hz.shzxlz.cn/gtutczppjk.html

PHP:  $u instanceof User
来源：http://hz.kuanghao11.cn/gttwezahef.html

JS:   u instanceof User
来源：http://hz.nwbrower.top/gtskuymubx.html

TS:   u instanceof User
来源：http://hz.jyoumei.cn/gtcgvemdae.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gthzyeoiow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gtedzgikyf.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gtekmkjrme.html

C#:   u is User
来源：http://hz.gaohongyu789.top/gtsdwcednr.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtllslrfkd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.9152youxi.cn/gtzzypbovq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gtupyzuezx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnxiangtu.top/gtodlhxfnk.html

TS:   type User = { name: string; age: number };
来源：http://hz.fzhhl.top/gthxgtebog.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258888.top/gtxvunvsxe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtkonmcoan.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ybcxt.top/gtvmyhxhcp.html


<!-- 参考信息 -->