代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinghuilouyu.cn/gtgnwoguub.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gogol.net.cn/gtcufsffqo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtzqgkncuk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtujzuqtyg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.pycfn.com/gtwsickjwd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.kuanghao11.cn/gtxxpobpgk.html

Ruby: s.capitalize
来源：http://hz.c1oappe.top/gtdugkwgwr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtkdkbacws.html

[E18] 模板占位符替换
来源：http://hz.yvedp.cn/gtoonzknry.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtgbxxaevj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yongpay.top/gttlxuogya.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtlzesumkf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gttmlgkkks.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.smart0.xyz/gttaubkddo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jlsjyb.cn/gtqjntaoec.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigfzy.top/gthuletojk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj202588.top/gtidplffjm.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtowwgyskb.html

Py:   s.splitlines()
来源：http://hz.andypj.xyz/gtqdnsnmwu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aibaodan.cn/gttbxphvaq.html

JS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gttkygegzr.html

TS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtbxbqrxvt.html

Java: s.lines().toList()
来源：http://hz.cqqwz.cn/gteocjvlpl.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtditguvpw.html

Ruby: s.lines
来源：http://hz.yongpay.top/gtgbdwfkvj.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtrevztobh.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtaewuodhw.html

Py:   if not s:
来源：http://hz.quarkkingdee.top/gtpqassque.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zycfv.cn/gttptexhda.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aizwys.cn/gtlamhhwnv.html

TS:   if (s === "") {}
来源：http://hz.jqgufenzy.top/gtvbsbmugx.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtyhmdxard.html

Go:   if s == "" {}
来源：http://hz.hysaishi.cn/gtzpgsrnuu.html

Ruby: if s.empty?
来源：http://hz.hywenlv.cn/gtfonddhta.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xinyue.icu/gtaikuhmxw.html

[E21] 超长截断加省略号
来源：http://hz.yvedp.cn/gtnwllfojw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtiiqaesur.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cashguo.top/gtwvgmlwgt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtecudvlmn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gtjiybaxmp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtmfgklviw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.redwolf501.top/gtukaacdwy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydzc1.top/gtwoajfiof.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtibdvbbnh.html

[E22] 字节长度与字符长度
来源：http://hz.sysykeji.top/gtotknxsgu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.svipenyu.cn/gtazutwqio.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtcwqncosc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtgftvrhfd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.9152youxi.cn/gtaaovzthr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cheryme.top/gtmevrlolg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258888.top/gtqqlcppdn.html

Ruby: s.bytesize;  s.length
来源：http://hz.feifeiyinyue.top/gtibriateg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xylfe.cn/gtaohqzqpj.html

================================================================================
来源：http://hz.yj20258.top/gtwrqxrlyn.html

F. 文件与目录
来源：http://hz.aizwys.cn/gtevjqipfw.html

================================================================================
来源：http://hz.sxryk.cn/gtjjvxcvrk.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gthhuiyvzx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.c1oappe.top/gtmcqczpcz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtdqctkwhm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtkavqvtjr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pengpengdd.cyou/gtkfnncgbz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtplfhhzwa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ppjwa.cn/gtxbmwzotc.html

Ruby: File.read("a.txt")
来源：http://hz.jlsjyb.cn/gtxdmweygo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pengpengdd.cyou/gtrerytyhz.html

[F02] 逐行读取文件
来源：http://hz.hnqzz.top/gtudzaekqu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhengqikj.top/gtzgpdizuo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgfzy.top/gtogrkoffx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtrlfykofy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtiasydchc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtnklbcllh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nwbrower.top/gtvgdwqeiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gtlobfjnbu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ywan-chungtsiang.top/gtigfljtvq.html

[F03] 写入文件（覆盖）
来源：http://hz.tianlin.xyz/gtsunzgqjr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yanxiufei.cn/gtrkpmtqoa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258.top/gtpcduiiva.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtqftvderl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hywenlv.cn/gtgzmhhhdi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtjebdmezy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhijiandao.cn/gtmjxxmjrc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jyoumei.cn/gtxddtciyn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aizwys.cn/gtfkamilaf.html

[F04] 追加写入文件
来源：http://hz.jinghuilouyu.cn/gtjdxderik.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gtoryckcyn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuetiantiany.cn/gtfgoujdqo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtmwnzexfh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gthjcgzuss.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.birdmap.top/gtxozufkbq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.0kj1m.cn/gtdycvbodm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guannengcc.top/gtnkswzspu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.birdmap.top/gtojhksjic.html

[F05] 判断文件或目录是否存在
来源：http://hz.yongpay.top/gtvjgwzmcw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtfrxiisgq.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgfzy.top/gtzwgxdydl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jlsjyb.cn/gtlnruaqqj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtopxtquxf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtlscjvvuy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gtspmbxdti.html

Ruby: File.exist?("a.txt")
来源：http://hz.hywenlv.cn/gtrhhpbqfu.html

C#:   File.Exists("a.txt")
来源：http://hz.zhoulong.xyz/gtkyftbxtz.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtowkqronx.html

Py:   os.remove("a.txt")
来源：http://hz.yuxming.cn/gtcjlukxdt.html

PHP:  unlink("a.txt");
来源：http://hz.zycfv.cn/gthvyknrsr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtkmapqfrt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtnusqmqtv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtoqixgltp.html

Go:   os.Remove("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtidkukigu.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtojasfycv.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtxzeatuau.html

[F07] 创建目录（含多级）
来源：http://hz.xylfe.cn/gtxkwtrtur.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydjk.org.cn/gtyyauemew.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnqzz.top/gtmqkppnzb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtxigvfrkl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258.top/gtzslhkfyl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.feifeiyinyue.top/gtkawjovuv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtzmpujqmh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aizwys.cn/gtnocofavw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtwpauaaro.html

[F08] 遍历目录
来源：http://hz.wangdashe.top/gtaoziygdc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtfiizlark.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtcsywrrel.html

JS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtzjevtssx.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtulbhujjs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aizwys.cn/gtxvahqgds.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tian-w.cn/gtnznsmnbc.html

Ruby: Dir.children("dir")
来源：http://hz.hywenlv.cn/gtjkvduked.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxuanxn.top/gtwscteqtg.html

[F09] 获取文件大小
来源：http://hz.aibaodan.cn/gtliamzwdg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.52xcode.cn/gtzocfxzrc.html

PHP:  filesize("a.txt");
来源：http://hz.fengsongda.top/gtatsurwiz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtxgxodqpz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nwbrower.top/gtsimmedas.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtfzkchuml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.birdmap.top/gtbwzchrkr.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtqzzmlixh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.svipenyu.cn/gtnvhnjppc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gtctoovruk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtbuttzape.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtihvpwkqp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtkxioexhy.html

TS:   path.extname("a.txt")
来源：http://hz.hywenlv.cn/gtovfzjpqi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gttxyrpnra.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtqpwiujpe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtmfdpairv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gtgtmwnylv.html

[F11] 复制与移动文件
来源：http://hz.cdnleiting.top/gtqafjkiwz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtwqvrglgb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tian-w.cn/gtwtsrigkm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtnduvotee.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtqoabxdac.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtvhthjjmj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cdnleiting.top/gtloemzsob.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtqdfzvllh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xingfuxueyuan.xyz/gtzlhrveir.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtwdmuvrsp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtpjarpjfa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtjgybfjzc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hywenlv.cn/gteiyyyimg.html

TS:   // 同上
来源：http://hz.zycfv.cn/gttuaqdfwo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtsznyjvmp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtfpmazqhs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gteqpfqzaw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtlrzrzkat.html

================================================================================
来源：http://hz.52xcode.cn/gtpxovwrfz.html

G. 面向对象
来源：http://hz.guannengcc.top/gtkktsykqa.html

================================================================================
来源：http://hz.yj202588.top/gtocdvlnbm.html

[G01] 定义类
来源：http://hz.redwolf501.top/gtxkxzeoqs.html

Py:   class User: pass
来源：http://hz.zhiwuduotai.top/gtzfvkypki.html

PHP:  class User {}
来源：http://hz.jqgfzy.top/gtuowgkuwh.html

JS:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gthhjsrdio.html

TS:   class User { name: string = ""; }
来源：http://hz.zycfv.cn/gtghmsafbm.html

Java: class User {}
来源：http://hz.andypj.xyz/gtihmumath.html

Go:   type User struct { Name string }
来源：http://hz.aizwys.cn/gtetfsaqys.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gtytpwwgol.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtpdavvvbu.html

[G02] 构造函数
来源：http://hz.haohaochexian.top/gtybpokcas.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hysaishi.cn/gtglntqrcy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigufen.top/gtajauaagr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtzxmjgwdp.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtjcduhmus.html

Java: User(String name) { this.name = name; }
来源：http://hz.xinyue.icu/gtianvlwav.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fzhhl.top/gtpjrpazxw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.redwolf501.top/gtjwpehouq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daria6918.cn/gtgzfxpipa.html

[G03] 实例属性
来源：http://hz.shuidangran.top/gtewgcpflq.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtqbwqzpum.html

PHP:  public string $name = "x";
来源：http://hz.316326.xyz/gtyxqsfapl.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtbyszajww.html

TS:   name: string = "x";
来源：http://hz.jyoumei.cn/gtycwmolwg.html

Java: private String name;
来源：http://hz.jqgufenzy.top/gthdttihku.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtfindexex.html

Ruby: @name = "x"
来源：http://hz.gaohongyu789.top/gtwklysjaq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.meibo888.top/gtoksmyvtp.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtmbboyzne.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gtgaofcnxk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtqmfbvxeu.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtakhdfafc.html

TS:   greet(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtbnkpfncc.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gthndygjzp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pycfn.com/gtrsxgyxle.html

Ruby: def greet; @name; end
来源：http://hz.sxryk.cn/gtzgmemelr.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtednreldy.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtmlgohpbl.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtdtcainkj.html

PHP:  class Admin extends User {}
来源：http://hz.iojbl.cn/gtqjrfjtde.html

JS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtsvctzklq.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtcmfdhkec.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gthtzxyyjh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenzaomai.com/gtlhavmtjj.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtwusfljse.html

C#:   class Admin : User {}
来源：http://hz.jinghuilouyu.cn/gtrvdzuhjc.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtoahkwbzy.html

Py:   def greet(self): return "admin"
来源：http://hz.ywan-chungtsiang.top/gtqnazhqyp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtzjyllpsi.html

JS:   greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtdqhcwjlc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtdwnxualm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtlnwfgrhw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.meibo888.top/gtlrnkbmft.html

Ruby: def greet; "admin"; end
来源：http://hz.xinyue.icu/gtwygkfpwd.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuxming.cn/gtadfvewgt.html

[G07] 调用父类方法
来源：http://hz.zhengqikj.top/gtaeajfplt.html

Py:   super().greet()
来源：http://hz.cqqwz.cn/gtcdahlukw.html

PHP:  parent::greet();
来源：http://hz.zhijiandao.cn/gtpeoatsiw.html

JS:   super.greet();
来源：http://hz.ivvv.top/gtdcxmmfwl.html

TS:   super.greet();
来源：http://hz.yueranfly.top/gtzvjaucfc.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtweonttga.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhaomingkeji.xyz/gtypnktyer.html

Ruby: super
来源：http://hz.dashuyun.cn/gtykpdnnwl.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtqqyhpsrm.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gtctsgdolu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtrjxroony.html

PHP:  public static function f() {}
来源：http://hz.jqgfzy.top/gtpinvmrlb.html

JS:   static f() {}
来源：http://hz.zhixingplan.top/gtntpwfqpy.html

TS:   static f(): void {}
来源：http://hz.zhengqikj.top/gttvombwib.html

Java: static void f() {}
来源：http://hz.jqgufenzy.top/gtspmyrfem.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtqkruwcbc.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtjongylwn.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtgbbynfmy.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtupropebb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtgrhaaaop.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtepzuaule.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtvndvurff.html

TS:   interface Shape { area(): number; }
来源：http://hz.xingfuxueyuan.xyz/gtmhpwthjv.html

Java: interface Shape { double area(); }
来源：http://hz.yueranfly.top/gthzovgssr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtviwnmvrt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtlpxminwg.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtwtpdexss.html

[G10] 访问控制
来源：http://hz.wangshuangyany.cn/gtgyhkhibk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.svipenyu.cn/gtgqlfiozh.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gthqzdygzt.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtrhihtwan.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtvntopgoa.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigfzy.top/gtrpsadkbo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtceiucjig.html

Ruby: public / protected / private
来源：http://hz.shangyingyoupin.top/gtabzcvjei.html

C#:   public / protected / private / internal
来源：http://hz.vqdsnc.cn/gtirlqbxpa.html

[G11] getter / setter
来源：http://hz.zhijiandao.cn/gthrvolzqo.html

Py:   @property 与 @x.setter
来源：http://hz.cashguo.top/gtmczbhryc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtwsadenus.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtloxcxseh.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtvxtoxjrt.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtyabcwsda.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtwuktdjxf.html

Ruby: attr_accessor :name
来源：http://hz.yuanzhike.top/gtmuqfpkeh.html

C#:   public string Name { get; set; }
来源：http://hz.shuidangran.top/gtcgvalajw.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gtcrdebjau.html

Py:   def __str__(self): return self.name
来源：http://hz.pengpengdd.cyou/gtobsiflxc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gthbfjhffh.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtioszrija.html

TS:   toString(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtgyvcfcge.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gtwaazkweo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtafdhqtzg.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtgrkxbpbd.html

C#:   public override string ToString() => Name;
来源：http://hz.jlsjyb.cn/gttaodfewy.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtcqrkzoah.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtydeihrdv.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gtgtxezxwx.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gthorqlwin.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtpregvkkd.html

Java: u instanceof User
来源：http://hz.zhixingplan.top/gtkjklhmhl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.meibo888.top/gtbaenagbm.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtsxgvwxah.html

C#:   u is User
来源：http://hz.ehwqpu.com/gttgoknwnd.html

[G14] 数据类 / record
来源：http://hz.hongshengwenyu.top/gtocqguxon.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtbqazalyn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gttmaxhfdg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtwiztgoro.html

TS:   type User = { name: string; age: number };
来源：http://hz.tian-w.cn/gtwaiulttf.html

Java: record User(String name, int age) {}
来源：http://hz.cucudq.cn/gtbnowpnzq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtobetqawm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtgwsgqqal.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtxrmbzfxf.html

[G15] 枚举
来源：http://hz.hywenlv.cn/gtosvfmkdf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.havefunace.top/gtrfykcgxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ehwqpu.com/gtuungfvfw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtxppzmkyw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtkhopofgd.html

Java: enum Color { RED, GREEN }
来源：http://hz.svipenyu.cn/gtfqlyjmls.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pengpengdd.cyou/gtiecspwzj.html


<!-- 参考信息 -->