代发 wailian999

PHP:  number_format(1234567);
来源：http://hz.xylfe.cn/gtjyzmglja.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtscxmdpui.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sweek.top/gtmzabkmoo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhoulong.xyz/gtxohudpwo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tian-w.cn/gtpwqpisxn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhaomingkeji.xyz/gtdaynhdnw.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtlycwjijt.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtqyoqiwyn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gotoacloud.top/gtxjyjtsnb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ivvv.top/gtiozpenno.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtsysgfxaw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtnksdwfsw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hysaishi.cn/gtbolaqsam.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dianchejie.cn/gtydpydqav.html

Ruby: s.capitalize
来源：http://hz.ybcxt.top/gtrzzwolqp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shuidangran.top/gthcumasax.html

[E18] 模板占位符替换
来源：http://hz.meibo888.top/gtvhplemwz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtztbvtuki.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nwbrower.top/gteciizwhf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtcxgwhbzg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtihqrcweu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gtrgyguxat.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jlsjyb.cn/gthwybezry.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtijktugcy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtpmzzfyaw.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gtenoyeotu.html

Py:   s.splitlines()
来源：http://hz.pycfn.com/gthggkdpft.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xylfe.cn/gtpaugcyvm.html

JS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gttjjuawvc.html

TS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtxqafopbx.html

Java: s.lines().toList()
来源：http://hz.jinqigfzy.top/gtuvmuplfx.html

Go:   strings.Split(s, "\n")
来源：http://hz.gzhubu.top/gthrlfsoke.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gtqcanvqmq.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gtybvrmmyc.html

[E20] 判断字符串是否为空
来源：http://hz.quarkkingdee.top/gtljrkmboy.html

Py:   if not s:
来源：http://hz.shangyingyoupin.top/gtivsyyhxd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gtxdneqyte.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cdnleiting.top/gtuhjutovv.html

TS:   if (s === "") {}
来源：http://hz.quarkkingdee.top/gtbmcprcdt.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtwhzeidey.html

Go:   if s == "" {}
来源：http://hz.yongpay.top/gtexliixgf.html

Ruby: if s.empty?
来源：http://hz.hnxiangtu.top/gtqxuxpcut.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gtsuyohpxp.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtxwuaomsw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtjwmvomzu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtieiremnb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtnpkanxau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtwvfndpon.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtwuunikmq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtntbxefje.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhongyouzk.top/gtllznaiip.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.smart0.xyz/gtpvjqayil.html

[E22] 字节长度与字符长度
来源：http://hz.hammf.cn/gthegxtebx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guannengcc.top/gtligvaqyf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtrfmqnddf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtovzgqspb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.andypj.xyz/gtkcszgbnc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtbjbjhyup.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gthkokzkrp.html

Ruby: s.bytesize;  s.length
来源：http://hz.gotoacloud.top/gtdarfcuph.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sufxvd.cn/gtdgvlsika.html

================================================================================
来源：http://hz.yongpay.top/gtttccgeke.html

F. 文件与目录
来源：http://hz.shanyushiyangkeji.top/gtchmaiedy.html

================================================================================
来源：http://hz.sufxvd.cn/gtafxpbbor.html

[F01] 读取整个文件
来源：http://hz.xinyue.icu/gtcqifucpf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sweek.top/gtkngscvtv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtaxpkypgi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tianlin.xyz/gtaqkyjwft.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinghuilouyu.cn/gtfqvtpaht.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtqbrwfhdy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.0kj1m.cn/gthcavcece.html

Ruby: File.read("a.txt")
来源：http://hz.gaohongyu789.top/gtrrtlxhzo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258.top/gtdttvfxnu.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtfctjomcl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hammf.cn/gtuapzxpzm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.0kj1m.cn/gtlygaxhbc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtdelkhahh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtwkqckaln.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtonfcsbiz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtpebdqxwp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jianghu66.top/gtptewyxpy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangdashe.top/gtnveysscd.html

[F03] 写入文件（覆盖）
来源：http://hz.zhengqikj.top/gtqohdoitc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangshuangyany.cn/gtyicsetzm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zycfv.cn/gtwpsektzw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtdiepkals.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtmmtfblmg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtsuiarkgm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtshcbefbf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cqqwz.cn/gtuznzdowx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pycfn.com/gthedxqgih.html

[F04] 追加写入文件
来源：http://hz.zhixingplan.top/gtqgfxjrun.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gttmwxgjrm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtbraajqsp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtopiulnwd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtuwlisqtp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtotbbzjya.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtsdivthzk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtikhuauim.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yuanzhike.top/gtlsgrpucg.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhongyouzk.top/gtnywgalmv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gtqfyfhsxj.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtxnotuwtx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gttpzdtuoa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtyjyqjulr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtlodgozew.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhoulong.xyz/gtjwtxswau.html

Ruby: File.exist?("a.txt")
来源：http://hz.nwbrower.top/gtfewewyia.html

C#:   File.Exists("a.txt")
来源：http://hz.svipenyu.cn/gtldzkotjw.html

[F06] 删除文件
来源：http://hz.haohaochexian.top/gtttjejonn.html

Py:   os.remove("a.txt")
来源：http://hz.shzxlz.cn/gtpmpjojsn.html

PHP:  unlink("a.txt");
来源：http://hz.nwbrower.top/gtkctfddbm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtxpxhzacp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtdohokase.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtcylbontw.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtoeoujxag.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtcthpwijm.html

C#:   File.Delete("a.txt");
来源：http://hz.yonumen.top/gtgdlrepky.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtjrtxywnm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gaohongyu789.top/gtuxtlrdab.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtmiymzgdd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gthimeuocr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtexhuyocv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtzbmitugr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.havefunace.top/gtucaezvnl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258888.top/gtclkpytxo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtejdvtasx.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gtkzrhfqod.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinyuanbaomall.cn/gtizstegyz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sufxvd.cn/gtwwlygsyu.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtnsehqlvz.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtmwwstffw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtcxqvusbu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtclesghej.html

Ruby: Dir.children("dir")
来源：http://hz.ywan-chungtsiang.top/gtmhwkaefn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guannengcc.top/gtfnvfshio.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtifzfqfxo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hfpthk.cn/gtfjihgqjn.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtkxdpniqw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtpvzfwbeb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtodxpoiji.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gttjgfskmj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shangyingyoupin.top/gtereeswmd.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtplprhlle.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtehzmkvtv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gtavltvfvh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtwadxstwi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yvedp.cn/gtvocspnyp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtfizqfhaf.html

TS:   path.extname("a.txt")
来源：http://hz.cucudq.cn/gtvllgnqzj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hammf.cn/gtidkkavke.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xuanzx.com/gtyfkdzzyw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtczzuklzv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtftvwribx.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtxbdgkwvq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtaggrrvno.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtcoyzmnyc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtafbxopds.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtnhmcwnxf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtxgkcvojg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.quarkkingdee.top/gtcazbkyzl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtgvchsvpi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtvjinhwdn.html

[F12] CSV 读写
来源：http://hz.dashuyun.cn/gtuccjnipu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aizwys.cn/gtjhuobfjm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtrpceeqis.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.smart0.xyz/gtvgeejwsm.html

TS:   // 同上
来源：http://hz.gzhubu.top/gtmocuhgtn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtuzbvrbzm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gtsltkusth.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydjk.org.cn/gtcsjyfxkw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuanzhike.top/gtzokfitui.html

================================================================================
来源：http://hz.pycfn.com/gtggyfetjt.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtldvaelia.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtopccjumg.html

[G01] 定义类
来源：http://hz.shanyushiyangkeji.top/gtasshfhrq.html

Py:   class User: pass
来源：http://hz.9152youxi.cn/gtqqfrehts.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtrardpkul.html

JS:   class User {}
来源：http://hz.316326.xyz/gtvqfyeuyf.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtaqgrvetz.html

Java: class User {}
来源：http://hz.wangshuangyany.cn/gtdcuivqbt.html

Go:   type User struct { Name string }
来源：http://hz.mhx1999.top/gthgyzoshl.html

Ruby: class User; end
来源：http://hz.cdnleiting.top/gtgusqbbij.html

C#:   class User {}
来源：http://hz.zycfv.cn/gthzktgton.html

[G02] 构造函数
来源：http://hz.dashuyun.cn/gtllkvinkq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.andypj.xyz/gtdlhjqbgb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gthjllsqiq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtstnfjqqv.html

TS:   constructor(public name: string) {}
来源：http://hz.quarkkingdee.top/gtbrejxgke.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gttajgwpep.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtopbiiesm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangdashe.top/gtuquczkmg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtlkubcyhe.html

[G03] 实例属性
来源：http://hz.xylfe.cn/gttismtmzk.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtmazvqvzh.html

PHP:  public string $name = "x";
来源：http://hz.zhongyouzk.top/gtxeowlawc.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtnimiqzmw.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gttogloxgt.html

Java: private String name;
来源：http://hz.dianchejie.cn/gtuyrvltxs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.meibo888.top/gtlagumquy.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gtjppffifo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtrwtngzcw.html

[G04] 定义方法
来源：http://hz.iojbl.cn/gtbwkyhhrh.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtctyqrehh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtqoxmtlgs.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtygzdstbq.html

TS:   greet(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtmtyrcehv.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtxaudphlp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yonumen.top/gttpqpysdd.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtbpntuhcy.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gtzebognlh.html

[G05] 继承
来源：http://hz.shzxlz.cn/gtcldzpnwr.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtqqxxdrqm.html

PHP:  class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtjudjotew.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtqscjqpnd.html

TS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtdmtuzssk.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtqqsqvqgb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tianlin.xyz/gtgjsdknll.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtwvmbaylj.html

C#:   class Admin : User {}
来源：http://hz.redwolf501.top/gtkidryfrj.html

[G06] 重写方法
来源：http://hz.ydzc1.top/gtduzczscf.html

Py:   def greet(self): return "admin"
来源：http://hz.fzhhl.top/gtzqzurbwi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtbnwecngq.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtawzwudhw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtclhmswwu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gttpcoplaf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtbvooveph.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtqxkdfprg.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtdjnvbmtl.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtmiisbrbz.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtssekihgs.html

PHP:  parent::greet();
来源：http://hz.ehwqpu.com/gtbgcjthoq.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtkhfdlisn.html

TS:   super.greet();
来源：http://hz.dianchejie.cn/gtjdrveuov.html

Java: super.greet();
来源：http://hz.gaohongyu789.top/gtepzvmqtq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yvedp.cn/gtxbaiuwye.html

Ruby: super
来源：http://hz.sysykeji.top/gtmasnjfjx.html

C#:   base.Greet();
来源：http://hz.xinyue.icu/gtrbafhduy.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtvxkvrgmp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtlfxzeefe.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtnavszavk.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtbklczntd.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtgvgupnko.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gtvbjhpsgw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnqzz.top/gtijpwpnfq.html

Ruby: def self.f; end
来源：http://hz.daxiang520.top/gtyisqzbnu.html

C#:   public static void F() {}
来源：http://hz.zdqjudy.top/gtvpjjcilx.html

[G09] 接口 / 抽象类
来源：http://hz.daxiang520.top/gtauokpcxx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gtbxkxardo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhijiandao.cn/gtwollfabr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aizwys.cn/gtkisnyrkj.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtiqucnkrg.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtgerhrfnh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jiagoushi.top/gtjipcgklk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.snrcjt.cn/gtzcpthrrw.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtxcjixbsd.html

[G10] 访问控制
来源：http://hz.meibo888.top/gtlmrfnael.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gtqyjlftev.html

PHP:  public / protected / private
来源：http://hz.zhengqikj.top/gtzkwxxebo.html

JS:   #private 字段；其余公开
来源：http://hz.cashguo.top/gtwtiwgtek.html

TS:   public / protected / private
来源：http://hz.birdmap.top/gtzcocklou.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtwowojsuf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxinkj.top/gtrhuintnx.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtbmwyhmvp.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtjunntntm.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtzmacwphp.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtwhapjqvt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtvlsqpbks.html

JS:   get name() { return this._name; }
来源：http://hz.ehwqpu.com/gtrqmpkqpd.html

TS:   get name(): string { return this._name; }
来源：http://hz.pengpengdd.cyou/gtdnaelfgb.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtmjslgfjc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtgckhceip.html

Ruby: attr_accessor :name
来源：http://hz.0kj1m.cn/gtaezrwssi.html

C#:   public string Name { get; set; }
来源：http://hz.chenzaomai.com/gtnidxeplv.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtnjzwkyjy.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtcmnilgxo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ivvv.top/gtneebpvtx.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gtbaqbyxdx.html

TS:   toString(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtxndpkvgy.html

Java: @Override public String toString() { return name; }
来源：http://hz.birdmap.top/gtomymeyvx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtxtmdnnka.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gthuwwkxmj.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtseoloqek.html

[G13] 判断对象类型
来源：http://hz.birdmap.top/gteydzmdak.html

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtgcgnjskt.html

PHP:  $u instanceof User
来源：http://hz.c1oappe.top/gtarwxnxqz.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtuqtnvafc.html

TS:   u instanceof User
来源：http://hz.gogol.net.cn/gtkmhwelqy.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtbfhnphut.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtovbulnhe.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtzbtqlbka.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtmtudzrqw.html

[G14] 数据类 / record
来源：http://hz.xuanzx.com/gtqadjasmb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigfzy.top/gttwhdwumr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtmldklnhi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj202588.top/gtzvziyttg.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnxiangtu.top/gtenhddgzk.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtuoimkcxh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhiwuduotai.top/gtbwcptvfi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pengpengdd.cyou/gtndzbrncj.html


<!-- 参考信息 -->